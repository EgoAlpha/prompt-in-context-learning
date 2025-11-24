# **第五讲 LangChain关键组件——智能体Agent**



**版本：**

python 3.12

pip install langchain==1.0.3

## 1.基本的智能体创建与使用

利用@tool装饰器创建工具

```Python
# 定义两个工具，计算与搜索
import os
from typing import Literal
from langchain_core.tools import tool
from tavily import TavilyClient

# It's best practice to initialize the client once and reuse it.
tavily_client = TavilyClient(api_key=os.environ["TAVILY_API_KEY"])
# Search tool to use to do research
@tool
def internet_search(
    query: str,
    max_results: int = 5,
    topic: Literal["general", "news", "finance"] = "general",
    include_raw_content: bool = False,
):
    """
    Search the internet for information using Tavily search engine
    """
    search_docs = tavily_client.search(
        query,
        max_results=max_results,
        include_raw_content=include_raw_content,
        topic=topic,
    )
    return search_docs


@tool
def calculate(expression: str) -> str:


    """Perform mathematical calculations and return the result.
    Args:
        expression: Mathematical expression to evaluate 
        (e.g., "2 + 3 * 4", "sqrt(16)", "sin(pi/2)")
    Returns:
        The calculated result as a string
    """
    result = str(eval(expression))
    return result
    
tools = [internet_search,calculate]
```

两种静态创建方法

```python
from langchain.agents import create_agent
from langchain.chat_models import init_chat_model

# 方法一
agent = create_agent(
    "openai:gpt-4",
    tools = tools
)

# 方法二
model =init_chat_model("openai:gpt-4")
agent = create_agent(model,tools = tools)
```

直接调用Agent

```python
res = agent.invoke(
    {"messages":
    [{"role":"user",
    "content":"deepseek在2024-2025年之间，用户增长了百分之多少？"
    }]
    }
)
```

## 2.动态模型的Agent创建

```Python

from langchain.agents import create_agent
from langchain.agents.middleware import wrap_model_call, ModelRequest, ModelResponse         
from langchain.chat_models import init_chat_model

basic_model = init_chat_model("openai:gpt-4o-mini")
advanced_model = init_chat_model("openai:gpt-4o")
@wrap_model_call
def dynamic_model_selection(request: ModelRequest, handler) -> ModelResponse:
    """Choose model based on conversation complexity."""
    message_count = len(request.state["messages"])

    if message_count > 5:
        # 使用高级模型进行更长时间的对话
        model = advanced_model
    else:
        model = basic_model

    request.model = model
    return handler(request)

agent = create_agent(
    model=basic_model,  # 默认模型
    tools=tools,
    middleware=[dynamic_model_selection]
)
```

短消息列表调用

```python
agent.invoke( {"messages": 
    [{"role": "user", 
    "content": "你好"}]
    })
```

长消息列表调用

```python
res["messages"].append(
    {"role": "user", 
    "content": "你认为接下来deepseek的发展前景如何会如何??"}
    )
agent.invoke(res)
```

## 3.系统消息System prompt

静态系统消息设置

```Python
agent = create_agent(
    model,
    tools,
    system_prompt="你是我的得力助手。要做到言简意赅，准确无误的回答我的问题。"
)
```

动态系统消息设置

```python
from typing import TypedDict
from langchain.agents import create_agent
from langchain.agents.middleware import dynamic_prompt, ModelRequest     

class Context(TypedDict):
    user_role: str

@dynamic_prompt
def user_role_prompt(request: ModelRequest) -> str:
    """Generate system prompt based on user role."""
    user_role = request.runtime.context.get("user_role", "user")
    base_prompt = "你是我的得力助手。"

    if user_role == "expert":
        return f"{base_prompt} 提供详细的技术答复。"
    elif user_role == "beginner":
        return f"{base_prompt} 简单解释概念，避免行话。"

    return base_prompt

agent = create_agent(
    model="openai:gpt-4o",
    tools=tools,
    middleware=[user_role_prompt],
    context_schema=Context
)

# 系统提示将根据上下文动态设置
result = agent.invoke(
    {"messages": [{"role": "user", "content": "为我解释机器学习这个概念。"}]},
    context={"user_role": "expert"}
)
```



## 4.结构化输出Structured output

```python
from pydantic import BaseModel
from langchain.agents import create_agent
from langchain.agents.structured_output import ToolStrategy                                     
class ContactInfo(BaseModel):
    name: str
    email: str
    phone: str

agent = create_agent(
    model="openai:gpt-4o-mini",
    tools=tools,
    response_format=ToolStrategy(ContactInfo)
)

result = agent.invoke({
    "messages": [{"role": "user", 
    "content": """从以下内容中提取信息: 大家都觉得非常靠谱的小明，他的具体联系渠道我这里可以给你。
    他总是能及时回复邮件，所以如果你有文件或详细问题，发邮件到 xiaoming@mail.com 这个邮箱地址。
    当然，如果事情比较紧急，或者需要实时语音沟通确认细节，你也可以直接拨打他的个人办公电话，
    号码是 (04xx) 123-4567,这个号码通常在工作日的办公时间内都能接通"""}]
})


print(result["structured_response"])
```

## 5.Agent的多种调用方式

```python
# 基本调用
result = agent.invoke(
    {"messages": [{"role": "user", "content": "What's the weather in San Francisco?"}]}
)
```

```python
# 流式调用
for chunk in agent.stream({"messages": 
    [{"role": "user", 
    "content": "deepseek在2024-2025年之间,用户增长了百分之多少??"}]
    },stream_mode="values"):
    
    latest_message = chunk["messages"][-1]

    if latest_message.content:
        print(f"Agent: {latest_message.content}")
    elif latest_message.tool_calls:
        print(f"Calling tools: {[tc['name'] for tc in latest_message.tool_calls]}")


```

```python
# 异步调用
import asyncio
# 请在非notebook中运行

async def async_invoke():
    response = await agent.ainvoke({"messages": 
    [{"role": "user", 
    "content": "deepseek在2024-2025年之间,用户增长了百分之多少??"}]
    })
    return response

response = asyncio.run(async_invoke())
```
