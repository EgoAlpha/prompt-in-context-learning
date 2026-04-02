# **第二十三讲  MCP**



**版本：**

python 3.12

langchain==1.2.1

langchain-mcp-adapters == 0.2.2

## 1. UV安装

```powershell
# 安装
pip install uv
# 验证
uv --version
```

## 2.项目创建与依赖项配置

```powershell
# 创建一个新的文件夹作为项目目录
uv init my_mcp_server
cd my_mcp_server
# 添加依赖
uv add "fastmcp"
```

## 3. math_server.py

```python
from fastmcp import FastMCP

mcp = FastMCP("Math")

@mcp.tool()
def add(a: int, b: int) -> int:
    """Add two numbers"""
    return a + b

@mcp.tool()
def multiply(a: int, b: int) -> int:
    """Multiply two numbers"""
    return a * b

if __name__ == "__main__":
    mcp.run(transport="stdio")
```

## 4.测试MCP服务

```bash
uv run python math_server.py
```

## 5.在client.py运行环境安装

```bash
pip install langchain-mcp-adapters
```

## 6.client.py文件（STDIO）

```python
import asyncio
from langchain_mcp_adapters.client import MultiServerMCPClient
from langchain.agents import create_agent
import os
from langchain_deepseek import ChatDeepSeek
from dotenv import load_dotenv

# 加载 .env 文件
dotenv_path = '.env'
load_dotenv(dotenv_path)

# 从环境变量读取配置
DEEPSEEK_API_KEY = os.getenv('DEEPSEEK_API_KEY')

model = ChatDeepSeek(
    model="deepseek-chat",
    api_key=DEEPSEEK_API_KEY,
    temperature=0.7,
)

async def main():
    client = MultiServerMCPClient(
        {"math": {
                "transport": "stdio",
                "command": "uv",
                "args": [
            "--directory",
            r"E:\MCP\my_mcp_server",
            "run",
            "math_server.py"
        ]
        }})

    tools = await client.get_tools()
    agent = create_agent(
        model,
        tools
    )
    response = await agent.ainvoke(
        {"messages": [{"role": "user", "content": "144乘455是多少？？"}]})
    print(response)

if __name__ == "__main__":
    asyncio.run(main())
```

## 7.Client.py文件（Http）

```bash
import asyncio
from langchain_mcp_adapters.client import MultiServerMCPClient
from langchain.agents import create_agent
import os
from langchain_deepseek import ChatDeepSeek
from dotenv import load_dotenv

# 加载 .env 文件
dotenv_path = '.env'
load_dotenv(dotenv_path)

# 从环境变量读取配置
DEEPSEEK_API_KEY = os.getenv('DEEPSEEK_API_KEY')


model = ChatDeepSeek(
    model="deepseek-chat",
    api_key=DEEPSEEK_API_KEY,
    temperature=0.7,
)


async def main():
    client = MultiServerMCPClient(
        {
            "github": {
                "transport": "http",
                "url": "https://api.githubcopilot.com/mcp/",# 填写自己的Github token
                "headers": {
                    "Authorization": "ghp_........",
                }}})

    tools = await client.get_tools()
    agent = create_agent(model, tools)
    response = await agent.ainvoke({"messages": "你好！"})
    print(response)

if __name__ == "__main__":
    asyncio.run(main())




```

