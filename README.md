<div align="center">


<img src="./figures/Prompt-EgoAlpha_white.svg" width="600px">

 <div align="center">

 [![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=30&duration=2500&pause=500&color=8D589A&background=FCFCFF00&center=true&vCenter=true&width=500&lines=Hello!+Human%2C+Are+You+Ready%3F;Welcome+to+my+world!)]()
 
 </div>

**An Open-Source Engineering Guide for Prompt-in-context-learning from EgoAlpha Lab.**

<img width="200%" src="./figures/hr.gif" />

<!-- <h3 align="center">

    <p>Resources for prompt learning and engineering; Mastery of LLMs like ChatGPT, GPT3, FlanT5, etc.</p>

</h3> -->

<!-- <h4 align="center">
    <p>
        <a href="./README.md">English</a> |
        <a href="./chatgptprompt_zh.md">简体中文</a>
    <p>
</h4> -->

<p align="center">

  <a href="#📜-papers">📝 Papers</a> |
  <a href="./Playground.md">⚡️  Playground</a> |
  <a href="./PromptEngineering.md">🛠 Prompt Engineering</a> |
  <a href="./chatgptprompt.md">🌍 ChatGPT Prompt</a> ｜
  <a href="./langchain_guide/LangChainTutorial.ipynb">⛳ LLMs Usage Guide</a> 

</p>

</div>

<div align="center">

