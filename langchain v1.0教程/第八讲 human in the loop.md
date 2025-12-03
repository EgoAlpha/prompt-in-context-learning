# **第八讲 LangChain  中间件——human in the loop**



**版本：**

python 3.12

pip install langchain==1.0.5

## 1.创建Agent传入中间件

定义模型

```Python
from langchain.chat_models import init_chat_model
model = init_chat_model("openai:gpt-4o-mini",
                        api_key="sk-...",
                        )
```

定义工具（要在同目录下有data.txt文件作为模拟数据）

```python
from langchain_core.tools import tool                                               # 
import os

@tool
def write_txt_tool(path: str, content: str) -> str:
    """将文本内容写入给定路径。"""
    with open(path, "w", encoding="utf-8") as file:
        file.write(content)
    return f"写入完成: {path}"

@tool
def read_txt_tool(path: str) -> str:
    """读取给定路径的文本内容。"""
    with open(path, "r", encoding="utf-8") as file:
        return file.read()

@tool
def delete_txt_tool(path: str) -> str:
    """删除给定路径的文本文件。"""
    if not os.path.exists(path):
        return f"文件不存在: {path}"
    os.remove(path)
    return f"删除完成: {path}"
```

创建Agent

```python
from langchain.agents import create_agent                                             
from langchain.agents.middleware import HumanInTheLoopMiddleware                      
from langgraph.checkpoint.memory import InMemorySaver                                


agent = create_agent(
    model=model,
    tools=[write_txt_tool, read_txt_tool,delete_txt_tool],
    middleware=[
        HumanInTheLoopMiddleware( 
            interrupt_on={
                "write_txt_tool": True, 
                "delete_txt_tool": {"allowed_decisions": ["approve", "reject"]},  
                "read_txt_tool": False,
            },

            description_prefix="工具执行待批准",
        ),
    ],
    checkpointer=InMemorySaver(),  
)
```

## 2.调用Agent

读取文件工具不会触发中间件中断

```Python
config = {"configurable": {"thread_id": "some_id"}} 

result = agent.invoke({"messages":[{"role": "user", 
    "content": "帮我查看data.txt文件中有什么内容?"}]},
    config = config)
```

写入文件工具会触发中间件中断

```python
result_1= agent.invoke({"messages":[{"role": "user", 
    "content": "为我在data.txt中添加小虎的成绩为90。"}]},
    config = config)

print(result_1['__interrupt__'])
```

## 3.响应中断

以approve响应中断

```Python
from langgraph.types import Command                                 
agent.invoke(
    Command( 
        resume={"decisions": [{"type": "approve"}]}
    ), 
    config=config
)
```

其他响应方式

```python
from langgraph.types import Command                                  

agent.invoke(
    Command( 
        resume={"decisions": [{"type": "approve"}]}
    ), 
    config=config
)
```

```python
agent.invoke(
    Command(
        resume={
            "decisions": [
                {
                    "type": "reject",
                    "message": "No, this is wrong because ..., instead do this ...",
                }
            ]
        }
    ),
    config=config
)
```

