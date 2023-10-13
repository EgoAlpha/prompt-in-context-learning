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

- **[2023.10.13]**
    - Paper: [Ferret: Refer and Ground Anything Anywhere at Any Granularity](https://arxiv.org/abs/2310.07704)

- **[2023.10.12]**
    - Paper: [Understanding the Effects of RLHF on LLM Generalisation and Diversity](https://arxiv.org/abs/2310.06452 )
    - Paper: [Learning Interactive Real-World Simulators](https://arxiv.org/abs/2310.06114 )

- **[2023.10.11]**
    - Paper: [PB-LLM: Partially Binarized Large Language Models](https://arxiv.org/abs/2310.00034)

- **[2023.10.10]**
    - Paper: [MVDREAM:MULTI-VIEW DIFFUSION FOR 3D GENERATION](https://arxiv.org/pdf/2308.16512.pdf)

- **[2023.10.9]**
    - Paper: [MiniGPT-5: Interleaved Vision-and-Language Generation via Generative Vokens](https://arxiv.org/pdf/2310.02239v2.pdf)

- **[2023.10.8]**
    - Paper: [Distilling Step-by-Step! Outperforming Larger Language Models with Less Training Data and Smaller Model Sizes](https://arxiv.org/abs/2305.02301)

- **[2023.10.7]**
    - Survey Paper: [A Survey of Chain of Thought Reasoning: Advances, Frontiers and Future](https://arxiv.org/abs/2309.15402)

- **[2023.10.6]**
    - Paper: [Language Models Represent Space and Time](https://arxiv.org/abs/2310.02207)

- **[2023.10.5]**
    - Paper: [Adapting Large Language Models via Reading Comprehension](https://arxiv.org/abs/2309.09530)

- **[2023.10.4]**
    - Paper: [LongLoRA: Efficient Fine-tuning of Long-Context Large Language Models](https://arxiv.org/abs/2309.12307)

- **[2023.10.3]**
    - Paper: [CHAIN-OF-VERIFICATION REDUCES HALLUCINATION IN LARGE LANGUAGE MODELS](https://arxiv.org/pdf/2309.11495)

- **[2023.10.2]**
    - Paper: [DreamLLM: Synergistic Multimodal Comprehension and Creation](https://arxiv.org/abs/2309.11499)

- **[2023.10.1]**
    - Paper: [Investigating the Catastrophic Forgetting in Multimodal Large Language Models](https://arxiv.org/abs/2309.10313)

[👉 Complete history news 👈](./historynews.md)

<img width="200%" src="./figures/hr.gif" />

---

# 📜 Papers

> You can directly click on the title to jump to the corresponding PDF link location

## Survey

<div style="line-height:0.2em;">


<div style="line-height:0.2em;">



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

[**A Survey on Large Language Model based Autonomous Agents**](https://doi.org/10.48550/arXiv.2308.11432) （**2023.08.22**）

![](https://img.shields.io/badge/Citations-13-green)  [![](https://img.shields.io/badge/Github%20Stars-1.1k-blue)](https://github.com/paitesanshi/llm-agent-survey)

[**Instruction Tuning for Large Language Models: A Survey**](https://doi.org/10.48550/arXiv.2308.10792) （**2023.08.21**）

![](https://img.shields.io/badge/Citations-7-green)  [![](https://img.shields.io/badge/Github%20Stars-9-blue)](https://github.com/xiaoya-li/instruction-tuning-survey)

[**Scientific discovery in the age of artificial intelligence**](https://doi.org/10.1038/s41586-023-06221-2) （**2023.08.01**）

![](https://img.shields.io/badge/Citations-7-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-141-red)

[**Foundational Models Defining a New Era in Vision: A Survey and Outlook**](https://doi.org/10.48550/arXiv.2307.13721) （**2023.07.25**）

![](https://img.shields.io/badge/Citations-3-green)  [![](https://img.shields.io/badge/Github%20Stars-260-blue)](https://github.com/awaisrauf/awesome-cv-foundational-models)

[**Foundational Models Defining a New Era in Vision: A Survey and Outlook**](https://arxiv.org/abs/2307.13721) （**2023.07.25**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Survey"](./PaperList/survey.md)👈

## Prompt Engineering

### Prompt Design

<div style="line-height:0.2em;">



[**LongLoRA: Efficient Fine-tuning of Long-Context Large Language Models**](https://doi.org/10.48550/arXiv.2309.12307) （**2023.09.21**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-1.2k-blue)](https://github.com/dvlab-research/longlora)

[**Chain-of-Verification Reduces Hallucination in Large Language Models**](https://doi.org/10.48550/arXiv.2309.11495) （**2023.09.20**）

![](https://img.shields.io/badge/Citations-3-green)

[**End-to-End Speech Recognition Contextualization with Large Language Models**](https://doi.org/10.48550/arXiv.2309.10917) （**2023.09.19**）

![](https://img.shields.io/badge/Citations-0-green)

[**PoSE: Efficient Context Window Extension of LLMs via Positional Skip-wise Training**](https://doi.org/10.48550/arXiv.2309.10400) （**2023.09.19**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-54-blue)](https://github.com/dwzhu-pku/pose)

[**DePT: Decomposed Prompt Tuning for Parameter-Efficient Fine-tuning**](https://doi.org/10.48550/arXiv.2309.05173) （**2023.09.11**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-27-blue)](https://github.com/zhengxiangshi/dept)

[**PE-MED: Prompt Enhancement for Interactive Medical Image Segmentation**](https://doi.org/10.48550/arXiv.2308.13746) （**2023.08.26**）

![](https://img.shields.io/badge/Citations-0-green)

[**ReLLa: Retrieval-enhanced Large Language Models for Lifelong Sequential Behavior Comprehension in Recommendation**](https://doi.org/10.48550/arXiv.2308.11131) （**2023.08.22**）

![](https://img.shields.io/badge/Citations-1-green)

[**SeqGPT: An Out-of-the-box Large Language Model for Open Domain Sequence Understanding**](https://doi.org/10.48550/arXiv.2308.10529) （**2023.08.21**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-66-blue)](https://github.com/alibaba-nlp/seqgpt)

[**Giraffe: Adventures in Expanding Context Lengths in LLMs**](https://doi.org/10.48550/arXiv.2308.10882) （**2023.08.21**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-454-blue)](https://github.com/abacusai/long-context)

[**Prompt Switch: Efficient CLIP Adaptation for Text-Video Retrieval**](https://doi.org/10.48550/arXiv.2308.07648) （**2023.08.15**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-4-blue)](https://github.com/bladewaltz1/promptswitch)


</div>

👉[Complete paper list 🔗 for "Prompt Design"](./PaperList/PromptDesignList.md)👈

### Automatic Prompt 

<div style="line-height:0.2em;">



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

[**Learning Easily Updated General Purpose Text Representations with Adaptable Task-Specific Prefixes**](https://arxiv.org/abs/2305.13499) （**2023.05.22**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)

[**Automated Few-shot Classification with Instruction-Finetuned Language Models**](https://arxiv.org/abs/2305.12576) （**2023.05.21**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-4-red)  [![](https://img.shields.io/badge/Github%20Stars-4-blue)](https://github.com/raldir/aut-few)

[**AutoTrial: Prompting Language Models for Clinical Trial Design**](https://doi.org/10.48550/arXiv.2305.11366) （**2023.05.19**）

![](https://img.shields.io/badge/Citations-0-green)

[**Flatness-Aware Prompt Selection Improves Accuracy and Sample Efficiency**](https://doi.org/10.48550/arXiv.2305.10713) （**2023.05.18**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-6-blue)](https://github.com/shadowkiller33/flatness)


</div>

👉[Complete paper list 🔗 for "Automatic Prompt"](./PaperList/AutomaticPromptList.md)👈

### Chain of Thought

<div style="line-height:0.2em;">



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

[**Strategic Reasoning with Language Models**](https://doi.org/10.48550/arXiv.2305.19165) （**2023.05.30**）

![](https://img.shields.io/badge/Citations-0-green)

[**Code Prompting: a Neural Symbolic Method for Complex Reasoning in Large Language Models**](https://doi.org/10.48550/arXiv.2305.18507) （**2023.05.29**）

![](https://img.shields.io/badge/Citations-0-green)

[**Leveraging Training Data in Few-Shot Prompting for Numerical Reasoning**](https://doi.org/10.48550/arXiv.2305.18170) （**2023.05.29**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-5-blue)](https://github.com/allanj/dynamic-pal)


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

[**Learning to Retrieve In-Context Examples for Large Language Models**](https://arxiv.org/abs/2307.07164) （**2023.07.14**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-11-red)

[**Schema-learning and rebinding as mechanisms of in-context learning and emergence**](https://doi.org/10.48550/arXiv.2307.01201) （**2023.06.16**）

![](https://img.shields.io/badge/Citations-0-green)

[**MetaVL: Transferring In-Context Learning Ability From Language Models to Vision-Language Models**](https://doi.org/10.48550/arXiv.2306.01311) （**2023.06.02**）

![](https://img.shields.io/badge/Citations-0-green)

[**Measuring and Mitigating Constraint Violations of In-Context Learning for Utterance-to-API Semantic Parsing**](https://arxiv.org/abs/2305.15338) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)


</div>

👉[Complete paper list 🔗 for "In-context Learning"](./PaperList/InContextLearningList.md)👈

## Multimodal Prompt

<div style="line-height:0.2em;">



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

[**UniVTG: Towards Unified Video-Language Temporal Grounding**](https://doi.org/10.48550/arXiv.2307.16715) （**2023.07.31**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-162-blue)](https://github.com/showlab/univtg)

[**Med-Flamingo: a Multimodal Medical Few-shot Learner**](https://doi.org/10.48550/arXiv.2307.15189) （**2023.07.27**）

![](https://img.shields.io/badge/Citations-3-green)  [![](https://img.shields.io/badge/Github%20Stars-253-blue)](https://github.com/snap-stanford/med-flamingo)


</div>

👉[Complete paper list 🔗 for "Multimodal Prompt"](./PaperList/multimodalprompt.md)👈

## Prompt Application

<div style="line-height:0.2em;">



[**Chain-of-Verification Reduces Hallucination in Large Language Models**](https://doi.org/10.48550/arXiv.2309.11495) （**2023.09.20**）

![](https://img.shields.io/badge/Citations-3-green)

[**Kosmos-2.5: A Multimodal Literate Model**](https://doi.org/10.48550/arXiv.2309.11419) （**2023.09.20**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-10-blue)](https://github.com/kyegomez/Kosmos2.5)

[**DreamLLM: Synergistic Multimodal Comprehension and Creation**](https://doi.org/10.48550/arXiv.2309.11499) （**2023.09.20**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-185-blue)](https://github.com/RunpeiDong/DreamLLM)

[**SwitchGPT: Adapting Large Language Models for Non-Text Outputs**](https://doi.org/10.48550/arXiv.2309.07623) （**2023.09.14**）

![](https://img.shields.io/badge/Citations-0-green)

[**NExT-GPT: Any-to-Any Multimodal LLM**](https://doi.org/10.48550/arXiv.2309.05519) （**2023.09.11**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-1.9k-blue)](https://github.com/NExT-GPT/NExT-GPT)

[**From Sparse to Dense: GPT-4 Summarization with Chain of Density Prompting**](https://doi.org/10.48550/arXiv.2309.04269) （**2023.09.08**）

![](https://img.shields.io/badge/Citations-0-green)

[**Large Language Models as Optimizers**](https://arxiv.org/abs/2309.03409) （**2023.09.07**）

![](https://img.shields.io/badge/Citations-0-green)

[**DoLa: Decoding by Contrasting Layers Improves Factuality in Large Language Models**](https://doi.org/10.48550/arXiv.2309.03883) （**2023.09.07**）

![](https://img.shields.io/badge/Citations-3-green)  [![](https://img.shields.io/badge/Github%20Stars-184-blue)](https://github.com/voidism/dola)

[**YaRN: Efficient Context Window Extension of Large Language Models**](https://doi.org/10.48550/arXiv.2309.00071) （**2023.08.31**）

![](https://img.shields.io/badge/Citations-7-green)  [![](https://img.shields.io/badge/Github%20Stars-655-blue)](https://github.com/jquesnelle/yarn)

[**PE-MED: Prompt Enhancement for Interactive Medical Image Segmentation**](https://doi.org/10.48550/arXiv.2308.13746) （**2023.08.26**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Prompt Application"](./PaperList/promptapplication.md)👈

## Foundation Models

<div style="line-height:0.2em;">



[**Q-Transformer: Scalable Offline Reinforcement Learning via Autoregressive Q-Functions**](https://doi.org/10.48550/arXiv.2309.10150) （**2023.09.18**）

![](https://img.shields.io/badge/Citations-1-green)

[**Replacing softmax with ReLU in Vision Transformers**](https://doi.org/10.48550/arXiv.2309.08586) （**2023.09.15**）

![](https://img.shields.io/badge/Citations-1-green)

[**ZGaming: Zero-Latency 3D Cloud Gaming by Image Prediction**](https://doi.org/10.1145/3603269.3604819) （**2023.09.01**）

![](https://img.shields.io/badge/Citations-0-green)

[**PE-MED: Prompt Enhancement for Interactive Medical Image Segmentation**](https://doi.org/10.48550/arXiv.2308.13746) （**2023.08.26**）

![](https://img.shields.io/badge/Citations-0-green)

[**SkipcrossNets: Adaptive Skip-cross Fusion for Road Detection**](https://doi.org/10.48550/arXiv.2308.12863) （**2023.08.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**SeqGPT: An Out-of-the-box Large Language Model for Open Domain Sequence Understanding**](https://doi.org/10.48550/arXiv.2308.10529) （**2023.08.21**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-66-blue)](https://github.com/alibaba-nlp/seqgpt)

[**Prompt Switch: Efficient CLIP Adaptation for Text-Video Retrieval**](https://doi.org/10.48550/arXiv.2308.07648) （**2023.08.15**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-4-blue)](https://github.com/bladewaltz1/promptswitch)

[**VisIT-Bench: A Benchmark for Vision-Language Instruction Following Inspired by Real-World Use**](https://doi.org/10.48550/arXiv.2308.06595) （**2023.08.12**）

![](https://img.shields.io/badge/Citations-1-green)

[**Accelerating LLM Inference with Staged Speculative Decoding**](https://doi.org/10.48550/arXiv.2308.04623) （**2023.08.08**）

![](https://img.shields.io/badge/Citations-1-green)

[**Food-500 Cap: A Fine-Grained Food Caption Benchmark for Evaluating Vision-Language Models**](https://doi.org/10.48550/arXiv.2308.03151) （**2023.08.06**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-2-blue)](https://github.com/aaronma2020/Food500-Cap)


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