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

- **[2023.1.15]**
  - Paper: [TOFU: A Task of Fictitious Unlearning for LLMs](https://simg.baai.ac.cn/paperfile/ccd571d3-7b4b-4355-975b-6ca81d882f5b.pdf)

- **[2023.1.14]**
  - Technical Report: [DeepSeekMoE: Towards Ultimate Expert Specialization in Mixture-of-Experts Language Models](https://github.com/deepseek-ai/DeepSeek-MoE/blob/main/DeepSeekMoE.pdf)

- **[2023.1.13]**
  - [GPT Store is now online!](https://openai.com/blog/introducing-the-gpt-store)
  - Paper: [MagicVideo-V2: Multi-Stage High-Aesthetic Video Generation](https://arxiv.org/abs/2401.04468)
  

- **[2023.1.12]**
  - Survey Paper: [Large Language Models Empowered Agent-based Modeling and Simulation: A Survey and Perspectives](https://arxiv.org/abs/2312.11970)

- **[2023.1.11]**
  - Paper: [Lyrics: Boosting Fine-grained Language-Vision Alignment and Comprehension via Semantic-aware Visual Objects](https://arxiv.org/abs/2312.05278)

- **[2023.1.10]**
  - Paper: [Incorporating Visual Experts to Resolve the Information Loss in Multimodal Large Language Models](https://arxiv.org/abs/2401.03105v1)

- **[2023.1.9]**
  - Paper: [Chain-of-Table: Evolving Tables in the Reasoning Chain for Table Understanding](https://arxiv.org/abs/2401.04398v1)

- **[2023.1.8]**
  - Paper: [WaveCoder: Widespread And Versatile Enhanced Instruction Tuning with Refined Data Generation](https://arxiv.org/abs/2312.14187)

- **[2023.1.7]**
  - Paper: [LLaMA Pro: Progressive LLaMA with Block Expansion](https://arxiv.org/abs/2401.02415v1)

- **[2023.1.6]**
  - Paper: [Task Oriented Dialogue as a Catalyst for Self-Supervised Automatic Speech Recognition](https://arxiv.org/abs/2401.02417v1)

- **[2023.1.5]**
  - Paper: [Learning to Prompt with Text Only Supervision for Vision-Language Models](https://arxiv.org/abs/2401.02418v1)

- **[2023.1.4]**
  - Paper: [LLM Augmented LLMs: Expanding Capabilities through Composition](https://arxiv.org/abs/2401.02412v1)

- **[2023.1.3]**
  - Paper:[CogAgent: A Visual Language Model for GUI Agents](https://arxiv.org/abs/2312.08914)
  - Paper: [TinyGPT-V: Efficient Multimodal Large Language Model via Small Backbones](https://arxiv.org/abs/2312.16862)

- **[2023.1.2]**
  - Paper:[MobileVLM: A Fast, Strong and Open Vision Language Assistant for Mobile Devices](https://arxiv.org/abs/2312.16886)

- **[2023.1.1]**
  - Paper:[Generative AI for Math: Part I MATHPILE: A Billion-Token-Scale Pretraining Corpus for Math](https://arxiv.org/pdf/2312.17120.pdf)

- **[2023.12.31]**
  - [Hugging Face Year in Review: 2023, The Year of Open Source LLMs](https://huggingface.co/blog/2023-in-llms)

- **[2023.12.30]**
  - Paper: [Unsupervised embedding of trajectories captures the latent structure of scientific migration](https://www.pnas.org/doi/10.1073/pnas.2305414120)

- **[2023.12.29]**
  - KwaiAgents is a series of Agent-related works open-sourced by the KwaiKEG from Kuaishou Technology 【[Paper](https://arxiv.org/abs/2312.04889)/[Github](https://github.com/KwaiKEG/KwaiAgents?tab=readme-ov-file)】

- **[2023.12.28]**
  - Paper: [EmbodiedScan: A Holistic Multi-Modal 3D Perception Suite Towards Embodied AI](https://arxiv.org/pdf/2312.16170v1.pdf)
  - Paper: [Principled Instructions Are All You Need for Questioning LLaMA-1/2, GPT-3.5/4](https://arxiv.org/pdf/2312.16171v1.pdf)

- **[2023.12.27]**
  - Paper: [The Truth is in There: Improving Reasoning in Language Models with Layer-Selective Rank Reduction](https://arxiv.org/pdf/2312.13558v1.pdf)

- **[2023.12.26]**
  - Paper: [LORAMOE: REVOLUTIONIZING MIXTURE OF EXPERTS FOR MAINTAINING WORLD KNOWLEDGE IN LANGUAGE MODEL ALIGNMENT](https://simg.baai.ac.cn/paperfile/96f0cfd7-79c7-4110-88e5-4ea80a7fbc8d.pdf)

- **[2023.12.25]**
  - Survey Paper: [Retrieval-Augmented Generation for Large Language Models: A Survey](https://simg.baai.ac.cn/paperfile/25a43194-c74c-4cd3-b60f-0a1f27f8b8af.pdf)

[👉 Complete history news 👈](./historynews.md)

<img width="200%" src="./figures/hr.gif" />

---

# 📜 Papers

> You can directly click on the title to jump to the corresponding PDF link location

## Survey

<div style="line-height:0.2em;">


<div style="line-height:0.2em;">



[**Retrieval-Augmented Generation for Large Language Models: A Survey**](https://arxiv.org/abs/2312.10997) （**2023.12.18**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-126-blue)](https://github.com/tongji-kgllm/rag-survey)

[**Retrieval-augmented Generation to Improve Math Question-Answering: Trade-offs Between Groundedness and Human Preference**](https://doi.org/10.48550/arXiv.2310.03184) （**2023.10.04**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-5-blue)](https://github.com/digitalharborfoundation/rag-for-math-qa)

[**A Survey of Chain of Thought Reasoning: Advances, Frontiers and Future**](https://doi.org/10.48550/arXiv.2309.15402) （**2023.09.27**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-179-blue)](https://github.com/zchuz/cot-reasoning-survey)

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

![](https://img.shields.io/badge/Citations-1-green)

[**A Survey on Large Language Model based Autonomous Agents**](https://doi.org/10.48550/arXiv.2308.11432) （**2023.08.22**）

![](https://img.shields.io/badge/Citations-13-green)  [![](https://img.shields.io/badge/Github%20Stars-1.7k-blue)](https://github.com/paitesanshi/llm-agent-survey)


</div>

👉[Complete paper list 🔗 for "Survey"](./PaperList/survey.md)👈

## Prompt Engineering

### Prompt Design

<div style="line-height:0.2em;">



[**The Truth is in There: Improving Reasoning in Language Models with Layer-Selective Rank Reduction**](https://arxiv.org/abs/2312.13558) （**2023.12.21**）

![](https://img.shields.io/badge/Citations-0-green)

[**G-LLaVA: Solving Geometric Problem with Multi-Modal Large Language Model**](https://arxiv.org/abs/2312.11370) （**2023.12.18**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-49-blue)](https://github.com/pipilurj/g-llava)

[**A mathematical perspective on Transformers**](https://arxiv.org/abs/2312.10794) （**2023.12.17**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-9-blue)](https://github.com/borjang/2023-transformers-rotf)

[**LoRAMoE: Revolutionizing Mixture of Experts for Maintaining World Knowledge in Language Model Alignment**](https://arxiv.org/abs/2312.09979) （**2023.12.15**）

![](https://img.shields.io/badge/Citations-0-green)

[**LLM360: Towards Fully Transparent Open-Source LLMs**](https://arxiv.org/abs/2312.06550) （**2023.12.11**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-15-red)  [![](https://img.shields.io/badge/Github%20Stars-46-blue)](https://github.com/llm360/analysis360)

[**Control Risk for Potential Misuse of Artificial Intelligence in Science**](https://arxiv.org/abs/2312.06632) （**2023.12.11**）

![](https://img.shields.io/badge/Citations-0-green)

[**WonderJourney: Going from Anywhere to Everywhere**](https://arxiv.org/abs/2312.03884) （**2023.12.06**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-6-red)

[**LLaVA-Grounding: Grounded Visual Chat with Large Multimodal Models**](https://arxiv.org/abs/2312.02949) （**2023.12.05**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-88-blue)](https://github.com/ux-decoder/llava-grounding)

[**An Embodied Generalist Agent in 3D World**](https://doi.org/10.48550/arXiv.2311.12871) （**2023.11.18**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-117-blue)](https://github.com/embodied-generalist/embodied-generalist)

[**MedAgents: Large Language Models as Collaborators for Zero-shot Medical Reasoning**](https://doi.org/10.48550/arXiv.2311.10537) （**2023.11.16**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Prompt Design"](./PaperList/PromptDesignList.md)👈

### Chain of Thought

<div style="line-height:0.2em;">



[**A Logically Consistent Chain-of-Thought Approach for Stance Detection**](https://arxiv.org/abs/2312.16054) （**2023.12.26**）

![](https://img.shields.io/badge/Citations-0-green)

[**Assessing the Impact of Prompting, Persona, and Chain of Thought Methods on ChatGPT's Arithmetic Capabilities**](https://arxiv.org/abs/2312.15006) （**2023.12.22**）

![](https://img.shields.io/badge/Citations-0-green)

[**G-LLaVA: Solving Geometric Problem with Multi-Modal Large Language Model**](https://arxiv.org/abs/2312.11370) （**2023.12.18**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-49-blue)](https://github.com/pipilurj/g-llava)

[**ProCoT: Stimulating Critical Thinking and Writing of Students through Engagement with Large Language Models (LLMs)**](https://arxiv.org/abs/2312.09801) （**2023.12.15**）

![](https://img.shields.io/badge/Citations-0-green)

[**Multi-modal Latent Space Learning for Chain-of-Thought Reasoning in Language Models**](https://arxiv.org/abs/2312.08762) （**2023.12.14**）

![](https://img.shields.io/badge/Citations-0-green)

[**Control Risk for Potential Misuse of Artificial Intelligence in Science**](https://arxiv.org/abs/2312.06632) （**2023.12.11**）

![](https://img.shields.io/badge/Citations-0-green)

[**Chain-of-Thought in Neural Code Generation: From and For Lightweight Language Models**](https://arxiv.org/abs/2312.05562) （**2023.12.09**）

![](https://img.shields.io/badge/Citations-0-green)

[**Latent Skill Discovery for Chain-of-Thought Reasoning**](https://arxiv.org/abs/2312.04684) （**2023.12.07**）

![](https://img.shields.io/badge/Citations-0-green)

[**Computation of the optimal error exponent function for fixed-length lossy source coding in discrete memoryless sources**](https://arxiv.org/abs/2312.03784) （**2023.12.06**）

![](https://img.shields.io/badge/Citations-0-green)

[**WonderJourney: Going from Anywhere to Everywhere**](https://arxiv.org/abs/2312.03884) （**2023.12.06**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-6-red)


</div>

👉[Complete paper list 🔗 for "Chain of Thought"](./PaperList/ChainofThoughtList.md)👈

### In-context Learning

<div style="line-height:0.2em;">



[**G-LLaVA: Solving Geometric Problem with Multi-Modal Large Language Model**](https://arxiv.org/abs/2312.11370) （**2023.12.18**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-49-blue)](https://github.com/pipilurj/g-llava)

[**A mathematical perspective on Transformers**](https://arxiv.org/abs/2312.10794) （**2023.12.17**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-9-blue)](https://github.com/borjang/2023-transformers-rotf)

[**Control Risk for Potential Misuse of Artificial Intelligence in Science**](https://arxiv.org/abs/2312.06632) （**2023.12.11**）

![](https://img.shields.io/badge/Citations-0-green)

[**WonderJourney: Going from Anywhere to Everywhere**](https://arxiv.org/abs/2312.03884) （**2023.12.06**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-6-red)

[**Minimizing Factual Inconsistency and Hallucination in Large Language Models**](https://doi.org/10.48550/arXiv.2311.13878) （**2023.11.23**）

![](https://img.shields.io/badge/Citations-0-green)

[**Igniting Language Intelligence: The Hitchhiker's Guide From Chain-of-Thought Reasoning to Language Agents**](https://doi.org/10.48550/arXiv.2311.11797) （**2023.11.20**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-252-blue)](https://github.com/zoeyyao27/cot-igniting-agent)

[**An Embodied Generalist Agent in 3D World**](https://doi.org/10.48550/arXiv.2311.12871) （**2023.11.18**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-117-blue)](https://github.com/embodied-generalist/embodied-generalist)

[**MedAgents: Large Language Models as Collaborators for Zero-shot Medical Reasoning**](https://doi.org/10.48550/arXiv.2311.10537) （**2023.11.16**）

![](https://img.shields.io/badge/Citations-0-green)

[**Towards Verifiable Text Generation with Symbolic References**](https://doi.org/10.48550/arXiv.2311.09188) （**2023.11.15**）

![](https://img.shields.io/badge/Citations-0-green)

[**Learning skillful medium-range global weather forecasting.**](https://doi.org/10.1126/science.adi2336) （**2023.11.14**）

![](https://img.shields.io/badge/Citations-8-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-360-red)


</div>

👉[Complete paper list 🔗 for "In-context Learning"](./PaperList/InContextLearningList.md)👈


### Retrieval Augmented Generation

<div style="line-height:0.2em;">



[**ARES: An Automated Evaluation Framework for Retrieval-Augmented Generation Systems**](https://doi.org/10.48550/arXiv.2311.09476) （**2023.11.16**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-114-blue)](https://github.com/stanford-futuredata/ares)

[**Self-RAG: Learning to Retrieve, Generate, and Critique through Self-Reflection**](https://doi.org/10.48550/arXiv.2310.11511) （**2023.10.17**）

![](https://img.shields.io/badge/Citations-13-green)

[**Benchmarking Large Language Models in Retrieval-Augmented Generation**](https://doi.org/10.48550/arXiv.2309.01431) （**2023.09.04**）

![](https://img.shields.io/badge/Citations-8-green)

[**Evaluating Correctness and Faithfulness of Instruction-Following Models for Question Answering**](https://doi.org/10.48550/arXiv.2307.16877) （**2023.07.31**）

![](https://img.shields.io/badge/Citations-17-green)  [![](https://img.shields.io/badge/Github%20Stars-56-blue)](https://github.com/mcgill-nlp/instruct-qa)

[**Are Pre-trained Language Models Useful for Model Ensemble in Chinese Grammatical Error Correction?**](https://arxiv.org/abs/2305.15183) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-5-red)  [![](https://img.shields.io/badge/Github%20Stars-8-blue)](https://github.com/jamydon/plm-based-cgec-model-ensemble)

[**Referral Augmentation for Zero-Shot Information Retrieval**](https://arxiv.org/abs/2305.15098) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-3-red)  [![](https://img.shields.io/badge/Github%20Stars-6-blue)](https://github.com/michaelwilliamtang/referral-augment)

[**Decomposing Complex Queries for Tip-of-the-tongue Retrieval**](https://arxiv.org/abs/2305.15053) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)

[**LLMDet: A Large Language Models Detection Tool**](https://arxiv.org/abs/2305.15004) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-7-red)

[**OverPrompt: Enhancing ChatGPT Capabilities through an Efficient In-Context Learning Approach**](https://arxiv.org/abs/2305.14973) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-8-red)

[**Frugal Prompting for Dialog Models**](https://arxiv.org/abs/2305.14919) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Retrieval Augmented Generation"](./PaperList/KnowledgeAugmentedPromptList.md)👈


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

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)  [![](https://img.shields.io/badge/Github%20Stars-4-blue)](https://github.com/cognitiveailab/words2wires)

[**Testing the General Deductive Reasoning Capacity of Large Language Models Using OOD Examples**](https://arxiv.org/abs/2305.15269) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-13-red)  [![](https://img.shields.io/badge/Github%20Stars-77-blue)](https://github.com/asaparov/prontoqa)

[**EvEval: A Comprehensive Evaluation of Event Semantics for Large Language Models**](https://arxiv.org/abs/2305.15268) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-6-red)


</div>

👉[Complete paper list 🔗 for "Evaluation & Reliability"](./PaperList/EvaluationReliabilityList.md)👈

## Agent

<div style="line-height:0.2em;">



[**AppAgent: Multimodal Agents as Smartphone Users**](https://arxiv.org/abs/2312.13771) （**2023.12.21**）

![](https://img.shields.io/badge/Citations-0-green)

[**WonderJourney: Going from Anywhere to Everywhere**](https://arxiv.org/abs/2312.03884) （**2023.12.06**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-6-red)

[**Agent as Cerebrum, Controller as Cerebellum: Implementing an Embodied LMM-based Agent on Drones**](https://doi.org/10.48550/arXiv.2311.15033) （**2023.11.25**）

![](https://img.shields.io/badge/Citations-0-green)

[**GPT-4V in Wonderland: Large Multimodal Models for Zero-Shot Smartphone GUI Navigation**](https://doi.org/10.48550/arXiv.2311.07562) （**2023.11.13**）

![](https://img.shields.io/badge/Citations-3-green)  [![](https://img.shields.io/badge/Github%20Stars-85-blue)](https://github.com/zzxslp/mm-navigator)

[**Lemur: Harmonizing Natural Language and Code for Language Agents**](https://doi.org/10.48550/arXiv.2310.06830) （**2023.10.10**）

![](https://img.shields.io/badge/Citations-12-green)  [![](https://img.shields.io/badge/Github%20Stars-474-blue)](https://github.com/openlemur/lemur)

[**Agents: An Open-source Framework for Autonomous Language Agents**](https://doi.org/10.48550/arXiv.2309.07870) （**2023.09.14**）

![](https://img.shields.io/badge/Citations-16-green)  [![](https://img.shields.io/badge/Github%20Stars-4.1k-blue)](https://github.com/aiwaves-cn/agents)

[**An Appraisal-Based Chain-Of-Emotion Architecture for Affective Language Model Game Agents**](https://doi.org/10.48550/arXiv.2309.05076) （**2023.09.10**）

![](https://img.shields.io/badge/Citations-2-green)

[**Cognitive Architectures for Language Agents**](https://doi.org/10.48550/arXiv.2309.02427) （**2023.09.05**）

![](https://img.shields.io/badge/Citations-20-green)  [![](https://img.shields.io/badge/Github%20Stars-468-blue)](https://github.com/ysymyth/awesome-language-agents)

[**Retroformer: Retrospective Large Language Agents with Policy Gradient Optimization**](https://doi.org/10.48550/arXiv.2308.02151) （**2023.08.04**）

![](https://img.shields.io/badge/Citations-13-green)

[**Math Agents: Computational Infrastructure, Mathematical Embedding, and Genomics**](https://doi.org/10.48550/arXiv.2307.02502) （**2023.07.04**）

![](https://img.shields.io/badge/Citations-2-green)


</div>

👉[Complete paper list 🔗 for "Agent"](./PaperList/AgentList.md)👈

## Multimodal Prompt

<div style="line-height:0.2em;">



[**G-LLaVA: Solving Geometric Problem with Multi-Modal Large Language Model**](https://arxiv.org/abs/2312.11370) （**2023.12.18**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-49-blue)](https://github.com/pipilurj/g-llava)

[**LLaVA-Grounding: Grounded Visual Chat with Large Multimodal Models**](https://arxiv.org/abs/2312.02949) （**2023.12.05**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-88-blue)](https://github.com/ux-decoder/llava-grounding)

[**Sequential Modeling Enables Scalable Learning for Large Vision Models**](https://arxiv.org/abs/2312.00785) （**2023.12.01**）

![](https://img.shields.io/badge/Citations-0-green)

[**LLaMA-VID: An Image is Worth 2 Tokens in Large Language Models**](https://doi.org/10.48550/arXiv.2311.17043) （**2023.11.28**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-349-blue)](https://github.com/dvlab-research/llama-vid)

[**MeshGPT: Generating Triangle Meshes with Decoder-Only Transformers**](https://doi.org/10.48550/arXiv.2311.15475) （**2023.11.27**）

![](https://img.shields.io/badge/Citations-0-green)

[**An Embodied Generalist Agent in 3D World**](https://doi.org/10.48550/arXiv.2311.12871) （**2023.11.18**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-117-blue)](https://github.com/embodied-generalist/embodied-generalist)

[**Emu Video: Factorizing Text-to-Video Generation by Explicit Image Conditioning**](https://doi.org/10.48550/arXiv.2311.10709) （**2023.11.17**）

![](https://img.shields.io/badge/Citations-2-green)

[**MedAgents: Large Language Models as Collaborators for Zero-shot Medical Reasoning**](https://doi.org/10.48550/arXiv.2311.10537) （**2023.11.16**）

![](https://img.shields.io/badge/Citations-0-green)

[**Chat-UniVi: Unified Visual Representation Empowers Large Language Models with Image and Video Understanding**](https://doi.org/10.48550/arXiv.2311.08046) （**2023.11.14**）

![](https://img.shields.io/badge/Citations-3-green)

[**EviPrompt: A Training-Free Evidential Prompt Generation Method for Segment Anything Model in Medical Images**](https://doi.org/10.48550/arXiv.2311.06400) （**2023.11.10**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Multimodal Prompt"](./PaperList/multimodalprompt.md)👈

## Prompt Application

<div style="line-height:0.2em;">



[**A mathematical perspective on Transformers**](https://arxiv.org/abs/2312.10794) （**2023.12.17**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-9-blue)](https://github.com/borjang/2023-transformers-rotf)

[**Mathematical discoveries from program search with large language models.**](https://doi.org/10.1038/s41586-023-06924-6) （**2023.12.14**）

![](https://img.shields.io/badge/Citations-1-green)

[**LLM360: Towards Fully Transparent Open-Source LLMs**](https://arxiv.org/abs/2312.06550) （**2023.12.11**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-15-red)  [![](https://img.shields.io/badge/Github%20Stars-46-blue)](https://github.com/llm360/analysis360)

[**From Text to Motion: Grounding GPT-4 in a Humanoid Robot"Alter3"**](https://arxiv.org/abs/2312.06571) （**2023.12.11**）

![](https://img.shields.io/badge/Citations-0-green)

[**Control Risk for Potential Misuse of Artificial Intelligence in Science**](https://arxiv.org/abs/2312.06632) （**2023.12.11**）

![](https://img.shields.io/badge/Citations-0-green)

[**Sequential Modeling Enables Scalable Learning for Large Vision Models**](https://arxiv.org/abs/2312.00785) （**2023.12.01**）

![](https://img.shields.io/badge/Citations-0-green)

[**MeshGPT: Generating Triangle Meshes with Decoder-Only Transformers**](https://doi.org/10.48550/arXiv.2311.15475) （**2023.11.27**）

![](https://img.shields.io/badge/Citations-0-green)

[**Minimizing Factual Inconsistency and Hallucination in Large Language Models**](https://doi.org/10.48550/arXiv.2311.13878) （**2023.11.23**）

![](https://img.shields.io/badge/Citations-0-green)

[**Igniting Language Intelligence: The Hitchhiker's Guide From Chain-of-Thought Reasoning to Language Agents**](https://doi.org/10.48550/arXiv.2311.11797) （**2023.11.20**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-252-blue)](https://github.com/zoeyyao27/cot-igniting-agent)

[**An Embodied Generalist Agent in 3D World**](https://doi.org/10.48550/arXiv.2311.12871) （**2023.11.18**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-117-blue)](https://github.com/embodied-generalist/embodied-generalist)


</div>

👉[Complete paper list 🔗 for "Prompt Application"](./PaperList/promptapplication.md)👈

## Foundation Models

<div style="line-height:0.2em;">



[**Time is Encoded in the Weights of Finetuned Language Models**](https://arxiv.org/abs/2312.13401) （**2023.12.20**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-30-blue)](https://github.com/KaiNylund/lm-weights-encode-time)

[**Photorealistic Video Generation with Diffusion Models**](https://arxiv.org/abs/2312.06662) （**2023.12.11**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-39-red)

[**Mamba: Linear-Time Sequence Modeling with Selective State Spaces**](https://arxiv.org/abs/2312.00752) （**2023.12.01**）

![](https://img.shields.io/badge/Citations-1-green)

[**Minimizing Factual Inconsistency and Hallucination in Large Language Models**](https://doi.org/10.48550/arXiv.2311.13878) （**2023.11.23**）

![](https://img.shields.io/badge/Citations-0-green)

[**White-Box Transformers via Sparse Rate Reduction: Compression Is All There Is?**](https://doi.org/10.48550/arXiv.2311.13110) （**2023.11.22**）

![](https://img.shields.io/badge/Citations-0-green)

[**Learning skillful medium-range global weather forecasting.**](https://doi.org/10.1126/science.adi2336) （**2023.11.14**）

![](https://img.shields.io/badge/Citations-8-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-360-red)

[**Chat-UniVi: Unified Visual Representation Empowers Large Language Models with Image and Video Understanding**](https://doi.org/10.48550/arXiv.2311.08046) （**2023.11.14**）

![](https://img.shields.io/badge/Citations-3-green)

[**SpectralGPT: Spectral Foundation Model**](https://doi.org/10.48550/arXiv.2311.07113) （**2023.11.13**）

![](https://img.shields.io/badge/Citations-0-green)

[**Social Motion Prediction with Cognitive Hierarchies**](https://doi.org/10.48550/arXiv.2311.04726) （**2023.11.08**）

![](https://img.shields.io/badge/Citations-0-green)

[**Pre-training LLMs using human-like development data corpus**](https://doi.org/10.48550/arXiv.2311.04666) （**2023.11.08**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Foundation Models"](./PaperList/foundationmodels.md)👈

<!-- ### 📌 Hard Prompt/ Discrete Prompt

<div style="line-height:0.2em;">



[**Winner-Take-All Column Row Sampling for Memory Efficient Adaptation of Language Model**](https://arxiv.org/abs/2305.15265) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-1-blue)](https://github.com/zirui-ray-liu/wtacrs)

[**How to Distill your BERT: An Empirical Study on the Impact of Weight Initialisation and Distillation Objectives**](https://arxiv.org/abs/2305.15032) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-12-red)  [![](https://img.shields.io/badge/Github%20Stars-8-blue)](https://github.com/mainlp/how-to-distill-your-bert)

[**ChatAgri: Exploring Potentials of ChatGPT on Cross-linguistic Agricultural Text Classification**](https://arxiv.org/abs/2305.15024) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-51-red)  [![](https://img.shields.io/badge/Github%20Stars-32-blue)](https://github.com/albert-jin/agricultural_textual_classification_chatgpt)

[**Cheap and Quick: Efficient Vision-Language Instruction Tuning for Large Language Models**](https://arxiv.org/abs/2305.15023) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-49-red)

[**LLMDet: A Large Language Models Detection Tool**](https://arxiv.org/abs/2305.15004) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-7-red)

[**OverPrompt: Enhancing ChatGPT Capabilities through an Efficient In-Context Learning Approach**](https://arxiv.org/abs/2305.14973) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-8-red)

[**In-Context Demonstration Selection with Cross Entropy Difference**](https://arxiv.org/abs/2305.14726) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-5-red)  [![](https://img.shields.io/badge/Github%20Stars-2.8k-blue)](https://github.com/microsoft/lmops)

[**Contrastive Learning with Logic-driven Data Augmentation for Logical Reasoning over Text**](https://arxiv.org/abs/2305.12599) （**2023.05.21**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)

[**LogiCoT: Logical Chain-of-Thought Instruction-Tuning Data Collection with GPT-4**](https://arxiv.org/abs/2305.12147) （**2023.05.20**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-9-red)

[**SelfzCoT: a Self-Prompt Zero-shot CoT from Semantic-level to Code-level for a Better Utilization of LLMs**](https://doi.org/10.48550/arXiv.2305.11461) （**2023.05.19**）

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