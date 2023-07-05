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

# 📢 News
<!-- 🔥🔥🔥 -->
☄️ **EgoAlpha releases the TrustGPT focuses on reasoning. Trust the GPT with the strongest reasoning abilities for authentic and reliable answers. You can click [here](https://trustgpt.co) or visit the [Playgrounds](./Playground.md) directly to experience it。**

- **[2023.7.5]**
    - [MetaGPT: Multi-Role Meta-Programming Framework](https://github.com/geekan/MetaGPT)
    - Paper: [Conformer LLMs -- Convolution Augmented Large Language Models](https://arxiv.org/abs/2307.00461)

- **[2023.7.4]**
    - Paper:[Shikra: Unleashing Multimodal LLM's Referential Dialogue Magic](http://arxiv.org/abs/2306.15195)
    
- **[2023.7.3]**
    - [Largest-scale Chinese multitask instruction set, introducing a thousand Chinese datasets.](https://huggingface.co/datasets/BAAI/COIG-PC)
    
- **[2023.7.2]**
    - Paper: [Towards Measuring the Representation of Subjective Global Opinions in Language Models](https://arxiv.org/abs/2306.16388)
    
- **[2023.7.1]**
    - Paper:[Masked Vision-language Transformer in Fashion](https://link.springer.com/article/10.1007/s11633-022-1394-4)
    
- **[2023.6.30]**
    - Paper: [Inferring the Goals of Communicating Agents from Actions and Instructions](https://arxiv.org/abs/2306.16207)

- **[2023.6.29]**
    - Paper: [AudioPaLM: A Large Language Model That Can Speak and Listen](https://arxiv.org/pdf/2306.12925.pdf)

- **[2023.6.28]**
    - Paper:[Kosmos-2: Grounding Multimodal Large Language Models to the World](https://arxiv.org/abs//2306.14824)

- **[2023.6.27]**
    - Paper: [A Survey on Multimodal Large Language Models](https://arxiv.org/pdf/2306.13549v1.pdf)
    
- **[2023.6.26]**
    - Paper: [PIXIU: A Large Language Model, Instruction Data and Evaluation Benchmark for Finance](https://arxiv.org/abs/2306.05443)

[👉 Complete history news 👈](./historynews.md)

<img width="200%" src="./figures/hr.gif" />

# 📜 Papers

> You can directly click on the title to jump to the corresponding PDF link location

- [Survey](#Survey)

- [Prompt Engineering](#prompt-engineering)

    - [Prompt Design](#prompt-design)
    - [Automatic Prompt](#automatic-prompt)
    - [Chain of Thought](#chain-of-thought)
    - [Knowledge Augmented Prompt](#knowledge-augmented-prompt)
    - [Evaluation & Reliability](#evaluation--reliability)

- [In-context learning](#in-context-learning)

- [Multimodal Prompt](#multimodal-prompt)

- [Prompt Application](#prompt-application)

- [Foundation Models](#foundation-models)

---

## Survey

<div style="line-height:0.2em;">



[**A Survey on Multimodal Large Language Models**](https://doi.org/10.48550/arXiv.2306.13549) （**2023.06.23**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-2.2k-blue)](https://github.com/bradyfu/awesome-multimodal-large-language-models)

[**A Survey of Vision-Language Pre-training from the Lens of Multimodal Machine Translation**](https://doi.org/10.48550/arXiv.2306.07198) （**2023.06.12**）

![](https://img.shields.io/badge/Citations-0-green)

[**Towards Revealing the Mystery behind Chain of Thought: a Theoretical Perspective**](https://arxiv.org/abs/2305.15408) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-2-red)

[**Do Models Really Learn to Follow Instructions? An Empirical Study of Instruction Tuning**](https://doi.org/10.48550/arXiv.2305.11383) （**2023.05.19**）

![](https://img.shields.io/badge/Citations-0-green)

[**Prompt Engineering for Healthcare: Methodologies and Applications**](https://doi.org/10.48550/arXiv.2304.14670) （**2023.04.28**）

![](https://img.shields.io/badge/Citations-0-green)

[**Harnessing the Power of LLMs in Practice: A Survey on ChatGPT and Beyond**](https://arxiv.org/abs/2304.13712) （**2023.04.26**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-257-red)  [![](https://img.shields.io/badge/Github%20Stars-5.3k-blue)](https://github.com/mooler0410/llmspracticalguide)

[**A Survey of Large Language Models**](https://arxiv.org/abs/2303.18223) （**2023.03.31**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-480-red)  [![](https://img.shields.io/badge/Github%20Stars-2.0k-blue)](https://github.com/rucaibox/llmsurvey)

[**Augmented Language Models: a Survey**](https://doi.org/10.48550/arXiv.2302.07842) （**2023.02.15**）

![](https://img.shields.io/badge/Citations-4-green)

[**A Survey for In-context Learning**](https://doi.org/10.48550/arXiv.2301.00234) （**2022.12.31**）

![](https://img.shields.io/badge/Citations-0-green)

[**Towards Reasoning in Large Language Models: A Survey**](https://doi.org/10.48550/arXiv.2212.10403) （**2022.12.20**）

![](https://img.shields.io/badge/Citations-5-green)  [![](https://img.shields.io/badge/Github%20Stars-331-blue)](https://github.com/jeffhj/lm-reasoning)


</div>

👉[Complete paper list 🔗 for "Survey"](./PaperList/survey.md)👈

## Prompt Engineering

### Prompt Design

<div style="line-height:0.2em;">



[**OphGLM: Training an Ophthalmology Large Language-and-Vision Assistant based on Instructions and Dialogue**](https://doi.org/10.48550/arXiv.2306.12174) （**2023.06.21**）

![](https://img.shields.io/badge/Citations-0-green)

[**PIXIU: A Large Language Model, Instruction Data and Evaluation Benchmark for Finance**](https://doi.org/10.48550/arXiv.2306.05443) （**2023.06.08**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-123-blue)](https://github.com/chancefocus/pixiu)

[**Learning Multi-Step Reasoning by Solving Arithmetic Tasks**](https://doi.org/10.48550/arXiv.2306.01707) （**2023.06.02**）

![](https://img.shields.io/badge/Citations-1-green)

[**OverPrompt: Enhancing ChatGPT Capabilities through an Efficient In-Context Learning Approach**](https://arxiv.org/abs/2305.14973) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**In-Context Impersonation Reveals Large Language Models' Strengths and Biases**](https://arxiv.org/abs/2305.14930) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-2-red)

[**Frugal Prompting for Dialog Models**](https://arxiv.org/abs/2305.14919) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Chain-of-Questions Training with Latent Answers for Robust Multistep Question Answering**](https://arxiv.org/abs/2305.14901) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-2-red)

[**Improving Probability-based Prompt Selection Through Unified Evaluation and Analysis**](https://arxiv.org/abs/2305.14877) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**BeamSearchQA: Large Language Models are Strong Zero-Shot QA Solver**](https://arxiv.org/abs/2305.14766) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**TACR: A Table-alignment-based Cell-selection and Reasoning Model for Hybrid Question-Answering**](https://arxiv.org/abs/2305.14682) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Prompt Design"](./PaperList/PromptDesignList.md)👈

### Automatic Prompt 

<div style="line-height:0.2em;">



[**Universal Self-adaptive Prompting**](https://arxiv.org/abs/2305.14926) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Discrete Prompt Optimization via Constrained Generation for Zero-shot Re-ranker**](https://arxiv.org/abs/2305.13729) （**2023.05.23**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-2-red)

[**Self-Polish: Enhance Reasoning in Large Language Models via Problem Refinement**](https://arxiv.org/abs/2305.14497) （**2023.05.23**）

![](https://img.shields.io/badge/Citations-0-green)

[**Learning Easily Updated General Purpose Text Representations with Adaptable Task-Specific Prefixes**](https://arxiv.org/abs/2305.13499) （**2023.05.22**）

![](https://img.shields.io/badge/Citations-0-green)

[**Automated Few-shot Classification with Instruction-Finetuned Language Models**](https://arxiv.org/abs/2305.12576) （**2023.05.21**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-3-blue)](https://github.com/raldir/aut-few)

[**AutoTrial: Prompting Language Models for Clinical Trial Design**](https://doi.org/10.48550/arXiv.2305.11366) （**2023.05.19**）

![](https://img.shields.io/badge/Citations-0-green)

[**Flatness-Aware Prompt Selection Improves Accuracy and Sample Efficiency**](https://doi.org/10.48550/arXiv.2305.10713) （**2023.05.18**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-4-blue)](https://github.com/shadowkiller33/flatness)

[**Compress, Then Prompt: Improving Accuracy-Efficiency Trade-off of LLM Inference with Transferable Prompt**](https://doi.org/10.48550/arXiv.2305.11186) （**2023.05.17**）

![](https://img.shields.io/badge/Citations-0-green)

[**Automatic Prompt Augmentation and Selection with Chain-of-Thought from Labeled Data**](https://doi.org/10.48550/arXiv.2302.12822) （**2023.02.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Guiding Large Language Models via Directional Stimulus Prompting**](https://doi.org/10.48550/arXiv.2302.11520) （**2023.02.22**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-11-blue)](https://github.com/leezekun/directional-stimulus-prompting)


</div>

👉[Complete paper list 🔗 for "Automatic Prompt"](./PaperList/AutomaticPromptList.md)👈

### Chain of Thought

<div style="line-height:0.2em;">



[**Chain-Of-Thought Prompting Under Streaming Batch: A Case Study**](https://doi.org/10.48550/arXiv.2306.00550) （**2023.06.01**）

![](https://img.shields.io/badge/Citations-0-green)

[**Majority Rule: better patching via Self-Consistency**](https://doi.org/10.48550/arXiv.2306.00108) （**2023.05.31**）

![](https://img.shields.io/badge/Citations-0-green)

[**Strategic Reasoning with Language Models**](https://doi.org/10.48550/arXiv.2305.19165) （**2023.05.30**）

![](https://img.shields.io/badge/Citations-0-green)

[**Code Prompting: a Neural Symbolic Method for Complex Reasoning in Large Language Models**](https://doi.org/10.48550/arXiv.2305.18507) （**2023.05.29**）

![](https://img.shields.io/badge/Citations-0-green)

[**Leveraging Training Data in Few-Shot Prompting for Numerical Reasoning**](https://doi.org/10.48550/arXiv.2305.18170) （**2023.05.29**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-5-blue)](https://github.com/allanj/dynamic-pal)

[**Tab-CoT: Zero-shot Tabular Chain of Thought**](https://doi.org/10.48550/arXiv.2305.17812) （**2023.05.28**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-13-blue)](https://github.com/xalp/tab-cot)

[**Beyond Chain-of-Thought, Effective Graph-of-Thought Reasoning in Large Language Models**](https://doi.org/10.48550/arXiv.2305.16582) （**2023.05.26**）

![](https://img.shields.io/badge/Citations-0-green)

[**MultiTool-CoT: GPT-3 Can Use Multiple External Tools with Chain of Thought Prompting**](https://doi.org/10.48550/arXiv.2305.16896) （**2023.05.26**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-9-blue)](https://github.com/inabatatsuro/multitool-cot)

[**Chain-of-Thought Hub: A Continuous Effort to Measure Large Language Models' Reasoning Performance**](https://doi.org/10.48550/arXiv.2305.17306) （**2023.05.26**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-1.5k-blue)](https://github.com/franxyao/chain-of-thought-hub)

[**Demo2Code: From Summarizing Demonstrations to Synthesizing Code via Extended Chain-of-Thought**](https://doi.org/10.48550/arXiv.2305.16744) （**2023.05.26**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Chain of Thought"](./PaperList/ChainofThoughtList.md)👈

### Knowledge Augmented Prompt

<div style="line-height:0.2em;">



[**Are Pre-trained Language Models Useful for Model Ensemble in Chinese Grammatical Error Correction?**](https://arxiv.org/abs/2305.15183) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Referral Augmentation for Zero-Shot Information Retrieval**](https://arxiv.org/abs/2305.15098) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Decomposing Complex Queries for Tip-of-the-tongue Retrieval**](https://arxiv.org/abs/2305.15053) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**LLMDet: A Large Language Models Detection Tool**](https://arxiv.org/abs/2305.15004) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**OverPrompt: Enhancing ChatGPT Capabilities through an Efficient In-Context Learning Approach**](https://arxiv.org/abs/2305.14973) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Frugal Prompting for Dialog Models**](https://arxiv.org/abs/2305.14919) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Bi-Drop: Generalizable Fine-tuning for Pre-trained Language Models via Adaptive Subnetwork Optimization**](https://arxiv.org/abs/2305.14760) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**In-Context Demonstration Selection with Cross Entropy Difference**](https://arxiv.org/abs/2305.14726) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**A Causal View of Entity Bias in (Large) Language Models**](https://arxiv.org/abs/2305.14695) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**SelfzCoT: a Self-Prompt Zero-shot CoT from Semantic-level to Code-level for a Better Utilization of LLMs**](https://doi.org/10.48550/arXiv.2305.11461) （**2023.05.19**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Knowledge Augmented Prompt"](./PaperList/KnowledgeAugmentedPromptList.md)👈


### Evaluation & Reliability

<div style="line-height:0.2em;">



[**Towards Measuring the Representation of Subjective Global Opinions in Language Models**](https://doi.org/10.48550/arXiv.2306.16388) （**2023.06.28**）

![](https://img.shields.io/badge/Citations-0-green)

[**SETI: Systematicity Evaluation of Textual Inference**](https://arxiv.org/abs/2305.15045) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Is GPT-4 a Good Data Analyst?**](https://arxiv.org/abs/2305.15038) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**From Words to Wires: Generating Functioning Electronic Devices from Natural Language Descriptions**](https://arxiv.org/abs/2305.14874) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)

[**Testing the General Deductive Reasoning Capacity of Large Language Models Using OOD Examples**](https://arxiv.org/abs/2305.15269) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)

[**EvEval: A Comprehensive Evaluation of Event Semantics for Large Language Models**](https://arxiv.org/abs/2305.15268) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**HuatuoGPT, towards Taming Language Model to Be a Doctor**](https://arxiv.org/abs/2305.15075) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-31-blue)](https://github.com/freedomintelligence/huatuogpt)

[**Have LLMs Advanced Enough? A Challenging Problem Solving Benchmark For Large Language Models**](https://arxiv.org/abs/2305.15074) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-6-red)  [![](https://img.shields.io/badge/Github%20Stars-20-blue)](https://github.com/hgaurav2k/jeebench)

[**ImageNetVC: Zero-Shot Visual Commonsense Evaluation on 1000 ImageNet Categories**](https://arxiv.org/abs/2305.15028) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-2-blue)](https://github.com/hemingkx/imagenetvc)

[**Sentiment Analysis in the Era of Large Language Models: A Reality Check**](https://arxiv.org/abs/2305.15005) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Evaluation & Reliability"](./PaperList/EvaluationReliabilityList.md)👈

## In-context Learning

<div style="line-height:0.2em;">



[**MetaVL: Transferring In-Context Learning Ability From Language Models to Vision-Language Models**](https://doi.org/10.48550/arXiv.2306.01311) （**2023.06.02**）

![](https://img.shields.io/badge/Citations-0-green)

[**SummIt: Iterative Text Summarization via ChatGPT**](https://arxiv.org/abs/2305.14835) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Measuring and Mitigating Constraint Violations of In-Context Learning for Utterance-to-API Semantic Parsing**](https://arxiv.org/abs/2305.15338) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)

[**OverPrompt: Enhancing ChatGPT Capabilities through an Efficient In-Context Learning Approach**](https://arxiv.org/abs/2305.14973) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Adversarial Demonstration Attacks on Large Language Models**](https://arxiv.org/abs/2305.14950) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Frugal Prompting for Dialog Models**](https://arxiv.org/abs/2305.14919) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Coverage-based Example Selection for In-Context Learning**](https://arxiv.org/abs/2305.14907) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Exploring Diverse In-Context Configurations for Image Captioning**](https://arxiv.org/abs/2305.14800) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-2.1k-blue)](https://github.com/mlfoundations/open_flamingo)

[**Mastering the ABCDs of Complex Questions: Answer-Based Claim Decomposition for Fine-grained Self-Evaluation**](https://arxiv.org/abs/2305.14750) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**In-Context Demonstration Selection with Cross Entropy Difference**](https://arxiv.org/abs/2305.14726) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "In-context Learning"](./PaperList/InContextLearningList.md)👈

## Multimodal Prompt

<div style="line-height:0.2em;">



[**Shikra: Unleashing Multimodal LLM's Referential Dialogue Magic**](https://doi.org/10.48550/arXiv.2306.15195) （**2023.06.27**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-111-blue)](https://github.com/shikras/shikra)

[**PromptIR: Prompting for All-in-One Blind Image Restoration**](https://arxiv.org/abs/2306.13090) （**2023.06.22**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-2-red)  [![](https://img.shields.io/badge/Github%20Stars-11-blue)](https://github.com/va1shn9v/promptir)

[**Macaw-LLM: Multi-Modal Language Modeling with Image, Audio, Video, and Text Integration**](https://doi.org/10.48550/arXiv.2306.09093) （**2023.06.15**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-979-blue)](https://github.com/lyuchenyang/macaw-llm)

[**Video-LLaMA: An Instruction-tuned Audio-Visual Language Model for Video Understanding**](https://doi.org/10.48550/arXiv.2306.02858) （**2023.06.05**）

![](https://img.shields.io/badge/Citations-4-green)  [![](https://img.shields.io/badge/Github%20Stars-1.0k-blue)](https://github.com/damo-nlp-sg/video-llama)

[**Meta-Learning For Vision-and-Language Cross-lingual Transfer**](https://arxiv.org/abs/2305.14843) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**LayoutGPT: Compositional Visual Planning and Generation with Large Language Models**](https://arxiv.org/abs/2305.15393) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-3-red)

[**Cream: Visually-Situated Natural Language Understanding with Contrastive Reading Model and Frozen Large Language Models**](https://arxiv.org/abs/2305.15080) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-4-red)  [![](https://img.shields.io/badge/Github%20Stars-6-blue)](https://github.com/naver-ai/cream)

[**EmbodiedGPT: Vision-Language Pre-Training via Embodied Chain of Thought**](https://arxiv.org/abs/2305.15021) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-3-red)  [![](https://img.shields.io/badge/Github%20Stars-19-blue)](https://github.com/EmbodiedGPT/EmbodiedGPT_Pytorch)

[**OverPrompt: Enhancing ChatGPT Capabilities through an Efficient In-Context Learning Approach**](https://arxiv.org/abs/2305.14973) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**In-Context Demonstration Selection with Cross Entropy Difference**](https://arxiv.org/abs/2305.14726) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Multimodal Prompt"](./PaperList/multimodalprompt.md)👈

## Prompt Application

<div style="line-height:0.2em;">



[**Inferring the Goals of Communicating Agents from Actions and Instructions**](https://doi.org/10.48550/arXiv.2306.16207) （**2023.06.28**）

![](https://img.shields.io/badge/Citations-1-green)

[**Kosmos-2: Grounding Multimodal Large Language Models to the World**](https://doi.org/10.48550/arXiv.2306.14824) （**2023.06.26**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-13.1k-blue)](https://github.com/microsoft/unilm/tree/master/kosmos-2)

[**AudioPaLM: A Large Language Model That Can Speak and Listen**](https://doi.org/10.48550/arXiv.2306.12925) （**2023.06.22**）

![](https://img.shields.io/badge/Citations-0-green)

[**XrayGPT: Chest Radiographs Summarization using Medical Vision-Language Models**](https://doi.org/10.48550/arXiv.2306.07971) （**2023.06.13**）

![](https://img.shields.io/badge/Citations-2-green)  [![](https://img.shields.io/badge/Github%20Stars-232-blue)](https://github.com/mbzuai-oryx/xraygpt)

[**PIXIU: A Large Language Model, Instruction Data and Evaluation Benchmark for Finance**](https://doi.org/10.48550/arXiv.2306.05443) （**2023.06.08**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-123-blue)](https://github.com/chancefocus/pixiu)

[**ChatDB: Augmenting LLMs with Databases as Their Symbolic Memory**](https://doi.org/10.48550/arXiv.2306.03901) （**2023.06.06**）

![](https://img.shields.io/badge/Citations-0-green)

[**Towards Revealing the Mystery behind Chain of Thought: a Theoretical Perspective**](https://arxiv.org/abs/2305.15408) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-2-red)

[**Peek Across: Improving Multi-Document Modeling via Cross-Document Question-Answering**](https://arxiv.org/abs/2305.15387) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**LLMDet: A Large Language Models Detection Tool**](https://arxiv.org/abs/2305.15004) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**OverPrompt: Enhancing ChatGPT Capabilities through an Efficient In-Context Learning Approach**](https://arxiv.org/abs/2305.14973) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Prompt Application"](./PaperList/promptapplication.md)👈

## Foundation Models

<div style="line-height:0.2em;">



[**Kosmos-2: Grounding Multimodal Large Language Models to the World**](https://doi.org/10.48550/arXiv.2306.14824) （**2023.06.26**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-13.1k-blue)](https://github.com/microsoft/unilm/tree/master/kosmos-2)

[**AudioPaLM: A Large Language Model That Can Speak and Listen**](https://doi.org/10.48550/arXiv.2306.12925) （**2023.06.22**）

![](https://img.shields.io/badge/Citations-0-green)

[**PIXIU: A Large Language Model, Instruction Data and Evaluation Benchmark for Finance**](https://doi.org/10.48550/arXiv.2306.05443) （**2023.06.08**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-123-blue)](https://github.com/chancefocus/pixiu)

[**M3Exam: A Multilingual, Multimodal, Multilevel Benchmark for Examining Large Language Models**](https://doi.org/10.48550/arXiv.2306.05179) （**2023.06.08**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-17-blue)](https://github.com/damo-nlp-sg/m3exam)

[**Simple and Controllable Music Generation**](https://doi.org/10.48550/arXiv.2306.05284) （**2023.06.08**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-7.8k-blue)](https://github.com/facebookresearch/audiocraft)

[**LLM-Blender: Ensembling Large Language Models with Pairwise Ranking and Generative Fusion**](https://doi.org/10.48550/arXiv.2306.02561) （**2023.06.05**）

![](https://img.shields.io/badge/Citations-0-green)

[**Towards Revealing the Mystery behind Chain of Thought: a Theoretical Perspective**](https://arxiv.org/abs/2305.15408) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-2-red)

[**Peek Across: Improving Multi-Document Modeling via Cross-Document Question-Answering**](https://arxiv.org/abs/2305.15387) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**SAMScore: A Semantic Structural Similarity Metric for Image Translation Evaluation**](https://arxiv.org/abs/2305.15367) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)  [![](https://img.shields.io/badge/Github%20Stars-4-blue)](https://github.com/kent0n-li/samscore)

[**LLMDet: A Large Language Models Detection Tool**](https://arxiv.org/abs/2305.15004) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Foundation Models"](./PaperList/foundationmodels.md)👈

<!-- ### 📌 Hard Prompt/ Discrete Prompt

<div style="line-height:0.2em;">



[**LLMDet: A Large Language Models Detection Tool**](https://arxiv.org/abs/2305.15004) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**OverPrompt: Enhancing ChatGPT Capabilities through an Efficient In-Context Learning Approach**](https://arxiv.org/abs/2305.14973) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**In-Context Demonstration Selection with Cross Entropy Difference**](https://arxiv.org/abs/2305.14726) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**LogiCoT: Logical Chain-of-Thought Instruction-Tuning Data Collection with GPT-4**](https://arxiv.org/abs/2305.12147) （**2023.05.20**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-10-blue)](https://github.com/csitfun/logicot)

[**SelfzCoT: a Self-Prompt Zero-shot CoT from Semantic-level to Code-level for a Better Utilization of LLMs**](https://doi.org/10.48550/arXiv.2305.11461) （**2023.05.19**）

![](https://img.shields.io/badge/Citations-0-green)

[**Do Models Really Learn to Follow Instructions? An Empirical Study of Instruction Tuning**](https://doi.org/10.48550/arXiv.2305.11383) （**2023.05.19**）

![](https://img.shields.io/badge/Citations-0-green)

[**AutoTrial: Prompting Language Models for Clinical Trial Design**](https://doi.org/10.48550/arXiv.2305.11366) （**2023.05.19**）

![](https://img.shields.io/badge/Citations-0-green)

[**Efficient Prompting via Dynamic In-Context Learning**](https://doi.org/10.48550/arXiv.2305.11170) （**2023.05.18**）

![](https://img.shields.io/badge/Citations-0-green)

[**Hard Prompts Made Easy: Gradient-Based Discrete Optimization for Prompt Tuning and Discovery**](https://doi.org/10.48550/arXiv.2302.03668) （**2023.02.07**）

![](https://img.shields.io/badge/Citations-2-green)  [![](https://img.shields.io/badge/Github%20Stars-433-blue)](https://github.com/YuxinWenRick/hard-prompts-made-easy)

[**Cap4Video: What Can Auxiliary Captions Do for Text-Video Retrieval?**](https://doi.org/10.48550/arXiv.2301.00184) （**2022.12.31**）

![](https://img.shields.io/badge/Citations-4-green)  [![](https://img.shields.io/badge/Github%20Stars-38-blue)](https://github.com/whwu95/Cap4Video)


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