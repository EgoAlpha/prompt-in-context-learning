# **第十九讲 Langchain V1.0  ——  记忆 Memory**



**版本：**

python 3.12

langchain==1.2.0

deepagents == 0.3.5

## 1.短期记忆与线程

```python
from langchain.agents import create_agent
from langgraph.checkpoint.memory import InMemorySaver  

agent = create_agent(
    model = model,
    checkpointer=InMemorySaver(),  
)

agent.invoke(
    {"messages": [{"role": "user", "content": "你好，我是一个男生，叫李雷"}]},
    {"configurable": {"thread_id": "1"}},  
)

agent.invoke(
    {"messages": [{"role": "user", "content": "你好，我是一个女生，叫韩梅梅"}]},
    {"configurable": {"thread_id": "2"}},  )


res= agent.invoke(
    {"messages": [{"role": "user", "content": "我是谁？？"}]},
    {"configurable": {"thread_id": "1"}},  )
print(res)
```

## 2.自定义状态字段

```python
from typing import Literal
from langchain.agents import AgentState

class CustomAgentState(AgentState):  
    user_name: str
    Gender: Literal["male", "female"]

memory_saver = InMemorySaver()
agent = create_agent(
    model = model,
    checkpointer=memory_saver,  
    state_schema=CustomAgentState,  
)

res = agent.invoke(
    {
        "messages":[
            {"role": "user", "content": "你好!"}
            ],
        "user_name": "李雷",  
        "Gender": "male" ,
    },
    {"configurable": {"thread_id": "1"}})
# 观察自定义字段
print(res["user_name"]+"\n")
print(res["Gender"]+"\n")
```

## 3.工具读取记忆字段



```python
from langchain.tools import tool, ToolRuntime

@tool
def get_user_info(
    runtime: ToolRuntime
) -> str:
    """查看用户信息."""
    user_name = runtime.state["user_name"]
    Gender = runtime.state["Gender"]
    return f"User Name: {user_name}, Gender: {Gender}" 

agent = create_agent(
    model = model,
    tools=[get_user_info],
    checkpointer=memory_saver,  
    state_schema=CustomAgentState,  
)
res = agent.invoke(
    {
    "messages":[{"role": "user", "content": "我是谁？"}],
    },
    {"configurable": {"thread_id": "1"}})
print(res)
```

## 4.长期记忆写入

```bash
from langgraph.store.memory import InMemoryStore

store = InMemoryStore()

namespace_1 = ("六年级", "1班")
namespace_2 = ("五年级", "2班")

store.put(namespace_1, "张三", {
        "exam": "期末考试",
        "scores":{"英语":90,"数学":95},
        "date": "2026-01-15"
    })
store.put(namespace_1, "李四", {
        "exam": "期末考试",
        "scores":{"英语":80,"数学":85},
        "date": "2026-01-15"
    })
store.put(namespace_2, "王五", {
        "exam": "期末考试",
        "scores":{"英语":95,"数学":100},
        "date": "2026-01-15"
    })
```

## 5.观察长期记忆

```bash
li_info = store.get(("六年级", "1班"), "李四")
print(li_info)
wang_info = store.get(("五年级", "2班"), "王五")
print(wang_info)
```