<!-- ![Build](https://img.shields.io/appveyor/build/gruntjs/grunt) -->

![version](https://img.shields.io/badge/version-v3.0.0-green)
![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)

<!-- ![license](https://img.shields.io/bower/l/bootstrap?style=plastic) -->

</div>

> **⭐️ Shining ⭐️:** This is fresh, daily-updated resources for in-context learning and prompt engineering. As Artificial General Intelligence (AGI) is approaching, let’s take action and become a super learner so as to position ourselves at the forefront of this exciting era and strive for personal and professional greatness.

The resources include:

*🎉[Papers](#📜-papers)🎉*:  The latest papers about *In-Context Learning*, *Prompt Engineering*, *Agent*, and *Foundation Models*. 

*🎉[Playground](./Playground.md)🎉*:  Large language models（LLMs）that enable prompt experimentation. 

*🎉[Prompt Engineering](./PromptEngineering.md)🎉*: Prompt techniques for leveraging large language models. 

*🎉[ChatGPT Prompt](./chatgptprompt.md)🎉*: Prompt examples that can be applied in our work and daily lives. 

*🎉[LLMs Usage Guide](./chatgptprompt.md)🎉*: The method for quickly getting started with large language models by using LangChain.

In the future, there will likely be two types of people on Earth (perhaps even on Mars, but that's a question for Musk): 
- Those who enhance their abilities through the use of AIGC; 
- Those whose jobs are replaced by AI automation.

```

💎EgoAlpha: Hello! human👤, are you ready?

```  

<img width="200%" src="./figures/hr.gif" />

# Table of Contents
- [📢 News](#-news)
- [📜 Papers](#-papers)
  - [Survey](#survey)
  - [Prompt Engineering](#prompt-engineering)
    - [Prompt Design](#prompt-design)
    - [Chain of Thought](#chain-of-thought)
    - [In-context Learning](#in-context-learning)
    - [Retrieval Augmented Generation](#retrieval-augmented-generation)
    - [Evaluation \& Reliability](#evaluation--reliability)
  - [Agent](#agent)
  - [Multimodal Prompt](#multimodal-prompt)
  - [Prompt Application](#prompt-application)
  - [Foundation Models](#foundation-models)
- [👨‍💻 LLM Usage](#-llm-usage)
- [✉️ Contact](#️-contact)
- [🙏 Acknowledgements](#-acknowledgements)

<img width="200%" src="./figures/hr.gif" />

# 📢 News
<!-- 🔥🔥🔥 -->
☄️ **EgoAlpha releases the TrustGPT focuses on reasoning. Trust the GPT with the strongest reasoning abilities for authentic and reliable answers. You can click [here](https://trustgpt.co) or visit the [Playgrounds](./Playground.md) directly to experience it。**

- **[2024.12.26]**
  - 🔥🔥🔥Big Event in this week:
    - [The OpenAI launch event concluded successfully: o3 dominated the ARC-AGI test; how far are we from AGI?
](https://www.wsj.com/tech/ai/openai-gpt5-orion-delays-639e7693?st=ng5hBi)
    - [NeurIPS Showdown: Fei-Fei Li discusses visual intelligence in a 180-page presentation, Kai-Ming He talks about AI fatalism, and Bengio engages in a debate with OpenAI employees.
](https://spectrum.ieee.org/fei-fei-li-world-labs)
    - [Ilya declares: the era of pre-training is coming to an end.
](https://x.com/vincentweisser/status/1867719020444889118)
    - [The list of 2025 IEEE Fellows has been announced.
](https://www.ieee.org/content/dam/ieee-org/ieee/web/org/about/fellows/fellow-committee/2025-fellows-class-announcement.pdf)
  - Paper List Recently:
    - 【Survery】
      - Paper: [Prompt Compression for Large Language Models: A Survey](https://arxiv.org/abs/2410.12388)
      - Paper: [Towards Graph Prompt Learning: A Survey and Beyond](https://arxiv.org/abs/2408.14520)
    - 【ICL】
      - Paper: [The Power of Adaptation: Boosting In-Context Learning through Adaptive Prompting](https://arxiv.org/abs/2412.17891)
      - Paper: [Revisiting In-Context Learning with Long Context Language Models](https://arxiv.org/abs/2412.16926)
    - 【Foundation Models】
      - Paper: [Byte Latent Transformer: Patches Scale Better Than Tokens ](https://arxiv.org/abs/2412.09871)【From Meta】
      - Paper: [Automatic Database Configuration Debugging using Retrieval-Augmented Language Models](https://arxiv.org/abs/2412.07548)
    - 【RAG】
      - Paper: [GeAR: Graph-enhanced Agent for Retrieval-augmented Generation](https://arxiv.org/abs/2412.18431)
      - Paper: [A Reality Check on Context Utilisation for Retrieval-Augmented Generation](https://arxiv.org/abs/2412.17031)
      - Paper: [Towards More Robust Retrieval-Augmented Generation: Evaluating RAG Under Adversarial Poisoning Attacks](https://arxiv.org/abs/2412.16708)
    - 【Chain-of-thought】
      - Paper: [Enhancing Multi-Robot Semantic Navigation Through Multimodal Chain-of-Thought Score Collaboration](https://arxiv.org/abs/2412.18292)
      - Paper: [Knowledge Editing through Chain-of-Thought](https://arxiv.org/abs/2412.17727)
      - Paper: [DRT-o1: Optimized Deep Reasoning Translation via Long Chain-of-Thought](https://arxiv.org/abs/2412.17498)
    - 【Multimodal Prompts】
      - Paper: [MetaMorph: Multimodal Understanding and Generation via Instruction Tuning](https://arxiv.org/pdf/2412.14164v1)【From Feifei Li】
      - Paper: [HyperSeg: Towards Universal Visual Segmentation with Large Language Model](https://arxiv.org/abs/2411.17606)
      - Paper: [STIV: Scalable Text and Image Conditioned Video Generation](https://arxiv.org/abs/2412.07730)【APPLE-version Sora】

- **[2024.12.18]**
  - 🔥🔥🔥[Veo2&Imagen3: The "Google version" of Sora launched late at night, heralding the arrival of the 4K video generation era.](https://labs.google/fx/zh/tools/video-fx)
  - 【Survery】
    - Paper: [Towards Controllable Speech Synthesis in the Era of Large Language Models: A Survey](https://arxiv.org/abs/2412.06602)
    - Paper: [Steps are all you need: Rethinking STEM Education with Prompt Engineering](https://arxiv.org/abs/2412.05023)
    - Paper: [Survey of different Large Language Model Architectures: Trends, Benchmarks, and Challenges](https://arxiv.org/abs/2412.03220)
  - 【ICL】
    - Paper: [Unlocking LLMs: Addressing Scarce Data and Bias Challenges in Mental Health](https://arxiv.org/abs/2412.12981)
    - Paper: [Jailbreaking? One Step Is Enough!](https://arxiv.org/abs/2412.12621)
  - 【Agent】
    - Paper: [Proposer-Agent-Evaluator(PAE): Autonomous Skill Discovery For Foundation Model Internet Agents](https://arxiv.org/abs/2412.13194)
    - Paper: [SafeAgentBench: A Benchmark for Safe Task Planning of Embodied LLM Agents](https://arxiv.org/abs/2412.13178)
    - Paper: [Bayesian Persuasion with Externalities: Exploiting Agent Types](https://arxiv.org/abs/2412.12859)
  - 【RAG】
    - Paper: [C-FedRAG: A Confidential Federated Retrieval-Augmented Generation System](https://arxiv.org/abs/2412.13163)
    - Paper: [AIR-Bench: Automated Heterogeneous Information Retrieval Benchmark](https://arxiv.org/abs/2412.13102)
    - Paper: [OmniEval: An Omnidirectional and Automatic RAG Evaluation Benchmark in Financial Domain](https://arxiv.org/abs/2412.13018)
  - 【Chain-of-thought】
    - Paper: [CoMT: A Novel Benchmark for Chain of Multi-modal Thought on Large Vision-Language Models](https://arxiv.org/abs/2412.12932)
    - Paper: [Emma-X: An Embodied Multimodal Action Model with Grounded Chain of Thought and Look-ahead Spatial Reasoning](https://arxiv.org/abs/2412.11974)  

- **[2024.12.17]**
  - 🔥🔥🔥[ChatGPT Search, globally free! Her interactive voice search enables real-time querying, effectively challenging Google with simultaneous conversation and search.](https://x.com/OpenAI/status/1868715324885156177)

- **[2024.12.16]**
  - Paper: [Beyond Graph Convolution: Multimodal Recommendation with Topology-aware MLPs](https://arxiv.org/abs/2412.11747)

- **[2024.12.15]**
  - Paper: [C3oT: Generating Shorter Chain-of-Thought without Compromising Effectiveness](https://arxiv.org/abs/2412.11664)

- **[2024.12.14]**
  - Paper: [SAMIC: Segment Anything with In-Context Spatial Prompt Engineering](https://arxiv.org/abs/2412.11998)

- **[2024.12.13]**
  - Paper: [Doe-1: Closed-Loop Autonomous Driving with Large World Model](https://arxiv.org/abs/2412.09627)

- **[2024.12.12]**
  - Paper: [AgentTrek: Agent Trajectory Synthesis via Guiding Replay with Web Tutorials](https://arxiv.org/abs/2412.09605)

- **[2024.11.18]**
  - Paper: [IAA: Inner-Adaptor Architecture Empowers Frozen Large Language Model with Multimodal Capabilities](https://www.arxiv.org/abs/2408.12902)

- **[2024.11.17]**
  - Paper: [DROJ: A Prompt-Driven Attack against Large Language Models](https://arxiv.org/abs/2411.09125)

- **[2024.11.16]**
  - Paper:[On the Surprising Effectiveness of Attention Transfer for Vision Transformers](https://arxiv.org/abs/2411.09702)【NeurIPS2024】

- **[2024.11.15]**
  - Paper:[Squeezed Attention: Accelerating Long Context Length LLM Inference](https://arxiv.org/abs/2411.09688)

- **[2024.11.14]**
  - Paper:[The Limited Impact of Medical Adaptation of Large Language and Vision-Language Models](https://arxiv.org/abs/2411.08870)【EMNLP2024】

- **[2024.11.13]**
  - Paper:[LLMStinger: Jailbreaking LLMs using RL fine-tuned LLMs](https://arxiv.org/abs/2411.08862)【AAAI2025】

- **[2024.11.12]**
  - Paper:[LLMPhy: Complex Physical Reasoning Using Large Language Models and World Models](https://arxiv.org/abs/2411.08027)

- **[2024.11.11]**
  - Paper:[Towards Low-bit Communication for Tensor Parallel LLM Inference](https://arxiv.org/abs/2411.07942)

[👉 Complete history news 👈](./historynews.md)

<img width="200%" src="./figures/hr.gif" />

---

# 📜 Papers

> You can directly click on the title to jump to the corresponding PDF link location

## Survey

<div style="line-height:0.2em;">


<div style="line-height:0.2em;">



[**Motion meets Attention: Video Motion Prompts**](https://arxiv.org/abs/2407.03179) （**2024.07.03**）

![](https://img.shields.io/badge/Citations-0-green)

[**Towards a Personal Health Large Language Model**](https://arxiv.org/abs/2406.06474) （**2024.06.10**）

![](https://img.shields.io/badge/Citations-2-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-6-red)

[**Husky: A Unified, Open-Source Language Agent for Multi-Step Reasoning**](https://arxiv.org/abs/2406.06469) （**2024.06.10**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-14-red)  [![](https://img.shields.io/badge/Github%20Stars-228-blue)](https://github.com/agent-husky/husky-v1)

[**Towards Lifelong Learning of Large Language Models: A Survey**](https://arxiv.org/abs/2406.06391) （**2024.06.10**）

![](https://img.shields.io/badge/Citations-1-green)

[**Towards Semantic Equivalence of Tokenization in Multimodal LLM**](https://arxiv.org/abs/2406.05127) （**2024.06.07**）

![](https://img.shields.io/badge/Citations-4-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-6-red)

[**LLMs Meet Multimodal Generation and Editing: A Survey**](https://doi.org/10.48550/arXiv.2405.19334) （**2024.05.29**）

![](https://img.shields.io/badge/Citations-2-green)  [![](https://img.shields.io/badge/Github%20Stars-206-blue)](https://github.com/yingqinghe/awesome-llms-meet-multimodal-generation)

[**Tool Learning with Large Language Models: A Survey**](https://doi.org/10.48550/arXiv.2405.17935) （**2024.05.28**）

![](https://img.shields.io/badge/Citations-3-green)  [![](https://img.shields.io/badge/Github%20Stars-106-blue)](https://github.com/quchangle1/llm-tool-survey)

[**When LLMs step into the 3D World: A Survey and Meta-Analysis of 3D Tasks via Multi-modal Large Language Models**](https://doi.org/10.48550/arXiv.2405.10255) （**2024.05.16**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-833-blue)](https://github.com/activevisionlab/awesome-llm-3d)

[**Uncertainty Estimation and Quantification for LLMs: A Simple Supervised Approach**](https://doi.org/10.48550/arXiv.2404.15993) （**2024.04.24**）

![](https://img.shields.io/badge/Citations-1-green)

[**A Survey on the Memory Mechanism of Large Language Model based Agents**](https://doi.org/10.48550/arXiv.2404.13501) （**2024.04.21**）

![](https://img.shields.io/badge/Citations-4-green)  [![](https://img.shields.io/badge/Github%20Stars-79-blue)](https://github.com/nuster1128/llm_agent_memory_survey)


</div>

👉[Complete paper list 🔗 for "Survey"](./PaperList/survey.md)👈

## Prompt Engineering

### Prompt Design

<div style="line-height:0.2em;">



[**LLaRA: Supercharging Robot Learning Data for Vision-Language Policy**](https://arxiv.org/abs/2406.20095) （**2024.06.28**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-3-red)  [![](https://img.shields.io/badge/Github%20Stars-77-blue)](https://github.com/lostxine/llara)

[**Dataset Size Recovery from LoRA Weights**](https://arxiv.org/abs/2406.19395) （**2024.06.27**）

![](https://img.shields.io/badge/Citations-0-green)

[**Dual-Phase Accelerated Prompt Optimization**](https://arxiv.org/abs/2406.13443) （**2024.06.19**）

![](https://img.shields.io/badge/Citations-0-green)

[**From RAGs to rich parameters: Probing how language models utilize external knowledge over parametric information for factual queries**](https://arxiv.org/abs/2406.12824) （**2024.06.18**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-8-red)

[**VoCo-LLaMA: Towards Vision Compression with Large Language Models**](https://arxiv.org/abs/2406.12275) （**2024.06.18**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-10-red)  [![](https://img.shields.io/badge/Github%20Stars-58-blue)](https://github.com/Yxxxb/VoCo-LLaMA)

[**LaMDA: Large Model Fine-Tuning via Spectrally Decomposed Low-Dimensional Adaptation**](https://arxiv.org/abs/2406.12832) （**2024.06.18**）

![](https://img.shields.io/badge/Citations-0-green)

[**The Impact of Initialization on LoRA Finetuning Dynamics**](https://arxiv.org/abs/2406.08447) （**2024.06.12**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-3-red)

[**An Empirical Study on Parameter-Efficient Fine-Tuning for MultiModal Large Language Models**](https://arxiv.org/abs/2406.05130) （**2024.06.07**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)

[**Cross-Context Backdoor Attacks against Graph Prompt Learning**](https://doi.org/10.48550/arXiv.2405.17984) （**2024.05.28**）

![](https://img.shields.io/badge/Citations-1-green)

[**Yuan 2.0-M32: Mixture of Experts with Attention Router**](https://doi.org/10.48550/arXiv.2405.17976) （**2024.05.28**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-160-blue)](https://github.com/ieit-yuan/yuan2.0-m32)


</div>

👉[Complete paper list 🔗 for "Prompt Design"](./PaperList/PromptDesignList.md)👈

### Chain of Thought

<div style="line-height:0.2em;">



[**An Empirical Study on Parameter-Efficient Fine-Tuning for MultiModal Large Language Models**](https://arxiv.org/abs/2406.05130) （**2024.06.07**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)

[**Cantor: Inspiring Multimodal Chain-of-Thought of MLLM**](https://doi.org/10.48550/arXiv.2404.16033) （**2024.04.24**）

![](https://img.shields.io/badge/Citations-1-green)

[**nicolay-r at SemEval-2024 Task 3: Using Flan-T5 for Reasoning Emotion Cause in Conversations with Chain-of-Thought on Emotion States**](https://arxiv.org/abs/2404.03361) （**2024.04.04**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-5-blue)](https://github.com/nicolay-r/thor-ecac)

[**Visualization-of-Thought Elicits Spatial Reasoning in Large Language Models**](https://arxiv.org/abs/2404.03622) （**2024.04.04**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-25-red)

[**Can Small Language Models Help Large Language Models Reason Better?: LM-Guided Chain-of-Thought**](https://arxiv.org/abs/2404.03414) （**2024.04.04**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-17-red)

[**Visual CoT: Unleashing Chain-of-Thought Reasoning in Multi-Modal Language Models**](https://arxiv.org/abs/2403.16999) （**2024.03.25**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-16-red)  [![](https://img.shields.io/badge/Github%20Stars-63-blue)](https://github.com/deepcs233/visual-cot)

[**A Chain-of-Thought Prompting Approach with LLMs for Evaluating Students' Formative Assessment Responses in Science**](https://arxiv.org/abs/2403.14565) （**2024.03.21**）

![](https://img.shields.io/badge/Citations-0-green)

[**NavCoT: Boosting LLM-Based Vision-and-Language Navigation via Learning Disentangled Reasoning**](https://arxiv.org/abs/2403.07376) （**2024.03.12**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-5-red)  [![](https://img.shields.io/badge/Github%20Stars-18-blue)](https://github.com/expectorlin/navcot)

[**ERA-CoT: Improving Chain-of-Thought through Entity Relationship Analysis**](https://arxiv.org/abs/2403.06932) （**2024.03.11**）

![](https://img.shields.io/badge/Citations-1-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-6-red)  [![](https://img.shields.io/badge/Github%20Stars-27-blue)](https://github.com/oceanntwt/era-cot)

[**Bias-Augmented Consistency Training Reduces Biased Reasoning in Chain-of-Thought**](https://arxiv.org/abs/2403.05518) （**2024.03.08**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Chain of Thought"](./PaperList/ChainofThoughtList.md)👈

### In-context Learning

<div style="line-height:0.2em;">



[**LaMDA: Large Model Fine-Tuning via Spectrally Decomposed Low-Dimensional Adaptation**](https://arxiv.org/abs/2406.12832) （**2024.06.18**）

![](https://img.shields.io/badge/Citations-0-green)

[**The Impact of Initialization on LoRA Finetuning Dynamics**](https://arxiv.org/abs/2406.08447) （**2024.06.12**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-3-red)

[**An Empirical Study on Parameter-Efficient Fine-Tuning for MultiModal Large Language Models**](https://arxiv.org/abs/2406.05130) （**2024.06.07**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)

[**Leveraging Visual Tokens for Extended Text Contexts in Multi-Modal Learning**](https://arxiv.org/abs/2406.02547) （**2024.06.04**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-6-blue)](https://github.com/showlab/VisInContext)

[**Learning to grok: Emergence of in-context learning and skill composition in modular arithmetic tasks**](https://arxiv.org/abs/2406.02550) （**2024.06.04**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-2-red)  [![](https://img.shields.io/badge/Github%20Stars-3-blue)](https://github.com/ablghtianyi/ICL_Modular_Arithmetic)

[**Long Context is Not Long at All: A Prospector of Long-Dependency Data for Large Language Models**](https://doi.org/10.48550/arXiv.2405.17915) （**2024.05.28**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-39-blue)](https://github.com/October2001/ProLong)

[**Efficient Prompt Tuning by Multi-Space Projection and Prompt Fusion**](https://doi.org/10.48550/arXiv.2405.11464) （**2024.05.19**）

![](https://img.shields.io/badge/Citations-0-green)

[**MAML-en-LLM: Model Agnostic Meta-Training of LLMs for Improved In-Context Learning**](https://doi.org/10.48550/arXiv.2405.11446) （**2024.05.19**）

![](https://img.shields.io/badge/Citations-0-green)

[**Improving Diversity of Commonsense Generation by Large Language Models via In-Context Learning**](https://doi.org/10.48550/arXiv.2404.16807) （**2024.04.25**）

![](https://img.shields.io/badge/Citations-1-green)

[**Stronger Random Baselines for In-Context Learning**](https://doi.org/10.48550/arXiv.2404.13020) （**2024.04.19**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-1-blue)](https://github.com/gyauney/max-random-baseline)


</div>

👉[Complete paper list 🔗 for "In-context Learning"](./PaperList/InContextLearningList.md)👈


### Retrieval Augmented Generation

<div style="line-height:0.2em;">



[**Retrieval-Augmented Mixture of LoRA Experts for Uploadable Machine Learning**](https://arxiv.org/abs/2406.16989) （**2024.06.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Enhancing RAG Systems: A Survey of Optimization Strategies for Performance and Scalability**](https://doi.org/10.55041/ijsrem35402) （**2024.06.04**）

![](https://img.shields.io/badge/Citations-0-green)

[**Enhancing Noise Robustness of Retrieval-Augmented Language Models with Adaptive Adversarial Training**](https://doi.org/10.48550/arXiv.2405.20978) （**2024.05.31**）

![](https://img.shields.io/badge/Citations-1-green)

[**Accelerating Inference of Retrieval-Augmented Generation via Sparse Context Selection**](https://doi.org/10.48550/arXiv.2405.16178) （**2024.05.25**）

![](https://img.shields.io/badge/Citations-0-green)

[**DocReLM: Mastering Document Retrieval with Language Model**](https://doi.org/10.48550/arXiv.2405.11461) （**2024.05.19**）

![](https://img.shields.io/badge/Citations-0-green)

[**UniRAG: Universal Retrieval Augmentation for Multi-Modal Large Language Models**](https://doi.org/10.48550/arXiv.2405.10311) （**2024.05.16**）

![](https://img.shields.io/badge/Citations-0-green)

[**ChatHuman: Language-driven 3D Human Understanding with Retrieval-Augmented Tool Reasoning**](https://doi.org/10.48550/arXiv.2405.04533) （**2024.05.07**）

![](https://img.shields.io/badge/Citations-0-green)

[**REASONS: A benchmark for REtrieval and Automated citationS Of scieNtific Sentences using Public and Proprietary LLMs**](https://doi.org/10.48550/arXiv.2405.02228) （**2024.05.03**）

![](https://img.shields.io/badge/Citations-1-green)

[**Superposition Prompting: Improving and Accelerating Retrieval-Augmented Generation**](https://arxiv.org/abs/2404.06910) （**2024.04.10**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-14-red)

[**Untangle the KNOT: Interweaving Conflicting Knowledge and Reasoning Skills in Large Language Models**](https://arxiv.org/abs/2404.03577) （**2024.04.04**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-1-blue)](https://github.com/thu-keg/knot)


</div>

👉[Complete paper list 🔗 for "Retrieval Augmented Generation"](./PaperList/KnowledgeAugmentedPromptList.md)👈


### Evaluation & Reliability

<div style="line-height:0.2em;">



[**CELLO: Causal Evaluation of Large Vision-Language Models**](https://arxiv.org/abs/2406.19131) （**2024.06.27**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-4-blue)](https://github.com/opencausalab/cello)

[**PrExMe! Large Scale Prompt Exploration of Open Source LLMs for Machine Translation and Summarization Evaluation**](https://arxiv.org/abs/2406.18528) （**2024.06.26**）

![](https://img.shields.io/badge/Citations-0-green)

[**Revisiting Referring Expression Comprehension Evaluation in the Era of Large Multimodal Models**](https://arxiv.org/abs/2406.16866) （**2024.06.24**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-5-blue)](https://github.com/jierunchen/ref-l4)

[**OR-Bench: An Over-Refusal Benchmark for Large Language Models**](https://doi.org/10.48550/arXiv.2405.20947) （**2024.05.31**）

![](https://img.shields.io/badge/Citations-0-green)

[**TimeChara: Evaluating Point-in-Time Character Hallucination of Role-Playing Large Language Models**](https://doi.org/10.48550/arXiv.2405.18027) （**2024.05.28**）

![](https://img.shields.io/badge/Citations-0-green)

[**Subtle Biases Need Subtler Measures: Dual Metrics for Evaluating Representative and Affinity Bias in Large Language Models**](https://doi.org/10.48550/arXiv.2405.14555) （**2024.05.23**）

![](https://img.shields.io/badge/Citations-0-green)

[**HW-GPT-Bench: Hardware-Aware Architecture Benchmark for Language Models**](https://doi.org/10.48550/arXiv.2405.10299) （**2024.05.16**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-9-blue)](https://github.com/automl/hw-gpt-bench)

[**Multimodal LLMs Struggle with Basic Visual Network Analysis: a VNA Benchmark**](https://doi.org/10.48550/arXiv.2405.06634) （**2024.05.10**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-1-blue)](https://github.com/evanup/vna_benchmark)

[**Vibe-Eval: A hard evaluation suite for measuring progress of multimodal language models**](https://doi.org/10.48550/arXiv.2405.02287) （**2024.05.03**）

![](https://img.shields.io/badge/Citations-6-green)  [![](https://img.shields.io/badge/Github%20Stars-139-blue)](https://github.com/reka-ai/reka-vibe-eval)

[**Causal Evaluation of Language Models**](https://doi.org/10.48550/arXiv.2405.00622) （**2024.05.01**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-42-blue)](https://github.com/OpenCausaLab/CaLM)


</div>

👉[Complete paper list 🔗 for "Evaluation & Reliability"](./PaperList/EvaluationReliabilityList.md)👈

## Agent

<div style="line-height:0.2em;">



[**Cooperative Multi-Agent Deep Reinforcement Learning Methods for UAV-aided Mobile Edge Computing Networks**](https://arxiv.org/abs/2407.03280) （**2024.07.03**）

![](https://img.shields.io/badge/Citations-0-green)

[**Symbolic Learning Enables Self-Evolving Agents**](https://arxiv.org/abs/2406.18532) （**2024.06.26**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-8-red)  [![](https://img.shields.io/badge/Github%20Stars-4.8k-blue)](https://github.com/aiwaves-cn/agents)

[**Adversarial Attacks on Multimodal Agents**](https://arxiv.org/abs/2406.12814) （**2024.06.18**）

![](https://img.shields.io/badge/Citations-1-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)  [![](https://img.shields.io/badge/Github%20Stars-24-blue)](https://github.com/chenwu98/agent-attack)

[**DigiRL: Training In-The-Wild Device-Control Agents with Autonomous Reinforcement Learning**](https://arxiv.org/abs/2406.11896) （**2024.06.14**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-5-red)

[**Transforming Wearable Data into Health Insights using Large Language Model Agents**](https://arxiv.org/abs/2406.06464) （**2024.06.10**）

![](https://img.shields.io/badge/Citations-1-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-2-red)

[**Neuromorphic dreaming: A pathway to efficient learning in artificial agents**](https://doi.org/10.48550/arXiv.2405.15616) （**2024.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Fine-Tuning Large Vision-Language Models as Decision-Making Agents via Reinforcement Learning**](https://doi.org/10.48550/arXiv.2405.10292) （**2024.05.16**）

![](https://img.shields.io/badge/Citations-3-green)

[**Learning Multi-Agent Communication from Graph Modeling Perspective**](https://doi.org/10.48550/arXiv.2405.08550) （**2024.05.14**）

![](https://img.shields.io/badge/Citations-3-green)  [![](https://img.shields.io/badge/Github%20Stars-7-blue)](https://github.com/charleshsc/CommFormer)

[**Smurfs: Leveraging Multiple Proficiency Agents with Context-Efficiency for Tool Planning**](https://doi.org/10.48550/arXiv.2405.05955) （**2024.05.09**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-10-blue)](https://github.com/freedomintelligence/smurfs)

[**Unveiling Disparities in Web Task Handling Between Human and Web Agent**](https://doi.org/10.48550/arXiv.2405.04497) （**2024.05.07**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Agent"](./PaperList/AgentList.md)👈

## Multimodal Prompt

<div style="line-height:0.2em;">



[**InternLM-XComposer-2.5: A Versatile Large Vision Language Model Supporting Long-Contextual Input and Output**](https://arxiv.org/abs/2407.03320) （**2024.07.03**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-4-red)  [![](https://img.shields.io/badge/Github%20Stars-2.0k-blue)](https://github.com/internlm/internlm-xcomposer)

[**LLaRA: Supercharging Robot Learning Data for Vision-Language Policy**](https://arxiv.org/abs/2406.20095) （**2024.06.28**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-3-red)  [![](https://img.shields.io/badge/Github%20Stars-77-blue)](https://github.com/lostxine/llara)

[**Web2Code: A Large-scale Webpage-to-Code Dataset and Evaluation Framework for Multimodal LLMs**](https://arxiv.org/abs/2406.20098) （**2024.06.28**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-33-blue)](https://github.com/mbzuai-llm/web2code)

[**LLaVolta: Efficient Multi-modal Models via Stage-wise Visual Context Compression**](https://arxiv.org/abs/2406.20092) （**2024.06.28**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-20-blue)](https://github.com/beckschen/llavolta)

[**Cambrian-1: A Fully Open, Vision-Centric Exploration of Multimodal LLMs**](https://arxiv.org/abs/2406.16860) （**2024.06.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-67-red)  [![](https://img.shields.io/badge/Github%20Stars-1.4k-blue)](https://github.com/cambrian-mllm/cambrian)

[**VoCo-LLaMA: Towards Vision Compression with Large Language Models**](https://arxiv.org/abs/2406.12275) （**2024.06.18**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-10-red)  [![](https://img.shields.io/badge/Github%20Stars-58-blue)](https://github.com/Yxxxb/VoCo-LLaMA)

[**Beyond LLaVA-HD: Diving into High-Resolution Large Multimodal Models**](https://arxiv.org/abs/2406.08487) （**2024.06.12**）

![](https://img.shields.io/badge/Citations-1-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-11-red)  [![](https://img.shields.io/badge/Github%20Stars-90-blue)](https://github.com/yfzhang114/slime)

[**An Empirical Study on Parameter-Efficient Fine-Tuning for MultiModal Large Language Models**](https://arxiv.org/abs/2406.05130) （**2024.06.07**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)

[**Leveraging Visual Tokens for Extended Text Contexts in Multi-Modal Learning**](https://arxiv.org/abs/2406.02547) （**2024.06.04**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-6-blue)](https://github.com/showlab/VisInContext)

[**DeCo: Decoupling Token Compression from Semantic Abstraction in Multimodal Large Language Models**](https://doi.org/10.48550/arXiv.2405.20985) （**2024.05.31**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Multimodal Prompt"](./PaperList/multimodalprompt.md)👈

## Prompt Application

<div style="line-height:0.2em;">



[**IncogniText: Privacy-enhancing Conditional Text Anonymization via LLM-based Private Attribute Randomization**](https://arxiv.org/abs/2407.02956) （**2024.07.03**）

![](https://img.shields.io/badge/Citations-0-green)

[**Web2Code: A Large-scale Webpage-to-Code Dataset and Evaluation Framework for Multimodal LLMs**](https://arxiv.org/abs/2406.20098) （**2024.06.28**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-33-blue)](https://github.com/mbzuai-llm/web2code)

[**OMG-LLaVA: Bridging Image-level, Object-level, Pixel-level Reasoning and Understanding**](https://arxiv.org/abs/2406.19389) （**2024.06.27**）

![](https://img.shields.io/badge/Citations-2-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-7-red)  [![](https://img.shields.io/badge/Github%20Stars-934-blue)](https://github.com/lxtgh/omg-seg)

[**Adversarial Search Engine Optimization for Large Language Models**](https://arxiv.org/abs/2406.18382) （**2024.06.26**）

![](https://img.shields.io/badge/Citations-0-green)

[**VideoLLM-online: Online Video Large Language Model for Streaming Video**](https://arxiv.org/abs/2406.11816) （**2024.06.17**）

![](https://img.shields.io/badge/Citations-0-green)

[**Regularizing Hidden States Enables Learning Generalizable Reward Model for LLMs**](https://arxiv.org/abs/2406.10216) （**2024.06.14**）

![](https://img.shields.io/badge/Citations-0-green)

[**Autoregressive Model Beats Diffusion: Llama for Scalable Image Generation**](https://arxiv.org/abs/2406.06525) （**2024.06.10**）

![](https://img.shields.io/badge/Citations-1-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-43-red)  [![](https://img.shields.io/badge/Github%20Stars-957-blue)](https://github.com/foundationvision/llamagen)

[**Language models emulate certain cognitive profiles: An investigation of how predictability measures interact with individual differences**](https://arxiv.org/abs/2406.04988) （**2024.06.07**）

![](https://img.shields.io/badge/Citations-0-green)

[**PaCE: Parsimonious Concept Engineering for Large Language Models**](https://arxiv.org/abs/2406.04331) （**2024.06.06**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)  [![](https://img.shields.io/badge/Github%20Stars-15-blue)](https://github.com/peterljq/parsimonious-concept-engineering)

[**Yuan 2.0-M32: Mixture of Experts with Attention Router**](https://doi.org/10.48550/arXiv.2405.17976) （**2024.05.28**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-160-blue)](https://github.com/ieit-yuan/yuan2.0-m32)


</div>

👉[Complete paper list 🔗 for "Prompt Application"](./PaperList/promptapplication.md)👈

## Foundation Models

<div style="line-height:0.2em;">



[**TheoremLlama: Transforming General-Purpose LLMs into Lean4 Experts**](https://arxiv.org/abs/2407.03203) （**2024.07.03**）

![](https://img.shields.io/badge/Citations-0-green)

[**Pedestrian 3D Shape Understanding for Person Re-Identification via Multi-View Learning**](https://doi.org/10.1109/TCSVT.2024.3358850) （**2024.07.01**）

![](https://img.shields.io/badge/Citations-3-green)

[**Token Erasure as a Footprint of Implicit Vocabulary Items in LLMs**](https://arxiv.org/abs/2406.20086) （**2024.06.28**）

![](https://img.shields.io/badge/Citations-0-green)

[**OMG-LLaVA: Bridging Image-level, Object-level, Pixel-level Reasoning and Understanding**](https://arxiv.org/abs/2406.19389) （**2024.06.27**）

![](https://img.shields.io/badge/Citations-2-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-7-red)  [![](https://img.shields.io/badge/Github%20Stars-934-blue)](https://github.com/lxtgh/omg-seg)

[**Fundamental Problems With Model Editing: How Should Rational Belief Revision Work in LLMs?**](https://arxiv.org/abs/2406.19354) （**2024.06.27**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-2-red)

[**Efficient World Models with Context-Aware Tokenization**](https://arxiv.org/abs/2406.19320) （**2024.06.27**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)  [![](https://img.shields.io/badge/Github%20Stars-49-blue)](https://github.com/vmicheli/delta-iris)

[**The Remarkable Robustness of LLMs: Stages of Inference?**](https://arxiv.org/abs/2406.19384) （**2024.06.27**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-7-red)

[**ResumeAtlas: Revisiting Resume Classification with Large-Scale Datasets and Large Language Models**](https://arxiv.org/abs/2406.18125) （**2024.06.26**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-1-blue)](https://github.com/noran-mohamed/Resume-Classification-Dataset)

[**AITTI: Learning Adaptive Inclusive Token for Text-to-Image Generation**](https://arxiv.org/abs/2406.12805) （**2024.06.18**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-4-red)  [![](https://img.shields.io/badge/Github%20Stars-5-blue)](https://github.com/itsmag11/aitti)

[**Unveiling Encoder-Free Vision-Language Models**](https://arxiv.org/abs/2406.11832) （**2024.06.17**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-6-red)  [![](https://img.shields.io/badge/Github%20Stars-75-blue)](https://github.com/baaivision/eve)


</div>

👉[Complete paper list 🔗 for "Foundation Models"](./PaperList/foundationmodels.md)👈

<!-- ### 📌 Hard Prompt/ Discrete Prompt

<div style="line-height:0.2em;">



[**Winner-Take-All Column Row Sampling for Memory Efficient Adaptation of Language Model**](https://arxiv.org/abs/2305.15265) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-4-blue)](https://github.com/zirui-ray-liu/wtacrs)

[**How to Distill your BERT: An Empirical Study on the Impact of Weight Initialisation and Distillation Objectives**](https://arxiv.org/abs/2305.15032) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-14-red)  [![](https://img.shields.io/badge/Github%20Stars-9-blue)](https://github.com/mainlp/how-to-distill-your-bert)

[**ChatAgri: Exploring Potentials of ChatGPT on Cross-linguistic Agricultural Text Classification**](https://arxiv.org/abs/2305.15024) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-93-red)  [![](https://img.shields.io/badge/Github%20Stars-38-blue)](https://github.com/albert-jin/agricultural_textual_classification_chatgpt)

[**Cheap and Quick: Efficient Vision-Language Instruction Tuning for Large Language Models**](https://arxiv.org/abs/2305.15023) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-63-red)  [![](https://img.shields.io/badge/Github%20Stars-491-blue)](https://github.com/luogen1996/lavin)

[**LLMDet: A Large Language Models Detection Tool**](https://arxiv.org/abs/2305.15004) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-11-red)

[**OverPrompt: Enhancing ChatGPT Capabilities through an Efficient In-Context Learning Approach**](https://arxiv.org/abs/2305.14973) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)

[**Interpretable by Design Visual Question Answering**](https://arxiv.org/abs/2305.14882) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-4-red)

[**In-Context Demonstration Selection with Cross Entropy Difference**](https://arxiv.org/abs/2305.14726) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-10-red)  [![](https://img.shields.io/badge/Github%20Stars-3.4k-blue)](https://github.com/microsoft/lmops)

[**LogicLLM: Exploring Self-supervised Logic-enhanced Training for Large Language Models**](https://arxiv.org/abs/2305.13718) （**2023.05.23**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-14-red)

[**Enhancing Cross-lingual Natural Language Inference by Soft Prompting with Multilingual Verbalizer**](https://arxiv.org/abs/2305.12761) （**2023.05.22**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-12-red)  [![](https://img.shields.io/badge/Github%20Stars-2-blue)](https://github.com/thu-bpm/softmv)


</div>

👉[Complete paper list 🔗 for "Hard Prompt"](./PaperList/HardPromptList.md)👈

### 📌 Soft Prompt/ Continuous Prompt

<div style="line-height:0.2em;">




</div>

👉[Complete paper list 🔗 for "Soft Prompt"](./PaperList/SoftPromptList.md)👈 -->

<!-- ## Prompt for Knowledge Graph

// __PAPER_LIST__:{field:'Prompt Design',size:10,state:'corrected',type:'lite'}

👉[Complete paper list 🔗 for "Prompt for Knowledge Graph"](./PaperList/PromptKnowledgeGraphList.md)👈 --> 

<img width="200%" src="./figures/hr.gif" />

<!-- # 🎓 Citation

If you find our work helps, please star our project and cite our paper. Thanks a lot!

```

综述论文可以放在这个位置

``` -->

<!-- <img width="200%" src="./figures/hr.gif" /> -->

# 👨‍💻 LLM Usage
Large language models (LLMs) are becoming a revolutionary technology that is shaping the development of our era. Developers can create applications that were previously only possible in our imaginations by building LLMs. However, using these LLMs often comes with certain technical barriers, and even at the introductory stage, people may be intimidated by cutting-edge technology: Do you have any questions like the following?

- ❓ *How can LLM be built using programming?* 
- ❓ *How can it be used and deployed in your own programs?* 

💡 If there was a tutorial that could be accessible to all audiences, not just computer science professionals, it would provide detailed and comprehensive guidance to quickly get started and operate in a short amount of time, ultimately achieving the goal of being able to use LLMs flexibly and creatively to build the programs they envision. And now, just for you: the most detailed and comprehensive Langchain beginner's guide, sourced from the official langchain website but with further adjustments to the content, accompanied by the most detailed and annotated code examples, teaching code lines by line and sentence by sentence to all audiences.

**Click 👉[here](./langchain_guide/LangChainTutorial.ipynb)👈 to take a quick tour of getting started with LLM.**

<img width="200%" src="./figures/hr.gif" />

# ✉️ Contact

This repo is maintained by [EgoAlpha Lab](https://github.com/EgoAlpha). Questions and discussions are welcome via `helloegoalpha@gmail.com`.

We are willing to engage in discussions with friends from the academic and industrial communities, and explore the latest developments in prompt engineering and in-context learning together.

<img width="200%" src="./figures/hr.gif" />

# 🙏 Acknowledgements

Thanks to the PhD students from [EgoAlpha Lab](https://github.com/EgoAlpha) and other workers who participated in this repo. We will improve the project in the follow-up period and maintain this community well. We also would like to express our sincere gratitude to the authors of the relevant resources. Your efforts have broadened our horizons and enabled us to perceive a more wonderful world.


<!-- <img width="200%" src="./figures/hr.gif" /> -->

<!-- # 👨‍👩‍👧‍👦 Contributors

## Main Contributors
* [Yu Liu]()
* [Yifei Cao](https://github.com/cyfedu1024)
* [Jizhe Yu]()
* [Yuan Yao]()
* [He Qi]() -->


<!-- ## Guest Contributors
* [No] -->

<!-- <img width="200%" src="./figures/hr.gif" />

# 📔 License

This project is open source and available under the MIT

<div align="center">
<img src="./figures/rocket.png"/>
</div> -->