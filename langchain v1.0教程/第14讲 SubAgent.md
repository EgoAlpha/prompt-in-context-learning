# **第十四讲 LangChain  ——子代理SubAgent**



**版本：**

python 3.12

pip install langchain==1.0.5

pip deepagents == 0.3.0

（1.0.5之前Summarization中间件参数会有变动）

## 1.创建模型对象



```Python
from langchain.chat_models import init_chat_model

# 或者导入环境变量
api_key="sk-..."
base_url="https://..."

model = init_chat_model("openai:gpt-4o-mini",
                        api_key=api_key,
                        base_url=base_url
)

```

## 2.创建工具对象



```Python
import os
from typing import Literal
from langchain_core.tools import tool
from tavily import TavilyClient

# 定义自己的key
tavily_client = TavilyClient(api_key=os.environ["TAVILY_API_KEY"])

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
```

## 3.基本字典创建：dictionary-base



```Python
from deepagents import create_deep_agent
internet_subagent = {
    "name": "internet-agent",
    "description": "Utilise online tools to search for information on the internet",
    "system_prompt": "You are a great Internet searcher",
    "tools": [internet_search],
    "model": model,  
}
agent = create_deep_agent(
    model=model,
    subagents=[internet_subagent]
)
```

## 4.调用与观察



```Python
from langchain.messages import HumanMessage
res = agent.invoke({"messages":
[HumanMessage(
    "进行网络搜索获取数据,比对deepseek模型的用户使用量,2024到2025年的增长了百分之多少??")]
})

# 观察task工具调用
print(res["messages"][1].tool_calls)

# 观察子代理回复
print(res["messages"][2].content)
```

## 5.自定义创建：compiled subagent



```Python
from deepagents import create_deep_agent, CompiledSubAgent
from langchain.agents import create_agent

custom_graph = create_agent(
    model=model,
    tools=[internet_search],
    prompt="You are a great Internet searcher."
)
custom_subagent = CompiledSubAgent(
    name="internet_search",
    description="A specialised agent for gathering information via web searches",
    runnable=custom_graph
)

agent_compiled = create_deep_agent(
    model=model,
    tools=[internet_search],
    subagents=[custom_subagent]
)
```

## 

