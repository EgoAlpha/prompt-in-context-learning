# **第十讲 LangChain  中间件——LLMtool selector 和 Todo list**



**版本：**

python 3.12

pip install langchain==1.0.5

（1.0.5之前Summarization中间件参数会有变动）

## 1.LLMtool selector的创建

创建真实工具

```Python
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
```

创建虚拟工具

```python
@tool
def tool_1(input:str) -> str:
    """
    This is a useless tool, intended solely as an example.
    """
    return "This is a useless tool, intended solely as an example."
@tool
def tool_2(input:str) -> str:
    """
    This is a useless tool, intended solely as an example.
    """
    return "This is a useless tool, intended solely as an example."
@tool
def tool_3(input:str) -> str:
    """
    This is a useless tool, intended solely as an example.
    """
    return "This is a useless tool, intended solely as an example."
@tool
def tool_4(input:str) -> str:
    """
    This is a useless tool, intended solely as an example.
    """
    return "This is a useless tool, intended solely as an example."
```

创建Agent并传入中间件

```python
from langchain.agents import create_agent
from langchain.agents.middleware import LLMToolSelectorMiddleware

agent = create_agent(
    model=model,
    tools=[tool_1, tool_2, tool_3, tool_4,calculate,internet_search],
    middleware=[
        LLMToolSelectorMiddleware(
            model=model,
            max_tools=2,
            always_include=["internet_search"],
        ),
    ],
)
```

## 2.To do list中间件的创建与调用

创建Agent

```Python
from langchain.agents import create_agent
from langchain.agents.middleware import TodoListMiddleware

agent = create_agent(
    model=model,
    tools=[internet_search, calculate],
    middleware=[TodoListMiddleware()],
)
```

以复杂任务调用Agent

```python
res = agent.invoke({"messages":["""你要一步一步的详细规划以下内容再进行回答。
请分析美国加利福尼亚中央谷地的杏仁种植业在未来30年面临的气候变化风险,并估算其经济影响。
具体需要回答,:
“假设当前气候趋势持续,到2050年,加利福尼亚中央谷地杏仁产量可能减少的百分比及其对该州经
济的潜在年度损失是多少美元?这些美元按照2025年11月的汇率能够购买多少比特币?
"""]})


```

观察最终回复与子任务列表

```Python
print(res["message"])
print("\n---------TODO---------------\n")
print(res["todos"])
```



