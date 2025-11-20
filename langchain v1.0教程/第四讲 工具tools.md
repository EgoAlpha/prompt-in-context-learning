# **第四讲 LangChain关键组件——工具tool**



**版本：**

python 3.12

pip install langchain==1.0.3

## 1.基本的工具创建与使用

利用@tool装饰器创建工具

```Python
from langchain_core.tools import tool

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

将工具绑定给模型

```python
#自行设置API_key和模型参数
model = init_chat_model("openai:gpt-4.1")

model_with_tool = model.bind_tools([calculate])

response = model_with_tool.invoke("7的6次方是多少？")
print(response)

```

## 2.多种工具的创建

```Python
import csv
import json
from typing import List, Dict

#本地数据检索工具
@tool
def search_csv(query: str, csv_path: str, limit: int = 10) -> str:
    """
    在本地 CSV 文件中按关键词简单搜索，返回前 limit 条匹配记录(JSON 字符串）。
    """
    query_lower = query.lower()
    results: List[Dict[str, str]] = []

    with open(csv_path, "r", encoding="utf-8-sig", newline="") as f:
        reader = csv.DictReader(f)
        for row in reader:
            if any(query_lower in str(value).lower() for value in row.values()):
                results.append(row)
                if len(results) >= limit:
                    break
    return json.dumps(results, ensure_ascii=False, indent=2)
```

```python
#网络搜索工具（Tavily）
from tavily import TavilyClient
@tool
def internet_search(
    query: str,
    max_results: int = 5,
    topic: Literal["general", "news", "finance"] = "general",
    include_raw_content: bool = False,
):
    """
    使用 Tavily 搜索引擎在互联网上搜索信息
    """
    search_docs = tavily_client.search(
        query,
        max_results=max_results,
        include_raw_content=include_raw_content,
        topic=topic,
    )
    return search_docs

```

## 3.工具的属性配置

```Python
from langchain_core.tools import tool

#工具名称和描述的自定义配置
@tool("caculator",description = "执行算数计算，用具解决数学问题")
def caculate(expression:str)->str:
    """执行数学表达式"""
    return str(eval(expression))
```

```python
from pydantic import BaseModel, Field
from typing import Literal
#定义工具入参格式
class WeatherInput(BaseModel):
    """天气查询的输入参数。"""
    location: str = Field(description="城市名称或坐标")
    units: Literal["celsius", "fahrenheit"] = Field(
        default="celsius",
        description="温度单位偏好"
    )

#将入参格式传入工具
@tool(args_schema=WeatherInput)
def get_weather(location: str, units: str = "celsius") -> str:
    """获取当前天气和可选预报。"""
    # 模拟天气数据 - 实际应用中会调用天气API
    temp = 22 if units == "celsius" else 72
    result = f"{location}当前天气: {temp}度{units[0].upper()}"
    
    return result
```



## 4.structuredtool 类的属性与方法

```python
# 属性
name = get_weather.name
description = get_weather.description
get_weather.response_format
#修改response_format
get_weather.response_format = "content_and_artifacts"
    
```

```python
# 方法
internet_search.get_input_schema()
print(internet_search.get_input_schema)

internet_search.get_output_schema()
print(internet_search.get_output_schema)

internet_search.invoke(input = "langchain1.0")
```

