# **第十二讲 LangChain  中间件——file system**



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

## 2.基本创建



```Python
from langchain.agents import create_agent
from deepagents.middleware.filesystem import FilesystemMiddleware

agent = create_agent(
    model=model,
    middleware=[
        FilesystemMiddleware(
            backend=None,  
            system_prompt="Write to the filesystem when...",
            custom_tool_descriptions={
                "ls": "Use the ls tool when...",
                "read_file": "Use the read_file tool to..."
            }  
        ),
    ],
)
```

## 3.后端类型：Filesystembackend



```Python
from deepagents.backends import FilesystemBackend
from langchain.messages import HumanMessage

agent_local = create_agent(
    model=model,
    tools=[],
    middleware=[FilesystemMiddleware(
        backend=FilesystemBackend(root_dir=".", virtual_mode=True)
        )]
)
res = agent_local.invoke({"messages": 
[HumanMessage("""调用工具写入一个文件，
文件名为：密码.txt 
内容为：'我们是EgoAlpha'
""")]})
```

## 4.后端类型：StateBackend



```Python
from deepagents.backends import StateBackend
from langchain.messages import HumanMessage

agent_state = create_agent(
    model=model,
    tools=[],
    middleware=[FilesystemMiddleware(
        backend=lambda runtime: StateBackend(runtime)
        )])
res = agent_state.invoke({
    "messages": [
        HumanMessage("""调用工具写入一个文件，
文件名为：密码.txt 
内容为：'我们是EgoAlpha'
"""),
        HumanMessage("""调用工具读取名为密码.txt的文件,
        告诉我里面的内容""")]
})
print("读到内容：", res["messages"][-1].content)
```

## 5.后端类型：StoreBackend



```Python
from langgraph.store.memory import InMemoryStore
from deepagents.backends import StoreBackend
store = InMemoryStore()          # 创建store实例
agent_store1 = create_agent(
    model=model,
    store=store,                
    middleware=[FilesystemMiddleware(backend=lambda runtime: StoreBackend(runtime))]
)
agent_store1.invoke({"messages": [HumanMessage("""调用工具写入一个文件，
文件名为：密码.txt 
内容为：'我们是EgoAlpha'
""")]})

agent_store2 = create_agent(
    model=model,
    store=store,                 # 同一个store实例
    middleware=[FilesystemMiddleware(backend=lambda runtime: StoreBackend(runtime))]
)
res = agent_store2.invoke({"messages": [HumanMessage("""调用工具读取名为密码.txt的文件,
        告诉我里面的内容""")]})
print("新线程读到：", res["messages"][-1].content)  
```

## 6.复合后端CompositeBackend



```Python
from deepagents import create_deep_agent
from deepagents.backends import CompositeBackend, StateBackend, StoreBackend
from langgraph.store.memory import InMemoryStore

composite_backend = lambda runtime: CompositeBackend(
    default=StateBackend(runtime),
    routes={
        ".": StoreBackend(runtime),
    }
)
agent = create_deep_agent(
    backend=composite_backend,
    store=InMemoryStore()  
)
```

