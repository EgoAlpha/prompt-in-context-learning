# **第九讲 LangChain  中间件——Summarization**



**版本：**

python 3.12

pip install langchain==1.0.5

（1.0.5之前Summarization中间件参数会有变动）

## 1.创建Agent传入中间件

定义模型

```Python
from langchain.chat_models import init_chat_model
model = init_chat_model("openai:gpt-4o-mini",
                        api_key="sk-...",
                        )
```

定义工具

```python
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

创建Agent

```python
from langchain.agents import create_agent
from langchain.agents.middleware import SummarizationMiddleware        

agent = create_agent(
    model=model,
    tools=[internet_search, calculate],
    middleware=[
        SummarizationMiddleware(
            model=model,
            trigger=("messages", 5),
            keep=("messages", 3),
        ),
    ],
)


```

## 2.调用Agent

提前准备消息列表

```Python
from langchain.messages import HumanMessage,AIMessage,ToolMessage

status = {"messages":
[HumanMessage(content='deepseek公司最近有什么最新的资讯?', additional_kwargs={}, response_metadata={}, id='3804b3f2-827c-411a-be33-f3cc84eda168'),
 AIMessage(content='', additional_kwargs={'refusal': None}, response_metadata={'token_usage': {'completion_tokens': 21, 'prompt_tokens': 164, 'total_tokens': 185, 'completion_tokens_details': {'accepted_prediction_tokens': 0, 'audio_tokens': 0, 'reasoning_tokens': 0, 'rejected_prediction_tokens': 0}, 'prompt_tokens_details': {'audio_tokens': 0, 'cached_tokens': 0}}, 'model_provider': 'openai', 'model_name': 'gpt-4o-mini', 'system_fingerprint': 'fp_50906f2aac', 'id': 'chatcmpl-Cid0iHZVVPLVE2vyntv2DHGuZKD4Q', 'service_tier': 'default', 'finish_reason': 'tool_calls', 'logprobs': None}, id='lc_run--0f8cfeb6-ec02-46cc-b24f-abdb5d29e407-0', tool_calls=[{'name': 'internet_search', 'args': {'query': 'deepseek 最新资讯', 'topic': 'news'}, 'id': 'call_CDVy2avyMw2QExcEs1f0xdNc', 'type': 'tool_call'}], usage_metadata={'input_tokens': 164, 'output_tokens': 21, 'total_tokens': 185, 'input_token_details': {'audio': 0, 'cache_read': 0}, 'output_token_details': {'audio': 0, 'reasoning': 0}}),
 ToolMessage(content='{"query": "deepseek 最新资讯", "follow_up_questions": null, "answer": null, "images": [], "results": [{"url": "https://indianexpress.com/article/technology/artificial-intelligence/deepseeks-math-v2-ai-model-self-verify-complex-theorems-10390760/", "title": "DeepSeek’s new Math-V2 AI model can solve and self-verify complex theorems - The Indian Express", "score": 0.72907686, "published_date": "Fri, 28 Nov 2025 06:34:57 GMT", "content": "# DeepSeek’s new Math-V2 AI model can solve and self-verify complex theorems ## DeepSeek-Math-V2 is said to match the performances of OpenAI and Google DeepMind’s models on problems from the International Maths Olympiad 2025. Chinese AI startup DeepSeek on Thursday, November 27, unveiled a new open-weight AI model designed to generate and self-verify mathematical theorems using advanced reasoning skills that the company says were developed specifically for this task. Named DeepSeek-Math-V2, the specialist mathematical reasoning LLM (large language model) is said to possess strong theorem-proving capabilities. In terms of performance, DeepSeek said that Math-V2 achieved gold medal-worthy scores when tested on math problems from the International Mathematical Olympiad (IMO) 2025 and CREST Mathematics Olympiad (CMO) 2024.", "raw_content": null}, {"url": "https://global.chinadaily.com.cn/a/202511/28/WS69295341a310d6866eb2bf02.html", "title": "DeepSeek AI mathematical reasoning model pioneering self-verifying reasoning - China Daily - Global Edition", "score": 0.61168414, "published_date": "Fri, 28 Nov 2025 00:00:00 GMT", "content": "* China Edition * CHINA * CHINA + China Daily PDF + China Daily E-paper # DeepSeek AI mathematical reasoning model pioneering self-verifying reasoning HANGZHOU -- Chinese AI firm DeepSeek has launched DeepSeekMath-V2, a groundbreaking mathematical reasoning model that sets new performance benchmarks and pushes the frontiers of AI-powered problem-solving. Ten photos from across China: Nov 21 - 27 GMD SCO Summit Cities Tianjin The content (including but not limited to text, photo, multimedia information, etc) published in this site belongs to China Daily Information Co (CDIC). China Edition * CHINA + China Daily PDF The content (including but not limited to text, photo, multimedia information, etc) published in this site belongs to China Daily Information Co (CDIC). About China Daily", "raw_content": null}, {"url": "https://ts2.tech/en/nvidia-stock-after-the-bell-nvda-near-180-as-2-billion-synopsys-stake-hpe-deal-and-ai-bubble-fears-collide-december-1-2025/", "title": "Nvidia Stock After the Bell: NVDA Near $180 as $2 Billion Synopsys Stake, HPE Deal and AI Bubble Fears Collide – December 1, 2025 - ts2.tech", "score": 0.36724812, "published_date": "Mon, 01 Dec 2025 21:29:54 GMT", "content": "# Nvidia Stock After the Bell: NVDA Near $180 as $2 Billion Synopsys Stake, HPE Deal and AI Bubble Fears Collide – December 1, 2025 Below is a detailed after‑the‑bell wrap‑up of\xa0**today’s Nvidia stock move, the latest forecasts and the key arguments from both bulls and bears**\xa0as of\xa0**December 1, 2025, 10 p.m. EST**. For now, the market’s verdict is cautious optimism:\xa0**Nvidia is holding near $180**, comfortably below its highs but far above where it started the year, while investors digest whether today’s deals will translate into\xa0**sustainable, high‑quality growth**\xa0— or simply inflate the debate around the most important stock in AI. Nvidia Buys $2B of Synopsys Stock, DeepSeek Debuts New AI Models", "raw_content": null}, {"url": "https://www.reuters.com/business/world-at-work/chinas-baidu-starts-layoffs-after-reporting-third-quarter-loss-sources-2025-11-28/", "title": "China\'s Baidu starts layoffs after reporting third-quarter loss - sources - Reuters", "score": 0.36006194, "published_date": "Fri, 28 Nov 2025 07:15:00 GMT", "content": "# China\'s Baidu starts layoffs after reporting third-quarter loss - sources BEIJING/SHANGHAI, Nov 28 (Reuters) - China\'s Baidu (9888.HK), opens new tab started layoffs this week that will hit multiple business units, six sources briefed on the matter said, as the company struggles with intensifying competition in artificial intelligence and declining advertising revenue. Although Baidu was the first major Chinese tech firm to roll out a ChatGPT-style service in 2023, it has struggled to maintain an early lead against competitors including Alibaba (9988.HK), opens new tab and AI start-up DeepSeek. Baidu\'s Ernie large language model is trailing offerings from rivals including Alibaba and DeepSeek after multiple strategy shifts, including a move to open source it earlier this year. * World at WorkcategoryChina\'s Baidu starts layoffs after reporting third-quarter loss - sources", "raw_content": null}, {"url": "https://www.startupecosystem.ca/news/chinas-tech-giants-take-ai-model-training-offshore-to-tap-nvidia-chips/", "title": "China’s Tech Giants Take AI Model Training Offshore to Tap Nvidia Chips - Startup Ecosystem Canada", "score": 0.35824135, "published_date": "Thu, 27 Nov 2025 06:07:50 GMT", "content": "## China’s Tech Giants Take AI Model Training Offshore to Tap Nvidia Chips * Canada startup news acquisition AI AI development AI infrastructure AI innovation AI integration AI investment AI models AI technology Anthropic Apple Artificial Intelligence Autonomous vehicles Canada founder news Canada startup news ChatGPT cryptocurrency Cybersecurity DeepSeek Electric Vehicles Elon Musk entrepreneurship fintech Funding round Generative AI Global founder news Global startup news healthcare innovation Innovation investment IPO Meta Microsoft Nvidia Ontario startup news OpenAI Sam Altman Seed funding Series A funding Startup growth TechCrunch Disrupt Tech innovation Tesla Toronto startup news venture capital 5 months ago Global Startupfest 2025 Awards Over $1 Million in Prizes to Diverse Startups 5 months ago Global TechCrunch All Stage Summit Offers Discounted Rates for Startups and Founders", "raw_content": null}], "response_time": 0.4, "request_id": "1b4e0fba-2245-4c1f-89ca-dce564fd40a4"}', name='internet_search', id='358baeca-7567-4ff1-b7f3-7a8c9f1ee886', tool_call_id='call_CDVy2avyMw2QExcEs1f0xdNc'),
 AIMessage(content='最近,DeepSeek 公司推出了其最新的数学推理模型 DeepSeek-Math-V2。这个模型可以生成并自我验证复杂的数学定理，其推理能力被专门开发以应对这一任务。DeepSeek 声称，Math-V2 在 2025 年国际数学奥林匹克（IMO）和 2024 年 CREST 数学奥林匹克的测试中表现优异，达到了金牌水平。\n\n以下是一些相关的资讯链接：\n\n1. [DeepSeek的数学V2 AI模型可以解决和自我验证复杂定理 - The Indian Express](https://indianexpress.com/article/technology/artificial-intelligence/deepseeks-math-v2-ai-model-self-verify-complex-theorems-10390760/)\n   - 发布时间：2025年11月28日\n\n2. [DeepSeek AI数学推理模型开创自我验证推理 - China Daily](https://global.chinadaily.com.cn/a/202511/28/WS69295341a310d6866eb2bf02.html)\n   - 发布时间：2025年11月28日\n\n这些信息表明，DeepSeek 在数学推理领域取得了显著进展，可能会在人工智能技术中引发更多关注。', additional_kwargs={'refusal': None}, response_metadata={'token_usage': {'completion_tokens': 272, 'prompt_tokens': 1657, 'total_tokens': 1929, 'completion_tokens_details': {'accepted_prediction_tokens': 0, 'audio_tokens': 0, 'reasoning_tokens': 0, 'rejected_prediction_tokens': 0}, 'prompt_tokens_details': {'audio_tokens': 0, 'cached_tokens': 0}}, 'model_provider': 'openai', 'model_name': 'gpt-4o-mini', 'system_fingerprint': 'fp_50906f2aac', 'id': 'chatcmpl-Cid0lkGkGMPYqQSaSFGfxBj2O6Isg', 'service_tier': 'default', 'finish_reason': 'stop', 'logprobs': None}, id='lc_run--b4804d4c-2865-46cb-befe-1712e3d2e09b-0', usage_metadata={'input_tokens': 1657, 'output_tokens': 272, 'total_tokens': 1929, 'input_token_details': {'audio': 0, 'cache_read': 0}, 'output_token_details': {'audio': 0, 'reasoning': 0}})]}
```

加入询问，调用Agent

```python
status["messages"].append(
    HumanMessage("deepseek的新模型有哪些特点与突破?")
    )
    
result = agent.invoke(status)
print(result)
```

## 3.多种配置方法



```Python
from langchain.agents import create_agent
from langchain.agents.middleware import SummarizationMiddleware



agent2 = create_agent(
    model=model,
    tools=[internet_search, calculate],
    middleware=[
        SummarizationMiddleware(
            model="gpt-4o-mini",
            trigger=("tokens", 4000),
            keep=("tokens", 2000),
        ),
    ],
)

agent3 = create_agent(
    model=model,
    tools=[internet_search, calculate],
    middleware=[
        SummarizationMiddleware(
            model="gpt-4o-mini",
            trigger=("fraction", 0.8),
            keep=("fraction", 0.3),
        ),
    ],
)


# 混合策略
agent4 = create_agent(
    model=model,
    tools=[internet_search, calculate],
    middleware=[
        SummarizationMiddleware(
            model="gpt-4o-mini",
            trigger=[
                ("tokens", 5000), ("messages", 3),
            ],
            keep=("messages", 20),
        ),
    ],
)


```



