# **第十六讲 LangChain  ——  如何使用Langsmith**



**版本：**

python 3.12

pip install langchain==1.2.0

pip deepagents == 0.3.0

langgraph-cli 版本0.4.11



## 1.LangSmith 环境变量配置



```Python
LANGSMITH_TRACE=true
LANGSMITH_ENDPOINT=https://api.smith.langchain.com
LANGSMITH_API_KEY=lsv2....

```

## 2.创建Agent基于langsmith观察



```Python
from langchain.chat_models import init_chat_model

api_key = os.getenv("OPENAI_API_KEY")  
base_url = os.getenv("OPENAI_BASE_URL")  
# 定义模型
model = init_chat_model("openai:gpt-5-mini",
                        api_key=api_key,
                        base_url=base_url
)
# 定义工具
import os
from typing import Literal
from langchain_core.tools import tool
from tavily import TavilyClient

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

# 定义Agent

from langchain.agents import create_agent
from langchain.agents.middleware import TodoListMiddleware

agent = create_agent(
    name="test_agent",
    model=model,
    tools=[internet_search,
    middleware=[TodoListMiddleware()],
)

res = agent.invoke({"messages":[
    """
    搜索一下2025年deepseek公司全年动态,然后为我生成一份简洁的年度报告。
    """]})
```

## 3.安装langgraph CLI

终端PIP安装

```bash
# Python >= 3.11 is required.
pip install --upgrade "langgraph-cli[inmem]"
pip install langchain langchain-openai
```

## 4.agent.py配置



```Python
from langchain.chat_models import init_chat_model
from langchain.agents import create_agent
from langchain.agents.middleware import TodoListMiddleware
import os
from typing import Literal
from langchain_core.tools import tool
from tavily import TavilyClient

api_key = os.getenv("OPENAI_API_KEY")  
base_url = os.getenv("OPENAI_BASE_URL")  
# 定义模型
model = init_chat_model("openai:gpt-5-mini",
                        api_key=api_key,
                        base_url=base_url
)
tavily_client = TavilyClient(api_key=os.environ["TAVILY_API_KEY"])

#定义工具
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


from deepagents import create_deep_agent
# 定义子代理和deepagent
internet_subagent = {
    "name": "internet-agent",
    "description": "Utilise online tools to search for information on the internet",
    "system_prompt": "You are a great Internet searcher",
    "tools": [internet_search],
    "model": model,  
}
agent_test = create_deep_agent(
    model=model,
    subagents=[internet_subagent]
)
```

## 5.langgraph.json配置

```Python
{
    "dependencies": ["."],
    "graphs": {
      "agent": "./agent.py:agent_test"
    },
    "env": ".env"
  }
```

## 
