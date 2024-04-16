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

- **[2024.4.16]**
  - Paper: [MMInA: Benchmarking Multihop Multimodal Internet Agents](https://arxiv.org/abs/2404.09992)
  - Paper: [Memory Sharing for Large Language Model based Agents](https://arxiv.org/abs/2404.09982)
  - Paper: [LLMorpheus: Mutation Testing using Large Language Models](https://arxiv.org/abs/2404.09952)


- **[2024.4.15]**
  - Paper: [Superposition Prompting: Improving and Accelerating Retrieval-Augmented Generation](https://arxiv.org/abs/2404.06910)
  - Paper: [BRAVE: Broadening the visual encoding of vision-language models](https://arxiv.org/abs/2404.07204)
  - Paper: [From Model-centered to Human-Centered: Revision Distance as a Metric for Text Evaluation in LLMs-based Applications](https://arxiv.org/abs/2404.07108)

- **[2024.4.14]**
  - Paper: [ExeGPT: Constraint-Aware Resource Scheduling for LLM Inference](https://arxiv.org/abs/2404.07947)
  - Paper: [ORacle: Large Vision-Language Models for Knowledge-Guided Holistic OR Domain Modeling](https://arxiv.org/abs/2404.07031)
  - Paper: [MetaCheckGPT -- A Multi-task Hallucination Detector Using LLM Uncertainty and Meta-models](https://arxiv.org/abs/2404.06948)

- **[2024.4.13]**
  - Paper: [OpenBias: Open-set Bias Detection in Text-to-Image Generative Models](https://arxiv.org/abs/2404.07990)
  - Paper: [Any2Point: Empowering Any-modality Large Models for Efficient 3D Understanding](https://arxiv.org/abs/2404.07989)
  - Paper: [Manipulating Large Language Models to Increase Product Visibility](https://arxiv.org/abs/2404.07981)

- **[2024.4.12]**
  - Paper: [RecurrentGemma: Moving Past Transformers for Efficient Open Language Models](https://arxiv.org/abs/2404.07839)
  - Paper: [Generating consistent PDDL domains with Large Language Models](https://arxiv.org/abs/2404.07751)
  - Paper: [ResearchAgent: Iterative Research Idea Generation over Scientific Literature with Large Language Models](https://arxiv.org/abs/2404.07738)

- **[2024.4.11]**
  - Paper: [ExeGPT: Constraint-Aware Resource Scheduling for LLM Inference](https://arxiv.org/abs/2404.07947)
  - Paper: [InfiCoder-Eval: Systematically Evaluating the Question-Answering Capabilities of Code Large Language Models](https://arxiv.org/abs/2404.07940)
  - Paper: [High-Dimension Human Value Representation in Large Language Models](https://arxiv.org/abs/2404.07900)

- **[2024.4.10]**
  - Paper: [OSWorld: Benchmarking Multimodal Agents for Open-Ended Tasks in Real Computer Environments](https://arxiv.org/abs/2404.07972)
  - Paper: [EduAgent: Generative Student Agents in Learning](https://arxiv.org/abs/2404.07963)
  - Paper: [Content Knowledge Identification with Multi-Agent Large Language Models (LLMs)](https://arxiv.org/abs/2404.07960)

- **[2024.4.9]**
  - Paper: [Ferret-UI: Grounded Mobile UI Understanding with Multimodal LLMs](https://arxiv.org/abs/2404.05719)
  - Paper: [MoMA: Multimodal LLM Adapter for Fast Personalized Image Generation](https://arxiv.org/abs/2404.05674)
  - Paper: [MIMIR: A Streamlined Platform for Personalized Agent Tuning in Domain Expertise](https://arxiv.org/abs/2404.04285)

- **[2024.4.8]**
  - Paper: [Long-horizon Locomotion and Manipulation on a Quadrupedal Robot with Large Language Models](https://arxiv.org/abs/2404.05291)
  - Paper: [LayoutLLM: Layout Instruction Tuning with Large Language Models for Document Understanding](https://arxiv.org/abs/2404.05225)
  - Paper: [DLoRA: Distributed Parameter-Efficient Fine-Tuning Solution for Large Language Model](https://arxiv.org/abs/2404.05182)

- **[2024.4.7]**
  - Paper: [LongVLM: Efficient Long Video Understanding via Large Language Models](https://arxiv.org/abs/2404.03384)
  - Paper: [nicolay-r at SemEval-2024 Task 3: Using Flan-T5 for Reasoning Emotion Cause in Conversations with Chain-of-Thought on Emotion States](https://arxiv.org/abs/2404.03361)
  - Paper: [Do Large Language Models Rank Fairly? An Empirical Study on the Fairness of LLMs as Rankers](https://arxiv.org/abs/2404.03192)

- **[2024.4.6]**
  - Paper: [Can Small Language Models Help Large Language Models Reason Better?: LM-Guided Chain-of-Thought](https://arxiv.org/abs/2404.03414)
  - Paper: [MiniGPT4-Video: Advancing Multimodal LLMs for Video Understanding with Interleaved Visual-Textual Tokens](https://arxiv.org/abs/2404.03413)
  - Paper: [Scaling Up Video Summarization Pretraining with Large Language Models](https://arxiv.org/abs/2404.03398)

- **[2024.4.5]**
  - Paper:[Evaluating LLMs at Detecting Errors in LLM Responses](https://arxiv.org/abs/2404.03602)
  - Paper:[Laser Learning Environment: A new environment for coordination-critical multi-agent tasks](https://arxiv.org/abs/2404.03596)
  - Paper:[Untangle the KNOT: Interweaving Conflicting Knowledge and Reasoning Skills in Large Language Models](https://arxiv.org/abs/2404.03577)

- **[2024.4.4]**
  - Paper:[AutoWebGLM: Bootstrap And Reinforce A Large Language Model-based Web Navigating Agent](https://arxiv.org/abs/2404.03648)
  - Paper:[Unveiling LLMs: The Evolution of Latent Representations in a Temporal Knowledge Graph](https://arxiv.org/abs/2404.03623)
  - Paper:[Visualization-of-Thought Elicits Spatial Reasoning in Large Language Models](https://arxiv.org/abs/2404.03622)

- **[2024.4.3]**
  - Paper: [Topic-based Watermarks for LLM-Generated Text](https://arxiv.org/abs/2404.02138)
  - Paper: [ViTamin: Designing Scalable Vision Models in the Vision-Language Era](https://arxiv.org/abs/2404.02132)
  - Paper: [Pre-trained Vision and Language Transformers Are Few-Shot Incremental Learners](https://arxiv.org/abs/2404.02117)

- **[2024.4.2]**
  - Paper: [Segment Any 3D Object with Language](https://arxiv.org/abs/2404.02157)
  - Paper: [Jailbreaking Leading Safety-Aligned LLMs with Simple Adaptive Attacks](https://arxiv.org/abs/2404.02151)
  - Paper: [Iterated Learning Improves Compositionality in Large Vision-Language Models](https://arxiv.org/abs/2404.02145)

- **[2024.4.1]**
  - Paper: [LUQ: Long-text Uncertainty Quantification for LLMs](https://arxiv.org/abs/2403.20279)
  - Paper: [ELITR-Bench: A Meeting Assistant Benchmark for Long-Context Language Models](https://arxiv.org/abs/2403.20262)
  - Paper: [ChatGPT v.s. Media Bias: A Comparative Study of GPT-3.5 and Fine-tuned Language Models](https://arxiv.org/abs/2403.20158)

- **[2024.3.31]**
  - Paper: [MTLoRA: A Low-Rank Adaptation Approach for Efficient Multi-Task Learning](https://arxiv.org/abs/2403.20320)
  - Paper: [Convolutional Prompting meets Language Models for Continual Learning](https://arxiv.org/abs/2403.20317)
  - Paper: [Towards Greener LLMs: Bringing Energy-Efficiency to the Forefront of LLM Inference](https://arxiv.org/abs/2403.20306)

- **[2024.3.30]**
  - Paper: [Unsolvable Problem Detection: Evaluating Trustworthiness of Vision Language Models](https://arxiv.org/abs/2403.20331)
  - Paper: [ReALM: Reference Resolution As Language Modeling](https://arxiv.org/abs/2403.20329)
  - Paper: [Gecko: Versatile Text Embeddings Distilled from Large Language Models](https://arxiv.org/abs/2403.20327)

- **[2024.3.29]**
  - Paper: [RSMamba: Remote Sensing Image Classification with State Space Model](https://arxiv.org/abs/2403.19654)
  - Paper: [Change-Agent: Towards Interactive Comprehensive Change Interpretation and Analysis from Change Detection and Change Captioning](https://arxiv.org/abs/2403.19646)
  - Paper: [WaterJudge: Quality-Detection Trade-off when Watermarking Large Language Models](https://arxiv.org/abs/2403.19548)

- **[2024.3.28]**
  - Paper: [Mini-Gemini: Mining the Potential of Multi-modality Vision Language Models](https://arxiv.org/abs/2403.18814)
  - Paper: [3P-LLM: Probabilistic Path Planning using Large Language Model for Autonomous Robot Navigation](https://arxiv.org/abs/2403.18778)
  - Paper: [MLDT: Multi-Level Decomposition for Complex Long-Horizon Robotic Task Planning with Open-Source Large Language Model](https://arxiv.org/abs/2403.18760)

- **[2024.3.27]**
  - 🔥🔥🔥[Stability AI open-sources 3B code generation model: it's patchable, and it can Debug](https://huggingface.co/stabilityai/stable-code-instruct-3b)
  - 🔥🔥🔥[Suno, the "AI Songwriter", is a hit in the music industry.](https://www.techradar.com/computing/artificial-intelligence/what-is-suno-ai)
  - Paper: [TextMonkey: An OCR-Free Large Multimodal Model for Understanding Document](https://arxiv.org/abs/2403.04473)
  
- **[2024.3.26]**
  - Paper: [AIOS: LLM Agent Operating System](https://arxiv.org/abs/2403.16971)
  - Paper: [Bayesian Methods for Trust in Collaborative Multi-Agent Autonomy](https://arxiv.org/abs/2403.16956)
  - Paper: [Multi-Agent Optimization for Safety Analysis of Cyber-Physical Systems: Position Paper](https://arxiv.org/abs/2403.16904)

- **[2024.3.25]**
  - Paper: [DreamLIP: Language-Image Pre-training with Long Captions](https://arxiv.org/abs/2403.17007)
  - Paper: [Visual CoT: Unleashing Chain-of-Thought Reasoning in Multi-Modal Language Models](https://arxiv.org/abs/2403.16999)
  - Paper: [Comp4D: LLM-Guided Compositional 4D Scene Generation](https://arxiv.org/abs/2403.16993)

[👉 Complete history news 👈](./historynews.md)

<img width="200%" src="./figures/hr.gif" />

---

# 📜 Papers

> You can directly click on the title to jump to the corresponding PDF link location

## Survey

<div style="line-height:0.2em;">


<div style="line-height:0.2em;">



[**The Ethics of ChatGPT in Medicine and Healthcare: A Systematic Review on Large Language Models (LLMs)**](https://arxiv.org/abs/2403.14473) （**2024.03.21**）

![](https://img.shields.io/badge/Citations-0-green)

[**Parameter-Efficient Fine-Tuning for Large Models: A Comprehensive Survey**](https://arxiv.org/abs/2403.14608) （**2024.03.21**）

![](https://img.shields.io/badge/Citations-0-green)

[**ChatGPT Alternative Solutions: Large Language Models Survey**](https://doi.org/10.5121/csit.2024.140514) （**2024.03.16**）

![](https://img.shields.io/badge/Citations-0-green)

[**MM1: Methods, Analysis&Insights from Multimodal LLM Pre-training**](https://arxiv.org/abs/2403.09611) （**2024.03.14**）

![](https://img.shields.io/badge/Citations-1-green)

[**Large Language Models and Causal Inference in Collaboration: A Comprehensive Survey**](https://arxiv.org/abs/2403.09606) （**2024.03.14**）

![](https://img.shields.io/badge/Citations-0-green)

[**Model Parallelism on Distributed Infrastructure: A Literature Review from Theory to LLM Case-Studies**](https://arxiv.org/abs/2403.03699) （**2024.03.06**）

![](https://img.shields.io/badge/Citations-0-green)

[**Benchmarking the Text-to-SQL Capability of Large Language Models: A Comprehensive Evaluation**](https://arxiv.org/abs/2403.02951) （**2024.03.05**）

![](https://img.shields.io/badge/Citations-1-green)

[**A Comprehensive Survey on Process-Oriented Automatic Text Summarization with Exploration of LLM-Based Methods**](https://arxiv.org/abs/2403.02901) （**2024.03.05**）

![](https://img.shields.io/badge/Citations-0-green)

[**Large Language Models for Data Annotation: A Survey**](https://arxiv.org/abs/2402.13446) （**2024.02.21**）

![](https://img.shields.io/badge/Citations-0-green)

[**A Survey on Knowledge Distillation of Large Language Models**](https://arxiv.org/abs/2402.13116) （**2024.02.20**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Survey"](./PaperList/survey.md)👈

## Prompt Engineering

### Prompt Design

<div style="line-height:0.2em;">



[**SAMCT: Segment Any CT Allowing Labor-Free Task-Indicator Prompts**](https://arxiv.org/abs/2403.13258) （**2024.03.20**）

![](https://img.shields.io/badge/Citations-0-green)

[**AFLoRA: Adaptive Freezing of Low Rank Adaptation in Parameter Efficient Fine-Tuning of Large Models**](https://arxiv.org/abs/2403.13269) （**2024.03.20**）

![](https://img.shields.io/badge/Citations-0-green)

[**Few-Shot Class Incremental Learning with Attention-Aware Self-Adaptive Prompt**](https://arxiv.org/abs/2403.09857) （**2024.03.14**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)

[**Unveiling the Generalization Power of Fine-Tuned Large Language Models**](https://arxiv.org/abs/2403.09162) （**2024.03.14**）

![](https://img.shields.io/badge/Citations-0-green)

[**Attention Prompt Tuning: Parameter-efficient Adaptation of Pre-trained Models for Spatiotemporal Modeling**](https://arxiv.org/abs/2403.06978) （**2024.03.11**）

![](https://img.shields.io/badge/Citations-0-green)

[**VidProM: A Million-scale Real Prompt-Gallery Dataset for Text-to-Video Diffusion Models**](https://arxiv.org/abs/2403.06098) （**2024.03.10**）

![](https://img.shields.io/badge/Citations-0-green)

[**Localized Zeroth-Order Prompt Optimization**](https://arxiv.org/abs/2403.02993) （**2024.03.05**）

![](https://img.shields.io/badge/Citations-0-green)

[**RIFF: Learning to Rephrase Inputs for Few-shot Fine-tuning of Language Models**](https://arxiv.org/abs/2403.02271) （**2024.03.04**）

![](https://img.shields.io/badge/Citations-0-green)

[**Prompt-Driven Dynamic Object-Centric Learning for Single Domain Generalization**](https://arxiv.org/abs/2402.18447) （**2024.02.28**）

![](https://img.shields.io/badge/Citations-0-green)

[**Meta-Task Prompting Elicits Embedding from Large Language Models**](https://arxiv.org/abs/2402.18458) （**2024.02.28**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Prompt Design"](./PaperList/PromptDesignList.md)👈

### Chain of Thought

<div style="line-height:0.2em;">



[**Visual CoT: Unleashing Chain-of-Thought Reasoning in Multi-Modal Language Models**](https://arxiv.org/abs/2403.16999) （**2024.03.25**）

![](https://img.shields.io/badge/Citations-0-green)

[**A Chain-of-Thought Prompting Approach with LLMs for Evaluating Students' Formative Assessment Responses in Science**](https://arxiv.org/abs/2403.14565) （**2024.03.21**）

![](https://img.shields.io/badge/Citations-0-green)

[**NavCoT: Boosting LLM-Based Vision-and-Language Navigation via Learning Disentangled Reasoning**](https://arxiv.org/abs/2403.07376) （**2024.03.12**）

![](https://img.shields.io/badge/Citations-0-green)

[**ERA-CoT: Improving Chain-of-Thought through Entity Relationship Analysis**](https://arxiv.org/abs/2403.06932) （**2024.03.11**）

![](https://img.shields.io/badge/Citations-1-green)

[**Bias-Augmented Consistency Training Reduces Biased Reasoning in Chain-of-Thought**](https://arxiv.org/abs/2403.05518) （**2024.03.08**）

![](https://img.shields.io/badge/Citations-0-green)

[**Chain-of-Thought Unfaithfulness as Disguised Accuracy**](https://doi.org/10.48550/arXiv.2402.14897) （**2024.02.22**）

![](https://img.shields.io/badge/Citations-0-green)

[**Chain-of-Thought Reasoning Without Prompting**](https://doi.org/10.48550/arXiv.2402.10200) （**2024.02.15**）

![](https://img.shields.io/badge/Citations-0-green)

[**Chain-of-Table: Evolving Tables in the Reasoning Chain for Table Understanding**](https://doi.org/10.48550/arXiv.2401.04398) （**2024.01.09**）

![](https://img.shields.io/badge/Citations-3-green)

[**A Logically Consistent Chain-of-Thought Approach for Stance Detection**](https://arxiv.org/abs/2312.16054) （**2023.12.26**）

![](https://img.shields.io/badge/Citations-0-green)

[**Assessing the Impact of Prompting, Persona, and Chain of Thought Methods on ChatGPT's Arithmetic Capabilities**](https://arxiv.org/abs/2312.15006) （**2023.12.22**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Chain of Thought"](./PaperList/ChainofThoughtList.md)👈

### In-context Learning

<div style="line-height:0.2em;">



[**AFLoRA: Adaptive Freezing of Low Rank Adaptation in Parameter Efficient Fine-Tuning of Large Models**](https://arxiv.org/abs/2403.13269) （**2024.03.20**）

![](https://img.shields.io/badge/Citations-0-green)

[**ExploRLLM: Guiding Exploration in Reinforcement Learning with Large Language Models**](https://arxiv.org/abs/2403.09583) （**2024.03.14**）

![](https://img.shields.io/badge/Citations-0-green)

[**NavCoT: Boosting LLM-Based Vision-and-Language Navigation via Learning Disentangled Reasoning**](https://arxiv.org/abs/2403.07376) （**2024.03.12**）

![](https://img.shields.io/badge/Citations-0-green)

[**Attention Prompt Tuning: Parameter-efficient Adaptation of Pre-trained Models for Spatiotemporal Modeling**](https://arxiv.org/abs/2403.06978) （**2024.03.11**）

![](https://img.shields.io/badge/Citations-0-green)

[**Bias-Augmented Consistency Training Reduces Biased Reasoning in Chain-of-Thought**](https://arxiv.org/abs/2403.05518) （**2024.03.08**）

![](https://img.shields.io/badge/Citations-0-green)

[**LoRA-SP: Streamlined Partial Parameter Adaptation for Resource-Efficient Fine-Tuning of Large Language Models**](https://arxiv.org/abs/2403.08822) （**2024.02.28**）

![](https://img.shields.io/badge/Citations-0-green)

[**Securing Reliability: A Brief Overview on Enhancing In-Context Learning for Foundation Models**](https://arxiv.org/abs/2402.17671) （**2024.02.27**）

![](https://img.shields.io/badge/Citations-0-green)

[**GISTEmbed: Guided In-sample Selection of Training Negatives for Text Embedding Fine-tuning**](https://doi.org/10.48550/arXiv.2402.16829) （**2024.02.26**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-15-blue)](https://github.com/avsolatorio/gistembed)

[**DiffuCOMET: Contextual Commonsense Knowledge Diffusion**](https://arxiv.org/abs/2402.17011) （**2024.02.26**）

![](https://img.shields.io/badge/Citations-0-green)

[**Long-Context Language Modeling with Parallel Context Encoding**](https://arxiv.org/abs/2402.16617) （**2024.02.26**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "In-context Learning"](./PaperList/InContextLearningList.md)👈


### Retrieval Augmented Generation

<div style="line-height:0.2em;">



[**Retrieval-Augmented Generation for AI-Generated Content: A Survey**](https://arxiv.org/abs/2402.19473) （**2024.02.29**）

![](https://img.shields.io/badge/Citations-0-green)

[**VerifiNER: Verification-augmented NER via Knowledge-grounded Reasoning with Large Language Models**](https://arxiv.org/abs/2402.18374) （**2024.02.28**）

![](https://img.shields.io/badge/Citations-0-green)

[**LLM Augmented LLMs: Expanding Capabilities through Composition**](https://doi.org/10.48550/arXiv.2401.02412) （**2024.01.04**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-120-blue)](https://github.com/lucidrains/CALM-pytorch)

[**ARES: An Automated Evaluation Framework for Retrieval-Augmented Generation Systems**](https://doi.org/10.48550/arXiv.2311.09476) （**2023.11.16**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-237-blue)](https://github.com/stanford-futuredata/ares)

[**Chain-of-Note: Enhancing Robustness in Retrieval-Augmented Language Models**](https://doi.org/10.48550/arXiv.2311.09210) （**2023.11.15**）

![](https://img.shields.io/badge/Citations-17-green)

[**From Classification to Generation: Insights into Crosslingual Retrieval Augmented ICL**](https://doi.org/10.48550/arXiv.2311.06595) （**2023.11.11**）

![](https://img.shields.io/badge/Citations-1-green)

[**Optimizing Retrieval-augmented Reader Models via Token Elimination**](https://doi.org/10.48550/arXiv.2310.13682) （**2023.10.20**）

![](https://img.shields.io/badge/Citations-3-green)  [![](https://img.shields.io/badge/Github%20Stars-4-blue)](https://github.com/mosheber/token_elimination)

[**Self-RAG: Learning to Retrieve, Generate, and Critique through Self-Reflection**](https://doi.org/10.48550/arXiv.2310.11511) （**2023.10.17**）

![](https://img.shields.io/badge/Citations-13-green)

[**Retrieve Anything To Augment Large Language Models**](https://doi.org/10.48550/arXiv.2310.07554) （**2023.10.11**）

![](https://img.shields.io/badge/Citations-10-green)  [![](https://img.shields.io/badge/Github%20Stars-3.6k-blue)](https://github.com/flagopen/flagembedding)

[**Self-Knowledge Guided Retrieval Augmentation for Large Language Models**](https://doi.org/10.48550/arXiv.2310.05002) （**2023.10.08**）

![](https://img.shields.io/badge/Citations-3-green)


</div>

👉[Complete paper list 🔗 for "Retrieval Augmented Generation"](./PaperList/KnowledgeAugmentedPromptList.md)👈


### Evaluation & Reliability

<div style="line-height:0.2em;">



[**ERBench: An Entity-Relationship based Automatically Verifiable Hallucination Benchmark for Large Language Models**](https://arxiv.org/abs/2403.05266) （**2024.03.08**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-4-blue)](https://github.com/dilab-kaist/erbench)

[**Benchmarking the Text-to-SQL Capability of Large Language Models: A Comprehensive Evaluation**](https://arxiv.org/abs/2403.02951) （**2024.03.05**）

![](https://img.shields.io/badge/Citations-1-green)

[**Beyond Specialization: Assessing the Capabilities of MLLMs in Age and Gender Estimation**](https://arxiv.org/abs/2403.02302) （**2024.03.04**）

![](https://img.shields.io/badge/Citations-0-green)

[**A Cognitive Evaluation Benchmark of Image Reasoning and Description for Large Vision Language Models**](https://arxiv.org/abs/2402.18409) （**2024.02.28**）

![](https://img.shields.io/badge/Citations-0-green)

[**Evaluating Very Long-Term Conversational Memory of LLM Agents**](https://doi.org/10.48550/arXiv.2402.17753) （**2024.02.27**）

![](https://img.shields.io/badge/Citations-0-green)

[**Semantic Mirror Jailbreak: Genetic Algorithm Based Jailbreak Prompts Against Open-source LLMs**](https://doi.org/10.48550/arXiv.2402.14872) （**2024.02.21**）

![](https://img.shields.io/badge/Citations-0-green)

[**TofuEval: Evaluating Hallucinations of LLMs on Topic-Focused Dialogue Summarization**](https://arxiv.org/abs/2402.13249) （**2024.02.20**）

![](https://img.shields.io/badge/Citations-0-green)

[**How Well Can LLMs Negotiate? NegotiationArena Platform and Analysis**](https://doi.org/10.48550/arXiv.2402.05863) （**2024.02.08**）

![](https://img.shields.io/badge/Citations-1-green)

[**Can Large Language Models Understand Context?**](https://doi.org/10.48550/arXiv.2402.00858) （**2024.02.01**）

![](https://img.shields.io/badge/Citations-1-green)

[**Evaluating Large Language Models for Generalization and Robustness via Data Compression**](https://doi.org/10.48550/arXiv.2402.00861) （**2024.02.01**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Evaluation & Reliability"](./PaperList/EvaluationReliabilityList.md)👈

## Agent

<div style="line-height:0.2em;">



[**Bayesian Methods for Trust in Collaborative Multi-Agent Autonomy**](https://arxiv.org/abs/2403.16956) （**2024.03.25**）

![](https://img.shields.io/badge/Citations-0-green)

[**AIOS: LLM Agent Operating System**](https://arxiv.org/abs/2403.16971) （**2024.03.25**）

![](https://img.shields.io/badge/Citations-0-green)

[**ReAct Meets ActRe: Autonomous Annotation of Agent Trajectories for Contrastive Self-Training**](https://arxiv.org/abs/2403.14589) （**2024.03.21**）

![](https://img.shields.io/badge/Citations-0-green)

[**VideoAgent: Long-form Video Understanding with Large Language Model as Agent**](https://arxiv.org/abs/2403.10517) （**2024.03.15**）

![](https://img.shields.io/badge/Citations-0-green)

[**SOTOPIA-$\pi$: Interactive Learning of Socially Intelligent Language Agents**](https://arxiv.org/abs/2403.08715) （**2024.03.13**）

![](https://img.shields.io/badge/Citations-0-green)

[**DeepSafeMPC: Deep Learning-Based Model Predictive Control for Safe Multi-Agent Reinforcement Learning**](https://arxiv.org/abs/2403.06397) （**2024.03.11**）

![](https://img.shields.io/badge/Citations-0-green)

[**OPEx: A Component-Wise Analysis of LLM-Centric Agents in Embodied Instruction Following**](https://arxiv.org/abs/2403.03017) （**2024.03.05**）

![](https://img.shields.io/badge/Citations-0-green)

[**Towards General Computer Control: A Multimodal Agent for Red Dead Redemption II as a Case Study**](https://arxiv.org/abs/2403.03186) （**2024.03.05**）

![](https://img.shields.io/badge/Citations-2-green)

[**Learning to Use Tools via Cooperative and Interactive Agents**](https://arxiv.org/abs/2403.03031) （**2024.03.05**）

![](https://img.shields.io/badge/Citations-0-green)

[**KnowAgent: Knowledge-Augmented Planning for LLM-Based Agents**](https://arxiv.org/abs/2403.03101) （**2024.03.05**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Agent"](./PaperList/AgentList.md)👈

## Multimodal Prompt

<div style="line-height:0.2em;">



[**Visual CoT: Unleashing Chain-of-Thought Reasoning in Multi-Modal Language Models**](https://arxiv.org/abs/2403.16999) （**2024.03.25**）

![](https://img.shields.io/badge/Citations-0-green)

[**Hierarchical Text-to-Vision Self Supervised Alignment for Improved Histopathology Representation Learning**](https://arxiv.org/abs/2403.14616) （**2024.03.21**）

![](https://img.shields.io/badge/Citations-0-green)

[**MyVLM: Personalizing VLMs for User-Specific Queries**](https://arxiv.org/abs/2403.14599) （**2024.03.21**）

![](https://img.shields.io/badge/Citations-0-green)

[**MathVerse: Does Your Multi-modal LLM Truly See the Diagrams in Visual Math Problems?**](https://arxiv.org/abs/2403.14624) （**2024.03.21**）

![](https://img.shields.io/badge/Citations-0-green)

[**PSALM: Pixelwise SegmentAtion with Large Multi-Modal Model**](https://arxiv.org/abs/2403.14598) （**2024.03.21**）

![](https://img.shields.io/badge/Citations-0-green)

[**SC-Tune: Unleashing Self-Consistent Referential Comprehension in Large Vision Language Models**](https://arxiv.org/abs/2403.13263) （**2024.03.20**）

![](https://img.shields.io/badge/Citations-0-green)

[**The First to Know: How Token Distributions Reveal Hidden Knowledge in Large Vision-Language Models?**](https://arxiv.org/abs/2403.09037) （**2024.03.14**）

![](https://img.shields.io/badge/Citations-0-green)

[**3D-VLA: A 3D Vision-Language-Action Generative World Model**](https://arxiv.org/abs/2403.09631) （**2024.03.14**）

![](https://img.shields.io/badge/Citations-1-green)

[**UniCode: Learning a Unified Codebook for Multimodal Large Language Models**](https://arxiv.org/abs/2403.09072) （**2024.03.14**）

![](https://img.shields.io/badge/Citations-0-green)

[**DeepSeek-VL: Towards Real-World Vision-Language Understanding**](https://arxiv.org/abs/2403.05525) （**2024.03.08**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Multimodal Prompt"](./PaperList/multimodalprompt.md)👈

## Prompt Application

<div style="line-height:0.2em;">



[**Comp4D: LLM-Guided Compositional 4D Scene Generation**](https://arxiv.org/abs/2403.16993) （**2024.03.25**）

![](https://img.shields.io/badge/Citations-0-green)

[**MathVerse: Does Your Multi-modal LLM Truly See the Diagrams in Visual Math Problems?**](https://arxiv.org/abs/2403.14624) （**2024.03.21**）

![](https://img.shields.io/badge/Citations-0-green)

[**Enhancing Code Generation Performance of Smaller Models by Distilling the Reasoning Ability of LLMs**](https://arxiv.org/abs/2403.13271) （**2024.03.20**）

![](https://img.shields.io/badge/Citations-0-green)

[**Instruction Multi-Constraint Molecular Generation Using a Teacher-Student Large Language Model**](https://arxiv.org/abs/2403.13244) （**2024.03.20**）

![](https://img.shields.io/badge/Citations-0-green)

[**Towards Robots That Know When They Need Help: Affordance-Based Uncertainty for Large Language Model Planners**](https://arxiv.org/abs/2403.13198) （**2024.03.19**）

![](https://img.shields.io/badge/Citations-0-green)

[**ChartInstruct: Instruction Tuning for Chart Comprehension and Reasoning**](https://arxiv.org/abs/2403.09028) （**2024.03.14**）

![](https://img.shields.io/badge/Citations-1-green)

[**Dynamic Memory Compression: Retrofitting LLMs for Accelerated Inference**](https://arxiv.org/abs/2403.09636) （**2024.03.14**）

![](https://img.shields.io/badge/Citations-0-green)

[**Towards Proactive Interactions for In-Vehicle Conversational Assistants Utilizing Large Language Models**](https://arxiv.org/abs/2403.09135) （**2024.03.14**）

![](https://img.shields.io/badge/Citations-0-green)

[**Simple and Scalable Strategies to Continually Pre-train Large Language Models**](https://arxiv.org/abs/2403.08763) （**2024.03.13**）

![](https://img.shields.io/badge/Citations-0-green)

[**LG-Traj: LLM Guided Pedestrian Trajectory Prediction**](https://arxiv.org/abs/2403.08032) （**2024.03.12**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Prompt Application"](./PaperList/promptapplication.md)👈

## Foundation Models

<div style="line-height:0.2em;">



[**DreamLIP: Language-Image Pre-training with Long Captions**](https://arxiv.org/abs/2403.17007) （**2024.03.25**）

![](https://img.shields.io/badge/Citations-0-green)

[**Instruction Multi-Constraint Molecular Generation Using a Teacher-Student Large Language Model**](https://arxiv.org/abs/2403.13244) （**2024.03.20**）

![](https://img.shields.io/badge/Citations-0-green)

[**VideoMamba: State Space Model for Efficient Video Understanding**](https://arxiv.org/abs/2403.06977) （**2024.03.11**）

![](https://img.shields.io/badge/Citations-1-green)

[**Mamba4Rec: Towards Efficient Sequential Recommendation with Selective State Space Models**](https://arxiv.org/abs/2403.03900) （**2024.03.06**）

![](https://img.shields.io/badge/Citations-0-green)

[**Griffin: Mixing Gated Linear Recurrences with Local Attention for Efficient Language Models**](https://arxiv.org/abs/2402.19427) （**2024.02.29**）

![](https://img.shields.io/badge/Citations-4-green)

[**LeMo-NADe: Multi-Parameter Neural Architecture Discovery with LLMs**](https://arxiv.org/abs/2402.18443) （**2024.02.28**）

![](https://img.shields.io/badge/Citations-0-green)

[**LoRA-SP: Streamlined Partial Parameter Adaptation for Resource-Efficient Fine-Tuning of Large Language Models**](https://arxiv.org/abs/2403.08822) （**2024.02.28**）

![](https://img.shields.io/badge/Citations-0-green)

[**GISTEmbed: Guided In-sample Selection of Training Negatives for Text Embedding Fine-tuning**](https://doi.org/10.48550/arXiv.2402.16829) （**2024.02.26**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-15-blue)](https://github.com/avsolatorio/gistembed)

[**Set the Clock: Temporal Alignment of Pretrained Language Models**](https://doi.org/10.48550/arXiv.2402.16797) （**2024.02.26**）

![](https://img.shields.io/badge/Citations-0-green)

[**Generative Pretrained Hierarchical Transformer for Time Series Forecasting**](https://arxiv.org/abs/2402.16516) （**2024.02.26**）

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

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-53-red)  [![](https://img.shields.io/badge/Github%20Stars-32-blue)](https://github.com/albert-jin/agricultural_textual_classification_chatgpt)

[**Cheap and Quick: Efficient Vision-Language Instruction Tuning for Large Language Models**](https://arxiv.org/abs/2305.15023) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-49-red)

[**LLMDet: A Large Language Models Detection Tool**](https://arxiv.org/abs/2305.15004) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-7-red)

[**OverPrompt: Enhancing ChatGPT Capabilities through an Efficient In-Context Learning Approach**](https://arxiv.org/abs/2305.14973) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-8-red)

[**Interpretable by Design Visual Question Answering**](https://arxiv.org/abs/2305.14882) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-3-red)

[**In-Context Demonstration Selection with Cross Entropy Difference**](https://arxiv.org/abs/2305.14726) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-5-red)  [![](https://img.shields.io/badge/Github%20Stars-2.8k-blue)](https://github.com/microsoft/lmops)

[**LogicLLM: Exploring Self-supervised Logic-enhanced Training for Large Language Models**](https://arxiv.org/abs/2305.13718) （**2023.05.23**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-13-red)  [![](https://img.shields.io/badge/Github%20Stars-1-blue)](https://github.com/sparkjiao/logicllm)

[**Contrastive Learning with Logic-driven Data Augmentation for Logical Reasoning over Text**](https://arxiv.org/abs/2305.12599) （**2023.05.21**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-3-red)


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