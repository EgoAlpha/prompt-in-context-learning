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

*🎉[LLMs Usage Guide](./langchain_guide/LangChainTutorial_en.ipynb)🎉*: The method for quickly getting started with large language models by using LangChain.

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
- **[2023.9.18]**
    - Survey Paper: [The Rise and Potential of Large Language Model Based Agents: A Survey](https://arxiv.org/pdf/2309.07864.pdf)

- **[2023.9.17]**
    - Paper: [Textbooks Are All You Need II: phi-1.5 technical report](https://arxiv.org/abs/2309.05463)

- **[2023.9.16]**
    - Paper: [DOLA: DECODING BY CONTRASTING LAYERS IMPROVES FACTUALITY IN LARGE LANGUAGE MODELS](https://arxiv.org/pdf/2309.03883.pdf)

- **[2023.9.15]**
    - Microsoft Open Sources EvoDiff: A New Generation of Protein Generative AI : [\[Paper\]](https://doi.org/10.1101/2023.09.11.556673 )
    - Paper: [DePT: Decomposed Prompt Tuning for Parameter-Efficient Fine-tuning](https://arxiv.org/pdf/2309.05173v1.pdf)

- **[2023.9.14]**
    - Can LLMs Really Reason and Plan? | blog @ CACM | Communications of the ACM【[Paper](https://cacm.acm.org/blogs/blog-cacm/276268-can-llms-really-reason-and-plan/fulltext)/[Video](https://www.youtube.com/watch?v=BmyB-4S9QuY )】

- **[2023.9.13]**
    - Chinese multimodal large model VisCPM open API interface! The upgraded version is far more capable than similar models\([Paper](https://arxiv.org/pdf/2308.12038.pdf)/[Github](https://github.com/OpenBMB/VisCPM)\)
    - Survey Paper: [A Survey on Large Language Model based Autonomous Agents](https://arxiv.org/pdf/2308.11432v2.pdf)

- **[2023.9.12]**
    - Paper: [From Sparse to Dense: GPT-4 Summarization with Chain of Density Prompting](https://arxiv.org/abs/2309.04269)

- **[2023.9.11]**
    - Paper:[Narrator: Towards Natural Control of Human-Scene Interaction Generation via Relationship Reasoning](https://arxiv.org/pdf/2303.09410.pdf)

- **[2023.9.10]**
    - Survey Paper: [Siren's Song in the AI Ocean: A Survey on Hallucination in Large Language Models](https://arxiv.org/abs/2309.01219)

- **[2023.9.9]**
    - Open-source version of code interpreter tops GitHub hotlist, runs locally, accesses Internet: [\[Github\]](https://github.com/KillianLucas/open-interpreter/#commands)
    - Paper:[LARGE LANGUAGE MODELS AS OPTIMIZERS](https://arxiv.org/pdf/2309.03409.pdf)
    - Survey Paper:[RenAIssance: A Survey into AI Text-to-Image Generation in the Era of Large Model](https://arxiv.org/abs/2309.00810)

- **[2023.9.8]**
    - Paper:[Physically Grounded Vision-Language Models for Robotic Manipulation](https://arxiv.org/abs/2309.02561)

- **[2023.9.7]**
    - Baichuan Intelligence Releases Baichuan2 Big Model: Comprehensively Ahead of Llama2, Training Slices Also Open Source: [Github](https://github.com/baichuan-inc/Baichuan2)/[Technical Report](https://cdn.baichuan-ai.com/paper/Baichuan2-technical-report.pdf)

- **[2023.9.6]**
    - Paper: [TouchStone: Evaluating Vision-Language Models by Language Models](https://arxiv.org/abs/2308.16890)
    
- **[2023.9.5]**
    - [70 billion parameters Llama 2 training accelerated 195%! Training/fine-tuning/reasoning full-process program open source, 0 code one-stop solution!](https://github.com/hpcaitech/ColossalAI)

    - Survey Paper:[Large language models in medicine: the potentials and pitfalls](https://arxiv.org/abs/2309.00087)

- **[2023.9.4]**
    - Paper:[SeqGPT: An Out-of-the-box Large Language Model for Open Domain Sequence Understanding](https://arxiv.org/abs/2308.10529)

- **[2023.9.3]**
    - Paper:[PE-MED: Prompt Enhancement for Interactive Medical Image Segmentation](https://arxiv.org/pdf/2308.13746.pdf)

- **[2023.9.2]**
    - Paper: [SkipcrossNets: Adaptive Skip-cross Fusion for Road Detection](https://arxiv.org/pdf/2308.12863v1.pdf)

- **[2023.9.1]**
    - 8 LLM products are fully open to the whole community, including IOS and Android APP【[Baidu](https://yiyan.baidu.com), [百川智能](www.baichuan-ai.com), [SenseChat]( https://chat.sensetime.com), 智谱清言, ByteDance, INTERN, CAS, MiniMax】
    - Paper:[FQ-ViT: Post-Training Quantization for Fully Quantized Vision Transformer](https://arxiv.org/pdf/2111.13824.pdf)

[👉 Complete history news 👈](./historynews.md)

<img width="200%" src="./figures/hr.gif" />

---

# 📜 Papers

> You can directly click on the title to jump to the corresponding PDF link location

## Survey

<div style="line-height:0.2em;">


<div style="line-height:0.2em;">



[**Point-Bind&Point-LLM: Aligning Point Cloud with Multi-modality for 3D Understanding, Generation, and Instruction Following**](https://arxiv.org/abs/2309.00615) （**2023.09.01**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-7-red)  [![](https://img.shields.io/badge/Github%20Stars-110-blue)](https://github.com/ziyuguo99/point-bind_point-llm)

[**Large language models in medicine: the potentials and pitfalls**](https://arxiv.org/abs/2309.00087) （**2023.08.31**）

![](https://img.shields.io/badge/Citations-0-green)

[**Scientific discovery in the age of artificial intelligence**](https://doi.org/10.1038/s41586-023-06221-2) （**2023.08.01**）

![](https://img.shields.io/badge/Citations-7-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-141-red)

[**Foundational Models Defining a New Era in Vision: A Survey and Outlook**](https://doi.org/10.48550/arXiv.2307.13721) （**2023.07.25**）

![](https://img.shields.io/badge/Citations-3-green)  [![](https://img.shields.io/badge/Github%20Stars-260-blue)](https://github.com/awaisrauf/awesome-cv-foundational-models)


[**Challenges and Applications of Large Language Models**](https://doi.org/10.48550/arXiv.2307.10169) （**2023.07.19**）

![](https://img.shields.io/badge/Citations-0-green)

[**A Survey on Evaluation of Large Language Models**](https://doi.org/10.48550/arXiv.2307.03109) （**2023.07.06**）

![](https://img.shields.io/badge/Citations-25-green)  [![](https://img.shields.io/badge/Github%20Stars-776-blue)](https://github.com/mlgroupjlu/llm-eval-survey)

[**A Survey on Multimodal Large Language Models**](https://doi.org/10.48550/arXiv.2306.13549) （**2023.06.23**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-2.2k-blue)](https://github.com/bradyfu/awesome-multimodal-large-language-models)

[**Opportunities and Challenges for ChatGPT and Large Language Models in Biomedicine and Health**](https://doi.org/10.48550/arXiv.2306.10070) （**2023.06.15**）

![](https://img.shields.io/badge/Citations-4-green)


</div>

👉[Complete paper list 🔗 for "Survey"](./PaperList/survey.md)👈

## Prompt Engineering

### Prompt Design

<div style="line-height:0.2em;">



[**PE-MED: Prompt Enhancement for Interactive Medical Image Segmentation**](https://doi.org/10.48550/arXiv.2308.13746) （**2023.08.26**）

![](https://img.shields.io/badge/Citations-0-green)

[**SeqGPT: An Out-of-the-box Large Language Model for Open Domain Sequence Understanding**](https://doi.org/10.48550/arXiv.2308.10529) （**2023.08.21**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-66-blue)](https://github.com/alibaba-nlp/seqgpt)

[**Giraffe: Adventures in Expanding Context Lengths in LLMs**](https://doi.org/10.48550/arXiv.2308.10882) （**2023.08.21**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-454-blue)](https://github.com/abacusai/long-context)

[**Prompt Switch: Efficient CLIP Adaptation for Text-Video Retrieval**](https://doi.org/10.48550/arXiv.2308.07648) （**2023.08.15**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-4-blue)](https://github.com/bladewaltz1/promptswitch)

[**Exploring the Intersection of Large Language Models and Agent-Based Modeling via Prompt Engineering**](https://doi.org/10.48550/arXiv.2308.07411) （**2023.08.14**）

![](https://img.shields.io/badge/Citations-0-green)

[**AgentBench: Evaluating LLMs as Agents**](https://doi.org/10.48550/arXiv.2308.03688) （**2023.08.07**）

![](https://img.shields.io/badge/Citations-2-green)  [![](https://img.shields.io/badge/Github%20Stars-972-blue)](https://github.com/thudm/agentbench)

[**PromptCARE: Prompt Copyright Protection by Watermark Injection and Verification**](https://doi.org/10.48550/arXiv.2308.02816) （**2023.08.05**）

![](https://img.shields.io/badge/Citations-1-green)

[**AntGPT: Can Large Language Models Help Long-term Action Anticipation from Videos?**](https://doi.org/10.48550/arXiv.2307.16368) （**2023.07.31**）

![](https://img.shields.io/badge/Citations-0-green)

[**ChatSpot: Bootstrapping Multimodal LLMs via Precise Referring Instruction Tuning**](https://doi.org/10.48550/arXiv.2307.09474) （**2023.07.18**）

![](https://img.shields.io/badge/Citations-2-green)

[**Self-consistency for open-ended generations**](https://arxiv.org/abs/2307.06857) （**2023.07.11**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-5-red)


</div>

👉[Complete paper list 🔗 for "Prompt Design"](./PaperList/PromptDesignList.md)👈

### Automatic Prompt 

<div style="line-height:0.2em;">



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

[**Compress, Then Prompt: Improving Accuracy-Efficiency Trade-off of LLM Inference with Transferable Prompt**](https://doi.org/10.48550/arXiv.2305.11186) （**2023.05.17**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Automatic Prompt"](./PaperList/AutomaticPromptList.md)👈

### Chain of Thought

<div style="line-height:0.2em;">



[**Graph of Thoughts: Solving Elaborate Problems with Large Language Models**](https://doi.org/10.48550/arXiv.2308.09687) （**2023.08.18**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-1.1k-blue)](https://github.com/spcl/graph-of-thoughts)

[**Exploring the Intersection of Large Language Models and Agent-Based Modeling via Prompt Engineering**](https://doi.org/10.48550/arXiv.2308.07411) （**2023.08.14**）

![](https://img.shields.io/badge/Citations-0-green)

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

[**Tab-CoT: Zero-shot Tabular Chain of Thought**](https://doi.org/10.48550/arXiv.2305.17812) （**2023.05.28**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-17-blue)](https://github.com/xalp/tab-cot)

[**Beyond Chain-of-Thought, Effective Graph-of-Thought Reasoning in Large Language Models**](https://doi.org/10.48550/arXiv.2305.16582) （**2023.05.26**）

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

[**Eliciting the Translation Ability of Large Language Models via Multilingual Finetuning with Translation Instructions**](https://arxiv.org/abs/2305.15083) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-3-red)


</div>

👉[Complete paper list 🔗 for "Evaluation & Reliability"](./PaperList/EvaluationReliabilityList.md)👈

## In-context Learning

<div style="line-height:0.2em;">



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

[**OverPrompt: Enhancing ChatGPT Capabilities through an Efficient In-Context Learning Approach**](https://arxiv.org/abs/2305.14973) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-6-red)

[**Adversarial Demonstration Attacks on Large Language Models**](https://arxiv.org/abs/2305.14950) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-9-red)


</div>

👉[Complete paper list 🔗 for "In-context Learning"](./PaperList/InContextLearningList.md)👈

## Multimodal Prompt

<div style="line-height:0.2em;">



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

[**OBJECT 3DIT: Language-guided 3D-aware Image Editing**](https://doi.org/10.48550/arXiv.2307.11073) （**2023.07.20**）

![](https://img.shields.io/badge/Citations-0-green)

[**Brain2Music: Reconstructing Music from Human Brain Activity**](https://doi.org/10.48550/arXiv.2307.11078) （**2023.07.20**）

![](https://img.shields.io/badge/Citations-0-green)

[**(Ab)using Images and Sounds for Indirect Instruction Injection in Multi-Modal LLMs**](https://doi.org/10.48550/arXiv.2307.10490) （**2023.07.19**）

![](https://img.shields.io/badge/Citations-1-green)

[**HyperDreamBooth: HyperNetworks for Fast Personalization of Text-to-Image Models**](https://arxiv.org/abs/2307.06949) （**2023.07.13**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-41-red)


</div>

👉[Complete paper list 🔗 for "Multimodal Prompt"](./PaperList/multimodalprompt.md)👈

## Prompt Application

<div style="line-height:0.2em;">



[**PE-MED: Prompt Enhancement for Interactive Medical Image Segmentation**](https://doi.org/10.48550/arXiv.2308.13746) （**2023.08.26**）

![](https://img.shields.io/badge/Citations-0-green)

[**SeqGPT: An Out-of-the-box Large Language Model for Open Domain Sequence Understanding**](https://doi.org/10.48550/arXiv.2308.10529) （**2023.08.21**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-66-blue)](https://github.com/alibaba-nlp/seqgpt)

[**Giraffe: Adventures in Expanding Context Lengths in LLMs**](https://doi.org/10.48550/arXiv.2308.10882) （**2023.08.21**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-454-blue)](https://github.com/abacusai/long-context)

[**ExpeL: LLM Agents Are Experiential Learners**](https://doi.org/10.48550/arXiv.2308.10144) （**2023.08.20**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-6-blue)](https://github.com/Andrewzh112/ExpeL)

[**The Devil is in the Errors: Leveraging Large Language Models for Fine-grained Machine Translation Evaluation**](https://doi.org/10.48550/arXiv.2308.07286) （**2023.08.14**）

![](https://img.shields.io/badge/Citations-1-green)

[**Accelerating LLM Inference with Staged Speculative Decoding**](https://doi.org/10.48550/arXiv.2308.04623) （**2023.08.08**）

![](https://img.shields.io/badge/Citations-1-green)

[**Shepherd: A Critic for Language Model Generation**](https://doi.org/10.48550/arXiv.2308.04592) （**2023.08.08**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-160-blue)](https://github.com/facebookresearch/shepherd)

[**AgentBench: Evaluating LLMs as Agents**](https://doi.org/10.48550/arXiv.2308.03688) （**2023.08.07**）

![](https://img.shields.io/badge/Citations-2-green)  [![](https://img.shields.io/badge/Github%20Stars-972-blue)](https://github.com/thudm/agentbench)

[**Advancing Beyond Identification: Multi-bit Watermark for Language Models**](https://doi.org/10.48550/arXiv.2308.00221) （**2023.08.01**）

![](https://img.shields.io/badge/Citations-0-green)

[**AntGPT: Can Large Language Models Help Long-term Action Anticipation from Videos?**](https://doi.org/10.48550/arXiv.2307.16368) （**2023.07.31**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Prompt Application"](./PaperList/promptapplication.md)👈

## Foundation Models

<div style="line-height:0.2em;">



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

[**Pre-Trained Large Language Models for Industrial Control**](https://doi.org/10.48550/arXiv.2308.03028) （**2023.08.06**）

![](https://img.shields.io/badge/Citations-0-green)

[**FLatten Transformer: Vision Transformer using Focused Linear Attention**](https://doi.org/10.48550/arXiv.2308.00442) （**2023.08.01**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-134-blue)](https://github.com/leaplabthu/flatten-transformer)

[**AntGPT: Can Large Language Models Help Long-term Action Anticipation from Videos?**](https://doi.org/10.48550/arXiv.2307.16368) （**2023.07.31**）

![](https://img.shields.io/badge/Citations-0-green)


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