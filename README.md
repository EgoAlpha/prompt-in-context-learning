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

![version](https://img.shields.io/badge/version-v2.0.0-yellow)
![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)

<!-- ![license](https://img.shields.io/bower/l/bootstrap?style=plastic) -->

</div>

> **⭐️ Shining ⭐️:** This is fresh, daily-updated resources for in-context learning and prompt engineering. As Artificial General Intelligence (AGI) is approaching, let’s take action and become a super learner so as to position ourselves at the forefront of this exciting era and strive for personal and professional greatness.

The resources include:

*🎉[Papers](#📜-papers)🎉*:  The latest papers about in-context learning or prompt engineering. 

*🎉[Playground](./Playground.md)🎉*:  Large language models that enable prompt experimentation. 

*🎉[Prompt Engineering](./PromptEngineering.md)🎉*: Prompt techniques for leveraging large language models. 

*🎉[ChatGPT Prompt](./chatgptprompt.md)🎉*: Prompt examples that can be applied in our work and daily lives. 

*🎉[LLMs Usage Guide](./chatgptprompt.md)🎉*: The method for quickly getting started with large language models by using LangChain.

In the future, there will likely be two types of people on Earth (perhaps even on Mars, but that's a question for Musk): 
- Those who enhance their abilities through the use of AI; 
- Those whose jobs are replaced by AI automation.

```

💎EgoAlpha: Hello! human👤, are you ready?

```  

<img width="200%" src="./figures/hr.gif" />

# Table of Contents
- [Table of Contents](#table-of-contents)
- [📢 News](#-news)
- [📜 Papers](#-papers)
  - [Survey](#survey)
  - [Prompt Engineering](#prompt-engineering)
    - [Prompt Design](#prompt-design)
    - [Automatic Prompt](#automatic-prompt)
    - [Chain of Thought](#chain-of-thought)
    - [Knowledge Augmented Prompt](#knowledge-augmented-prompt)
    - [Evaluation \& Reliability](#evaluation--reliability)
  - [In-context Learning](#in-context-learning)
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

- **[2023.12.3]**
  - Paper: [Scalable and Transferable Black-Box Jailbreaks for Language Models via Persona Modulation](https://arxiv.org/pdf/2311.03348.pdf)

- **[2023.12.2]**
  - [The PyTorch team has accelerated large model inference by a factor of 10, and with less than 1,000 lines of pure native PyTorch code!](https://pytorch.org/blog/accelerating-generative-ai-2/?)

- **[2023.12.1]**
  - Peking University's newest multimodal LLM open source: trained on mixed datasets and directly used for image-video tasks without modification: 【[arXiv](https://arxiv.org/pdf/2311.08046.pdf)/[Demo](https://huggingface.co/spaces/Chat-UniVi/Chat-UniVi)/[GitHub](https://github.com/PKU-YuanGroup/Chat-UniVi)/[HuggingFace](https://huggingface.co/Chat-UniVi)】

- **[2023.11.30]**
  - Paper: [Learning skillful medium-range global weather forecasting](https://www.science.org/doi/10.1126/science.adi2336)

- **[2023.11.29]**
  - 🔥🔥🔥[Text to Video, PIKA1.0 officially released!](https://pika.art/blog)
  - Paper: [MeshGPT: Generating Triangle Meshes with Decoder-Only Transformers](https://arxiv.org/abs/2311.15475)

- **[2023.11.28]**
  - [Break the Sequential Dependency of LLM Inference Using Lookahead Decoding](https://github.com/hao-ai-lab/LookaheadDecoding)

- **[2023.11.27]**
  - 🔥🔥🔥 Paper: [White-Box Transformers via Sparse Rate Reduction: Compression Is All There Is?](https://arxiv.org/abs/2311.13110)

- **[2023.11.26]**
  - [Use vision to make Prompt! Xiangyang Shen demonstrates IDEA Research Institute's new model, no training or fine-tuning, out-of-the-box!](https://trex-counting.github.io/)

- **[2023.11.25]**
  - Paper:[MedAgents: Large Language Models as Collaborators for Zero-shot Medical Reasoning](https://arxiv.org/abs/2311.10537)

- **[2023.11.24]**
  - Paper: [Social Motion Prediction with Cognitive Hierarchies](https://arxiv.org/pdf/2311.04726.pdf)

- **[2023.11.23]**
  - Paper: [3D-GPT: PROCEDURAL 3D MODELING WITH LARGE LANGUAGE MODELS.](https://arxiv.org/abs/2310.12945)

- **[2023.11.22]**
  - Paper: [Holographic codes from hyper invariant tensor networks](https://www.nature.com/articles/s41467-023-42743-z)

- **[2023.11.21]**
  - Paper: [CAMEL: Communicative Agents for “Mind” Exploration of Large Language Model Society](https://ghli.org/camel.pdf)

- **[2023.11.20]**
  - Paper: [Llemma: An Open Language Model For Mathematics](https://arxiv.org/abs/2310.10631)

- **[2023.11.19]**
  - [OpenAI Late Night Change, Sam Altman Kicked Out, Former CTO Temporary Interim CEO](https://openai.com/blog/openai-announces-leadership-transition)
  - Paper: [IN-CONTEXT LEARNING WITH ITERATIVE DEMON- STRATION SELECTION](https://arxiv.org/pdf/2310.09881.pdf)

- **[2023.11.18]**
  - Paper: [EMU VIDEO: Factorizing Text-to-Video Generation by Explicit Image Conditioning](https://emu-video.metademolab.com/assets/emu_video.pdf)

- **[2023.11.17]**
  - [DeepMind's big model on Science: 1-minute prediction of 10 days of weather data, 90% of the indicators beyond the strongest human model](https://www.science.org/doi/10.1126/science.adi2336)
  - Paper: [Towards Verifiable Text Generation with Symbolic References](https://arxiv.org/abs/2311.09188 )


- **[2023.11.16]**
  - [Microsoft's late-night amplification: GPT-4, DALL-E 3, GPTs for free, self-research big model dedicated AI chip](https://www.theverge.com/2023/11/15/23960345/microsoft-cpu-gpu-ai-chips-azure-maia-cobalt-specifications-cloud-infrastructure)
  - [DevOps finally has an exclusive big model, Ant and BYU jointly released](https://github.com/codefuse-ai/CodeFuse-DevOps-Model/tree/main)

- **[2023.11.15]**
  - 🔥🔥🔥Paper: [Chat-UniVi: Unified Visual Representation Empowers Large Language Models with Image and Video Understanding](https://arxiv.org/abs/2311.08046)
  - 🔥🔥🔥Paper: [SpectralGPT: Spectral Foundation Model](https://arxiv.org/pdf/2311.07113v1.pdf)
  - Paper: [CHATMAP : LARGE LANGUAGE MODEL INTERACTION WITH CARTOGRAPHIC DATA](https://arxiv.org/pdf/2310.01429.pdf)
  - Paper: [EviPrompt: A Training-Free Evidential Prompt Generation Method for Segment Anything Model in Medical Images](https://arxiv.org/abs/2311.06400)
  

- **[2023.11.14]**
  - Paper: [Can LLMs Follow Simple Rules?](https://arxiv.org/abs/2311.04235 )

- **[2023.11.13]**
  - Paper: [Holistic Analysis of Hallucination in GPT-4V(ision): Bias and Interference Challenges](https://arxiv.org/abs/2311.03287)

- **[2023.11.12]**
  - Paper: [Ziya2: Data-centric Learning is All LLMs Need](https://arxiv.org/abs/2311.03301)

- **[2023.11.11]**
  - Paper: [PILL:Plug Into LLM with Adapter Expert and Attention Gat](https://arxiv.org/pdf/2311.02126v1.pdf)

- **[2023.11.10]**
  - Paper: [Levels of AGI: Operationalizing Progress on the Path to AGI](https://arxiv.org/abs/2311.02462)
  - Paper: [mPLUG-Owl2: Revolutionizing Multi-modal Large Language Model with Modality Collaboration](https://arxiv.org/abs/2311.04257)

- **[2023.11.9]**
  - Paper: [Pre-training LLMs using human-like development data corpus](https://arxiv.org/abs/2311.04666 )

- **[2023.11.8]**
  - Paper: [TopicGPT: A Prompt-based Topic Modeling Framework](https://arxiv.org/abs/2311.01449)

- **[2023.11.7]**
  - Paper: [MasterKey: Automated Jailbreak Across Multiple Large Language Model Chatbots](https://arxiv.org/abs/2307.08715)

- **[2023.11.6]**
  - 🔥🔥🔥 01.Ai first open source large models, the Yi series of large models: [Yi-34B](https://huggingface.co/01-ai/Yi-34B) and [Yi-6B](https://huggingface.co/01-ai/Yi-6B).
  - 🔥🔥🔥 Elon Musk's xAI products in two consecutive releases: [PromptIDE](https://x.ai/prompt-ide/) & [Grok](https://grok.x.ai)

- **[2023.11.5]**
  - Paper: [GPT-Fathom: Benchmarking Large Language Models to Decipher the Evolutionary Path towards GPT-4 and Beyond](https://arxiv.org/abs/2309.16583)

- **[2023.11.4]**
  - Paper: [RoboGen: Towards Unleashing Infinite Data for Automated Robot Learning via Generative Simulation](https://arxiv.org/abs/2311.01455)

- **[2023.11.3]**
  - Paper: [In-context Learning with Transformer Is Really Equivalent to a Contrastive Learning Pattern](https://arxiv.org/abs/2310.13220)

- **[2023.11.2]**
  - [DeepMind Exposes Next-Generation AlphaFold, Prediction Accuracy Skyrockets by Nearly 10 Percent! The AlphaFold moment for DNA and RNA is here!](https://storage.googleapis.com/deepmind-media/DeepMind.com/Blog/a-glimpse-of-the-next-generation-of-alphafold/alphafold_latest_oct2023.pdf)

- **[2023.11.1]**
    - [NVIDIA releases ChipNeMo, a large model to design semiconductors and accelerate AI design chips](https://blogs.nvidia.com/blog/2023/10/30/llm-semiconductors-chip-nemo/ )
    - Paper: [LILO: Learning Interpretable Libraries by Compressing and Documenting Code](https://arxiv.org/abs/2310.19791 )

- **[2023.10.31]**
    - Paper: [CodeFusion: A Pre-trained Diffusion Model for Code Generation](https://arxiv.org/abs/2310.17680)

- **[2023.10.30]**
    - Paper: [GraphGPT: Graph Instruction Tuning for Large Language Models](https://arxiv.org/abs/2310.13023)

[👉 Complete history news 👈](./historynews.md)

<img width="200%" src="./figures/hr.gif" />

---

# 📜 Papers

> You can directly click on the title to jump to the corresponding PDF link location

## Survey

<div style="line-height:0.2em;">


<div style="line-height:0.2em;">



[**A Survey of Chain of Thought Reasoning: Advances, Frontiers and Future**](https://doi.org/10.48550/arXiv.2309.15402) （**2023.09.27**）

![](https://img.shields.io/badge/Citations-0-green)

[**The Rise and Potential of Large Language Model Based Agents: A Survey**](https://doi.org/10.48550/arXiv.2309.07864) （**2023.09.14**）

![](https://img.shields.io/badge/Citations-3-green)  [![](https://img.shields.io/badge/Github%20Stars-2.8k-blue)](https://github.com/woooodyy/llm-agent-paper-list)

[**Textbooks Are All You Need II: phi-1.5 technical report**](https://doi.org/10.48550/arXiv.2309.05463) （**2023.09.11**）

![](https://img.shields.io/badge/Citations-6-green)

[**Siren's Song in the AI Ocean: A Survey on Hallucination in Large Language Models**](https://doi.org/10.48550/arXiv.2309.01219) （**2023.09.03**）

![](https://img.shields.io/badge/Citations-8-green)  [![](https://img.shields.io/badge/Github%20Stars-399-blue)](https://github.com/hillzhang1999/llm-hallucination-survey)

[**Point-Bind&Point-LLM: Aligning Point Cloud with Multi-modality for 3D Understanding, Generation, and Instruction Following**](https://arxiv.org/abs/2309.00615) （**2023.09.01**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-7-red)  [![](https://img.shields.io/badge/Github%20Stars-110-blue)](https://github.com/ziyuguo99/point-bind_point-llm)

[**Large language models in medicine: the potentials and pitfalls**](https://arxiv.org/abs/2309.00087) （**2023.08.31**）

![](https://img.shields.io/badge/Citations-0-green)

[**Large Graph Models: A Perspective**](https://doi.org/10.48550/arXiv.2308.14522) （**2023.08.28**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-84-blue)](https://github.com/thumnlab/awesome-large-graph-model)

[**A Survey on Large Language Model based Autonomous Agents**](https://doi.org/10.48550/arXiv.2308.11432) （**2023.08.22**）

![](https://img.shields.io/badge/Citations-13-green)  [![](https://img.shields.io/badge/Github%20Stars-1.1k-blue)](https://github.com/paitesanshi/llm-agent-survey)

[**Instruction Tuning for Large Language Models: A Survey**](https://doi.org/10.48550/arXiv.2308.10792) （**2023.08.21**）

![](https://img.shields.io/badge/Citations-7-green)  [![](https://img.shields.io/badge/Github%20Stars-9-blue)](https://github.com/xiaoya-li/instruction-tuning-survey)

[**Scientific discovery in the age of artificial intelligence**](https://doi.org/10.1038/s41586-023-06221-2) （**2023.08.01**）

![](https://img.shields.io/badge/Citations-7-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-141-red)


</div>

👉[Complete paper list 🔗 for "Survey"](./PaperList/survey.md)👈

## Prompt Engineering

### Prompt Design

<div style="line-height:0.2em;">



[**CodeFusion: A Pre-trained Diffusion Model for Code Generation**](https://arxiv.org/abs/2310.17680) （**2023.10.26**）

![](https://img.shields.io/badge/Citations-0-green)

[**Woodpecker: Hallucination Correction for Multimodal Large Language Models**](https://arxiv.org/abs/2310.16045) （**2023.10.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**GraphGPT: Graph Instruction Tuning for Large Language Models**](https://doi.org/10.48550/arXiv.2310.13023) （**2023.10.19**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-98-blue)](https://github.com/HKUDS/GraphGPT)

[**MusicAgent: An AI Agent for Music Understanding and Generation with Large Language Models**](https://doi.org/10.48550/arXiv.2310.11954) （**2023.10.18**）

![](https://img.shields.io/badge/Citations-0-green)

[**OpenAgents: An Open Platform for Language Agents in the Wild**](https://doi.org/10.48550/arXiv.2310.10634) （**2023.10.16**）

![](https://img.shields.io/badge/Citations-0-green)

[**JMedLoRA: Medical Domain Adaptation on Japanese Large Language Models using Instruction-tuning**](https://doi.org/10.48550/arXiv.2310.10083) （**2023.10.16**）

![](https://img.shields.io/badge/Citations-0-green)

[**The Consensus Game: Language Model Generation via Equilibrium Search**](https://arxiv.org/abs/2310.09139) （**2023.10.13**）

![](https://img.shields.io/badge/Citations-0-green)

[**Understanding the Effects of RLHF on LLM Generalisation and Diversity**](https://arxiv.org/abs/2310.06452) （**2023.10.10**）

![](https://img.shields.io/badge/Citations-0-green)

[**SWE-bench: Can Language Models Resolve Real-World GitHub Issues?**](https://arxiv.org/abs/2310.06770) （**2023.10.10**）

![](https://img.shields.io/badge/Citations-0-green)

[**Walking Down the Memory Maze: Beyond Context Limit through Interactive Reading**](https://doi.org/10.48550/arXiv.2310.05029) （**2023.10.08**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Prompt Design"](./PaperList/PromptDesignList.md)👈

### Automatic Prompt 

<div style="line-height:0.2em;">



[**CodeFusion: A Pre-trained Diffusion Model for Code Generation**](https://arxiv.org/abs/2310.17680) （**2023.10.26**）

![](https://img.shields.io/badge/Citations-0-green)

[**GraphGPT: Graph Instruction Tuning for Large Language Models**](https://doi.org/10.48550/arXiv.2310.13023) （**2023.10.19**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-98-blue)](https://github.com/HKUDS/GraphGPT)

[**OpenAgents: An Open Platform for Language Agents in the Wild**](https://doi.org/10.48550/arXiv.2310.10634) （**2023.10.16**）

![](https://img.shields.io/badge/Citations-0-green)

[**MemGPT: Towards LLMs as Operating Systems**](https://arxiv.org/abs/2310.08560) （**2023.10.12**）

![](https://img.shields.io/badge/Citations-0-green)

[**LongLoRA: Efficient Fine-tuning of Long-Context Large Language Models**](https://doi.org/10.48550/arXiv.2309.12307) （**2023.09.21**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-1.2k-blue)](https://github.com/dvlab-research/longlora)

[**AgentBench: Evaluating LLMs as Agents**](https://doi.org/10.48550/arXiv.2308.03688) （**2023.08.07**）

![](https://img.shields.io/badge/Citations-2-green)  [![](https://img.shields.io/badge/Github%20Stars-972-blue)](https://github.com/thudm/agentbench)

[**Transferring Visual Attributes from Natural Language to Verified Image Generation**](https://arxiv.org/abs/2305.15026) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-2-red)

[**Universal Self-adaptive Prompting**](https://arxiv.org/abs/2305.14926) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-2-red)

[**Discrete Prompt Optimization via Constrained Generation for Zero-shot Re-ranker**](https://arxiv.org/abs/2305.13729) （**2023.05.23**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-6-red)  [![](https://img.shields.io/badge/Github%20Stars-1-blue)](https://github.com/zomss/co-prompt)

[**Self-Polish: Enhance Reasoning in Large Language Models via Problem Refinement**](https://arxiv.org/abs/2305.14497) （**2023.05.23**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-3-red)  [![](https://img.shields.io/badge/Github%20Stars-10-blue)](https://github.com/woooodyy/self-polish)


</div>

👉[Complete paper list 🔗 for "Automatic Prompt"](./PaperList/AutomaticPromptList.md)👈

### Chain of Thought

<div style="line-height:0.2em;">



[**CodeFusion: A Pre-trained Diffusion Model for Code Generation**](https://arxiv.org/abs/2310.17680) （**2023.10.26**）

![](https://img.shields.io/badge/Citations-0-green)

[**Large Language Models Cannot Self-Correct Reasoning Yet**](https://doi.org/10.48550/arXiv.2310.01798) （**2023.10.03**）

![](https://img.shields.io/badge/Citations-7-green)

[**A Survey of Chain of Thought Reasoning: Advances, Frontiers and Future**](https://doi.org/10.48550/arXiv.2309.15402) （**2023.09.27**）

![](https://img.shields.io/badge/Citations-0-green)

[**LongLoRA: Efficient Fine-tuning of Long-Context Large Language Models**](https://doi.org/10.48550/arXiv.2309.12307) （**2023.09.21**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-1.2k-blue)](https://github.com/dvlab-research/longlora)

[**Graph of Thoughts: Solving Elaborate Problems with Large Language Models**](https://doi.org/10.48550/arXiv.2308.09687) （**2023.08.18**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-1.1k-blue)](https://github.com/spcl/graph-of-thoughts)

[**Exploring the Intersection of Large Language Models and Agent-Based Modeling via Prompt Engineering**](https://doi.org/10.48550/arXiv.2308.07411) （**2023.08.14**）

![](https://img.shields.io/badge/Citations-0-green)

[**Cumulative Reasoning with Large Language Models**](https://doi.org/10.48550/arXiv.2308.04371) （**2023.08.08**）

![](https://img.shields.io/badge/Citations-3-green)  [![](https://img.shields.io/badge/Github%20Stars-90-blue)](https://github.com/iiis-ai/cumulative-reasoning)

[**AntGPT: Can Large Language Models Help Long-term Action Anticipation from Videos?**](https://doi.org/10.48550/arXiv.2307.16368) （**2023.07.31**）

![](https://img.shields.io/badge/Citations-0-green)

[**Chain-Of-Thought Prompting Under Streaming Batch: A Case Study**](https://doi.org/10.48550/arXiv.2306.00550) （**2023.06.01**）

![](https://img.shields.io/badge/Citations-0-green)

[**Majority Rule: better patching via Self-Consistency**](https://doi.org/10.48550/arXiv.2306.00108) （**2023.05.31**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Chain of Thought"](./PaperList/ChainofThoughtList.md)👈

### Knowledge Augmented Prompt

<div style="line-height:0.2em;">



[**Are Pre-trained Language Models Useful for Model Ensemble in Chinese Grammatical Error Correction?**](https://arxiv.org/abs/2305.15183) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-3-red)  [![](https://img.shields.io/badge/Github%20Stars-5-blue)](https://github.com/jamydon/plm-based-cgec-model-ensemble)

[**Referral Augmentation for Zero-Shot Information Retrieval**](https://arxiv.org/abs/2305.15098) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-2-red)  [![](https://img.shields.io/badge/Github%20Stars-2-blue)](https://github.com/michaelwilliamtang/referral-augment)

[**Decomposing Complex Queries for Tip-of-the-tongue Retrieval**](https://arxiv.org/abs/2305.15053) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)

[**LLMDet: A Large Language Models Detection Tool**](https://arxiv.org/abs/2305.15004) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-4-red)  [![](https://img.shields.io/badge/Github%20Stars-19-blue)](https://github.com/trustedllm/llmdet)

[**OverPrompt: Enhancing ChatGPT Capabilities through an Efficient In-Context Learning Approach**](https://arxiv.org/abs/2305.14973) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-6-red)

[**Frugal Prompting for Dialog Models**](https://arxiv.org/abs/2305.14919) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Bi-Drop: Generalizable Fine-tuning for Pre-trained Language Models via Adaptive Subnetwork Optimization**](https://arxiv.org/abs/2305.14760) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)

[**In-Context Demonstration Selection with Cross Entropy Difference**](https://arxiv.org/abs/2305.14726) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-2-red)

[**A Causal View of Entity Bias in (Large) Language Models**](https://arxiv.org/abs/2305.14695) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-4-red)

[**SelfzCoT: a Self-Prompt Zero-shot CoT from Semantic-level to Code-level for a Better Utilization of LLMs**](https://doi.org/10.48550/arXiv.2305.11461) （**2023.05.19**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Knowledge Augmented Prompt"](./PaperList/KnowledgeAugmentedPromptList.md)👈


### Evaluation & Reliability

<div style="line-height:0.2em;">



[**TouchStone: Evaluating Vision-Language Models by Language Models**](https://doi.org/10.48550/arXiv.2308.16890) （**2023.08.31**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-27-blue)](https://github.com/ofa-sys/touchstone)

[**Shepherd: A Critic for Language Model Generation**](https://doi.org/10.48550/arXiv.2308.04592) （**2023.08.08**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-160-blue)](https://github.com/facebookresearch/shepherd)

[**Self-consistency for open-ended generations**](https://doi.org/10.48550/arXiv.2307.06857) （**2023.07.11**）

![](https://img.shields.io/badge/Citations-1-green)

[**Jailbroken: How Does LLM Safety Training Fail?**](https://doi.org/10.48550/arXiv.2307.02483) （**2023.07.05**）

![](https://img.shields.io/badge/Citations-0-green)

[**Towards Measuring the Representation of Subjective Global Opinions in Language Models**](https://doi.org/10.48550/arXiv.2306.16388) （**2023.06.28**）

![](https://img.shields.io/badge/Citations-0-green)

[**On the Reliability of Watermarks for Large Language Models**](https://doi.org/10.48550/arXiv.2306.04634) （**2023.06.07**）

![](https://img.shields.io/badge/Citations-2-green)

[**SETI: Systematicity Evaluation of Textual Inference**](https://arxiv.org/abs/2305.15045) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**From Words to Wires: Generating Functioning Electronic Devices from Natural Language Descriptions**](https://arxiv.org/abs/2305.14874) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-2-red)  [![](https://img.shields.io/badge/Github%20Stars-4-blue)](https://github.com/cognitiveailab/words2wires)

[**Testing the General Deductive Reasoning Capacity of Large Language Models Using OOD Examples**](https://arxiv.org/abs/2305.15269) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)

[**EvEval: A Comprehensive Evaluation of Event Semantics for Large Language Models**](https://arxiv.org/abs/2305.15268) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-5-red)


</div>

👉[Complete paper list 🔗 for "Evaluation & Reliability"](./PaperList/EvaluationReliabilityList.md)👈

## In-context Learning

<div style="line-height:0.2em;">



[**CodeFusion: A Pre-trained Diffusion Model for Code Generation**](https://arxiv.org/abs/2310.17680) （**2023.10.26**）

![](https://img.shields.io/badge/Citations-0-green)

[**SuperHF: Supervised Iterative Learning from Human Feedback**](https://arxiv.org/abs/2310.16763) （**2023.10.25**）

![](https://img.shields.io/badge/Citations-0-green)

[**Woodpecker: Hallucination Correction for Multimodal Large Language Models**](https://arxiv.org/abs/2310.16045) （**2023.10.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**MemGPT: Towards LLMs as Operating Systems**](https://arxiv.org/abs/2310.08560) （**2023.10.12**）

![](https://img.shields.io/badge/Citations-0-green)

[**LongLoRA: Efficient Fine-tuning of Long-Context Large Language Models**](https://doi.org/10.48550/arXiv.2309.12307) （**2023.09.21**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-1.2k-blue)](https://github.com/dvlab-research/longlora)

[**Adapting Large Language Models via Reading Comprehension**](https://doi.org/10.48550/arXiv.2309.09530) （**2023.09.18**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-2.3k-blue)](https://github.com/microsoft/lmops)

[**Giraffe: Adventures in Expanding Context Lengths in LLMs**](https://doi.org/10.48550/arXiv.2308.10882) （**2023.08.21**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-454-blue)](https://github.com/abacusai/long-context)

[**Prompt Switch: Efficient CLIP Adaptation for Text-Video Retrieval**](https://doi.org/10.48550/arXiv.2308.07648) （**2023.08.15**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-4-blue)](https://github.com/bladewaltz1/promptswitch)

[**Exploring the Intersection of Large Language Models and Agent-Based Modeling via Prompt Engineering**](https://doi.org/10.48550/arXiv.2308.07411) （**2023.08.14**）

![](https://img.shields.io/badge/Citations-0-green)

[**PromptCARE: Prompt Copyright Protection by Watermark Injection and Verification**](https://doi.org/10.48550/arXiv.2308.02816) （**2023.08.05**）

![](https://img.shields.io/badge/Citations-1-green)


</div>

👉[Complete paper list 🔗 for "In-context Learning"](./PaperList/InContextLearningList.md)👈

## Multimodal Prompt

<div style="line-height:0.2em;">



[**BiLL-VTG: Bridging Large Language Models and Lightweight Visual Tools for Video-based Texts Generation**](https://doi.org/10.48550/arXiv.2310.10586) （**2023.10.16**）

![](https://img.shields.io/badge/Citations-0-green)

[**MiniGPT-5: Interleaved Vision-and-Language Generation via Generative Vokens**](https://doi.org/10.48550/arXiv.2310.02239) （**2023.10.03**）

![](https://img.shields.io/badge/Citations-0-green)

[**Kosmos-2.5: A Multimodal Literate Model**](https://doi.org/10.48550/arXiv.2309.11419) （**2023.09.20**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-10-blue)](https://github.com/kyegomez/Kosmos2.5)

[**Investigating the Catastrophic Forgetting in Multimodal Large Language Models**](https://doi.org/10.48550/arXiv.2309.10313) （**2023.09.19**）

![](https://img.shields.io/badge/Citations-0-green)

[**Physically Grounded Vision-Language Models for Robotic Manipulation**](https://arxiv.org/abs/2309.02561) （**2023.09.05**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-7-red)

[**Physically Grounded Vision-Language Models for Robotic Manipulation**](https://doi.org/10.48550/arXiv.2309.02561) （**2023.09.05**）

![](https://img.shields.io/badge/Citations-1-green)

[**Point-Bind&Point-LLM: Aligning Point Cloud with Multi-modality for 3D Understanding, Generation, and Instruction Following**](https://arxiv.org/abs/2309.00615) （**2023.09.01**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-7-red)  [![](https://img.shields.io/badge/Github%20Stars-110-blue)](https://github.com/ziyuguo99/point-bind_point-llm)

[**PE-MED: Prompt Enhancement for Interactive Medical Image Segmentation**](https://doi.org/10.48550/arXiv.2308.13746) （**2023.08.26**）

![](https://img.shields.io/badge/Citations-0-green)

[**SeamlessM4T-Massively Multilingual & Multimodal Machine Translation**](https://doi.org/10.48550/arXiv.2308.11596) （**2023.08.22**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-303-blue)](https://github.com/facebookresearch/fairseq2)

[**VisIT-Bench: A Benchmark for Vision-Language Instruction Following Inspired by Real-World Use**](https://doi.org/10.48550/arXiv.2308.06595) （**2023.08.12**）

![](https://img.shields.io/badge/Citations-1-green)


</div>

👉[Complete paper list 🔗 for "Multimodal Prompt"](./PaperList/multimodalprompt.md)👈

## Prompt Application

<div style="line-height:0.2em;">



[**Narratron: Collaborative Writing and Shadow-playing of Children Stories with Large Language Models**](https://doi.org/10.1145/3586182.3625120) （**2023.10.29**）

![](https://img.shields.io/badge/Citations-0-green)

[**CodeFusion: A Pre-trained Diffusion Model for Code Generation**](https://arxiv.org/abs/2310.17680) （**2023.10.26**）

![](https://img.shields.io/badge/Citations-0-green)

[**GraphGPT: Graph Instruction Tuning for Large Language Models**](https://doi.org/10.48550/arXiv.2310.13023) （**2023.10.19**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-98-blue)](https://github.com/HKUDS/GraphGPT)

[**Creative Robot Tool Use with Large Language Models**](https://doi.org/10.48550/arXiv.2310.13065) （**2023.10.19**）

![](https://img.shields.io/badge/Citations-0-green)

[**MusicAgent: An AI Agent for Music Understanding and Generation with Large Language Models**](https://doi.org/10.48550/arXiv.2310.11954) （**2023.10.18**）

![](https://img.shields.io/badge/Citations-0-green)

[**BiLL-VTG: Bridging Large Language Models and Lightweight Visual Tools for Video-based Texts Generation**](https://doi.org/10.48550/arXiv.2310.10586) （**2023.10.16**）

![](https://img.shields.io/badge/Citations-0-green)

[**JMedLoRA: Medical Domain Adaptation on Japanese Large Language Models using Instruction-tuning**](https://doi.org/10.48550/arXiv.2310.10083) （**2023.10.16**）

![](https://img.shields.io/badge/Citations-0-green)

[**Table-GPT: Table-tuned GPT for Diverse Table Tasks**](https://doi.org/10.48550/arXiv.2310.09263) （**2023.10.13**）

![](https://img.shields.io/badge/Citations-0-green)

[**MemGPT: Towards LLMs as Operating Systems**](https://arxiv.org/abs/2310.08560) （**2023.10.12**）

![](https://img.shields.io/badge/Citations-0-green)

[**Ferret: Refer and Ground Anything Anywhere at Any Granularity**](https://arxiv.org/abs/2310.07704) （**2023.10.11**）

![](https://img.shields.io/badge/Citations-1-green)


</div>

👉[Complete paper list 🔗 for "Prompt Application"](./PaperList/promptapplication.md)👈

## Foundation Models

<div style="line-height:0.2em;">



[**The Foundation Model Transparency Index**](https://arxiv.org/abs/2310.12941) （**2023.10.19**）

![](https://img.shields.io/badge/Citations-0-green)

[**Language Models Represent Space and Time**](https://arxiv.org/abs/2310.02207) （**2023.10.03**）

![](https://img.shields.io/badge/Citations-3-green)

[**Effective Distillation of Table-based Reasoning Ability from LLMs**](https://doi.org/10.48550/arXiv.2309.13182) （**2023.09.22**）

![](https://img.shields.io/badge/Citations-0-green)

[**Q-Transformer: Scalable Offline Reinforcement Learning via Autoregressive Q-Functions**](https://doi.org/10.48550/arXiv.2309.10150) （**2023.09.18**）

![](https://img.shields.io/badge/Citations-1-green)

[**Replacing softmax with ReLU in Vision Transformers**](https://doi.org/10.48550/arXiv.2309.08586) （**2023.09.15**）

![](https://img.shields.io/badge/Citations-1-green)

[**ZGaming: Zero-Latency 3D Cloud Gaming by Image Prediction**](https://doi.org/10.1145/3603269.3604819) （**2023.09.01**）

![](https://img.shields.io/badge/Citations-0-green)

[**Explaining Vision and Language through Graphs of Events in Space and Time**](https://doi.org/10.48550/arXiv.2309.08612) （**2023.08.29**）

![](https://img.shields.io/badge/Citations-0-green)

[**PE-MED: Prompt Enhancement for Interactive Medical Image Segmentation**](https://doi.org/10.48550/arXiv.2308.13746) （**2023.08.26**）

![](https://img.shields.io/badge/Citations-0-green)

[**SkipcrossNets: Adaptive Skip-cross Fusion for Road Detection**](https://doi.org/10.48550/arXiv.2308.12863) （**2023.08.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**SeqGPT: An Out-of-the-box Large Language Model for Open Domain Sequence Understanding**](https://doi.org/10.48550/arXiv.2308.10529) （**2023.08.21**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-66-blue)](https://github.com/alibaba-nlp/seqgpt)


</div>

👉[Complete paper list 🔗 for "Foundation Models"](./PaperList/foundationmodels.md)👈

<!-- ### 📌 Hard Prompt/ Discrete Prompt

<div style="line-height:0.2em;">



[**Winner-Take-All Column Row Sampling for Memory Efficient Adaptation of Language Model**](https://arxiv.org/abs/2305.15265) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**How to Distill your BERT: An Empirical Study on the Impact of Weight Initialisation and Distillation Objectives**](https://arxiv.org/abs/2305.15032) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-8-red)  [![](https://img.shields.io/badge/Github%20Stars-6-blue)](https://github.com/mainlp/how-to-distill-your-bert)

[**ChatAgri: Exploring Potentials of ChatGPT on Cross-linguistic Agricultural Text Classification**](https://arxiv.org/abs/2305.15024) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-15-red)  [![](https://img.shields.io/badge/Github%20Stars-27-blue)](https://github.com/albert-jin/agricultural_textual_classification_chatgpt)

[**Cheap and Quick: Efficient Vision-Language Instruction Tuning for Large Language Models**](https://arxiv.org/abs/2305.15023) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-37-red)  [![](https://img.shields.io/badge/Github%20Stars-328-blue)](https://github.com/luogen1996/lavin)

[**LLMDet: A Large Language Models Detection Tool**](https://arxiv.org/abs/2305.15004) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-4-red)  [![](https://img.shields.io/badge/Github%20Stars-19-blue)](https://github.com/trustedllm/llmdet)

[**OverPrompt: Enhancing ChatGPT Capabilities through an Efficient In-Context Learning Approach**](https://arxiv.org/abs/2305.14973) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-6-red)

[**In-Context Demonstration Selection with Cross Entropy Difference**](https://arxiv.org/abs/2305.14726) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-2-red)

[**LogiCoT: Logical Chain-of-Thought Instruction-Tuning Data Collection with GPT-4**](https://arxiv.org/abs/2305.12147) （**2023.05.20**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-5-red)  [![](https://img.shields.io/badge/Github%20Stars-33-blue)](https://github.com/csitfun/logicot)

[**SelfzCoT: a Self-Prompt Zero-shot CoT from Semantic-level to Code-level for a Better Utilization of LLMs**](https://doi.org/10.48550/arXiv.2305.11461) （**2023.05.19**）

![](https://img.shields.io/badge/Citations-0-green)

[**Do Models Really Learn to Follow Instructions? An Empirical Study of Instruction Tuning**](https://doi.org/10.48550/arXiv.2305.11383) （**2023.05.19**）

![](https://img.shields.io/badge/Citations-0-green)


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