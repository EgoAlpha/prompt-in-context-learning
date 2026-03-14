# **第二十一讲 沙箱Sandbox**



**版本：**

python 3.12

langchain==1.2.1

# 模式一



## 1. .env文件

```.env
DEEPSEEK_API_KEY=sk-...
DEEPSEEK_BASE_URL=https://...

# 可选
LANGSMITH_TRACING=true
LANGSMITH_API_KEY=lsv2_...
TAVILY_API_KEY=tvly-...




DAYTONA_API_KEY=dtn_...
DAYTONA_API_URL=https://app.daytona.io/api
```

## 2.Dockerfile文件

```dockerfile
FROM python:3.11-slim

WORKDIR /app

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

RUN mkdir -p /workspace

COPY agent.py .

EXPOSE 8000

CMD ["python", "agent.py"]
```

## 3. requirements.txt文件

```txt
deepagents
langchain-openai
fastapi
uvicorn
python-dotenv

```

## 4.agent.py文件

```python
#!/usr/bin/env python3

import os
from typing import Optional
from fastapi import FastAPI
from pydantic import BaseModel


from deepagents import create_deep_agent
from langchain.chat_models import init_chat_model
from deepagents.backends import LocalShellBackend


BACKEND = LocalShellBackend(
    root_dir="/workspace",
    env={"PATH": "/usr/local/bin:/usr/bin:/bin"},
    inherit_env=False,
    timeout=120,
    max_output_bytes=500_000)



API_KEY = os.getenv("DEEPSEEK_API_KEY")
BASE_URL = os.getenv("DEEPSEEK_BASE_URL")

model = init_chat_model(
    model="openai:deepseek-ai/DeepSeek-V3.2",
    api_key=API_KEY,
    base_url=BASE_URL)

AGENT = create_deep_agent(
    model=model,
    backend=BACKEND)


app = FastAPI(title="DeepAgent in Docker")

class ChatRequest(BaseModel):
    message: str
    thread_id: Optional[str] = "default"

class ChatResponse(BaseModel):
    response: str
    thread_id: str


@app.post("/chat", response_model=ChatResponse)
def chat(request: ChatRequest):
    try:
        result = AGENT.invoke({"messages": [
                {"role": "user", "content": request.message}
            ]},
            config={"configurable": {"thread_id": request.thread_id}},
        )

        return ChatResponse(response=result["messages"][-1].content,
                            thread_id=request.thread_id, )
    except Exception as e:
        return ChatResponse(
            response=f"错误: {str(e)}",
            thread_id=request.thread_id,)


if __name__ == "__main__":
    import uvicorn

    uvicorn.run(app, host="0.0.0.0", port=8000)

```

## 5.client.py文件

```python
import requests

def chat(message, thread_id="default"):
    resp = requests.post(
        "http://localhost:8000/chat",
        json={"message": message, "thread_id": thread_id}
    )
    return resp.json()

# 测试
print("=== 测试1：简单对话 ===")
print(chat("你好，请介绍一下自己", "test-chat"))

print("\n=== 测试2：代码执行 ===")
print(chat("在workspace文件夹下，创建一个Python文件打印Hello World字符串。", "test-code"))

print("\n=== 测试3：查看文件 ===")
print(chat("查看一下workspace中有什么文件", "test-file"))



```

## 6.构建镜像运行沙箱

```bash
# 构建镜像
docker build -t deepagent .

# 运行容器 
docker run -it --rm -p 8000:8000 -v "%cd%/workspace:/workspace" --env-file .env deepagent
```

# 模式二：Sandbox  as tools



```python
from daytona import Daytona,DaytonaConfig
import os
from deepagents import create_deep_agent
from langchain_daytona import DaytonaSandbox
from langchain.chat_models import init_chat_model
from dotenv import load_dotenv

load_dotenv()

config = DaytonaConfig(api_key=os.getenv("DAYTONA_API_KEY"))
daytona = Daytona(config)

sandbox = daytona.create()
backend = DaytonaSandbox(sandbox=sandbox)

model = init_chat_model(
    model="openai:deepseek-ai/DeepSeek-V3.2",
    api_key=os.getenv("DEEPSEEK_API_KEY"),
    base_url=os.getenv("DEEPSEEK_BASE_URL"))


agent = create_deep_agent(
    model=model,
    system_prompt="你是一位拥有沙盒访问权限的Python编码助手。",
    backend=backend,
)

result = agent.invoke({
        "messages": [{
                "role": "user",
                "content": "编写一个python代码计算：57的十一次方。",
            }]})

for mes in result["messages"]:
    print(mes.content)

sandbox.stop()
```

