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

<h4 align="center">
    <p>
        <a href="./README.md">English</a> |
        <a href="./chatgptprompt_zh.md">简体中文</a>
    <p>
</h4>

<p align="center">

  <a href="#📜-papers">📝 Papers</a> |
  <a href="./Playground.md">⚡️  Playground</a> |
  <a href="./PromptEngineering.md">🛠 Prompt Engineering</a> |
  <a href="./chatgptprompt.md">🌍 ChatGPT Prompt</a> 

</p>

</div>

<div align="center">

<!-- ![Build](https://img.shields.io/appveyor/build/gruntjs/grunt) -->

![version](https://img.shields.io/badge/version-v1.0.0-blue)
![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)

<!-- ![license](https://img.shields.io/bower/l/bootstrap?style=plastic) -->

</div>

> **⭐️ Shining ⭐️:** This is fresh, daily-updated resources for in-context learning and prompt engineering. As Artificial General Intelligence (AGI) is approaching, let’s take action and become a super learner so as to position ourselves at the forefront of this exciting era and strive for personal and professional greatness.

The resources include:

*🎉[Papers](#📜-papers)🎉*:  The latest papers about in-context learning or prompt engineering. 

*🎉[Playground](./Playground.md)🎉*:  Large language models that enable prompt experimentation. 

*🎉[Prompt Engineering](./PromptEngineering.md)🎉*: Prompt techniques for leveraging large language models. 

*🎉[ChatGPT Prompt](./chatgptprompt.md)🎉*: Prompt examples that can be applied in our work and daily lives. 

In the future, there will likely be two types of people on Earth (perhaps even on Mars, but that's a question for Musk): 
- Those who enhance their abilities through the use of AI; 
- Those whose jobs are replaced by AI automation.

```

💎EgoAlpha: Hello! human👤, are you ready?

```  

# 📢 News
<!-- 🔥🔥🔥 -->
☄️ **EgoAlpha releases the TrustGPT focuses on reasoning. Trust the GPT with the strongest reasoning abilities for authentic and reliable answers. You can click [here](https://trustgpt.co) or visit the [Playgrounds](./Playground.md) directly to experience it。**

- **[2023.5.16]**
    - Paper:[MEGABYTE: Predicting Million-byte Sequences with Multiscale Transformers](https://arxiv.org/pdf/2305.07185.pdf)

- **[2023.5.15]** 
    - Paper: [ArtGPT-4: Artistic Vision-Language Understanding with Adapter-enhanced MiniGPT-4](https://arxiv.org/pdf/2305.07490.pdf)
    
- **[2023.5.14]**
    - Paper: [Distilling Step-by-Step! Outperforming Larger Language Models with Less Training Data and Smaller Model Sizes](https://arxiv.org/pdf/2305.02301v1.pdf)

- **[2023.5.13]**
    - Paper: [VPGTrans: Transfer Visual Prompt Generator across LLMs](https://arxiv.org/pdf/2305.01278.pdf)

- **[2023.5.12]**
    - Paper: [Cap4Video: What Can Auxiliary Captions Do for Text-Video Retrieval?](https://arxiv.org/abs/2301.00184)
    
- **[2023.5.11]**
    - Google has released PaLM 2, which improves multiple abilities and offers four versions for selection. ([Paper](https://event-cdn.baai.ac.cn/file/file-browser/KDtjMkep6E6n5XjRNJjknjewCF7Pcebx.pdf)/[Page](https://makersuite.google.com/waitlist ))
    - [The open-source healthcare large language model NHS-LLM and OpenGPT.](https://github.com/CogStack/opengpt)

    - Paper: [Language models can explain neurons in language models](https://openaipublic.blob.core.windows.net/neuron-explainer/paper/index.html)

- **[2023.5.10]** 
    - DetGPT: Detect What You Need via Reasoning ([Code](https://github.com/OptimalScale/DetGPT)/[Demo](https://detgpt.github.io/))

    - Meta releases a large-scale model called ImageBind that can traverse six senses, and it is now open-source. ([Paper](https://ai.facebook.com/blog/imagebind-six-modalities-binding-ai/)/[Code](https://github.com/facebookresearch/ImageBind))

    - [HuoTuo: Open Source Chinese Medical Large Model of Harbin Institute of Technology](https://github.com/SCIR-HI/Huatuo-Llama-Med-Chinese)

    - Paper: [X-LLM: Bootstrapping Advanced Large Language Models by Treating Multi-Modalities as Foreign Languages](https://arxiv.org/pdf/2305.04160.pdf)

- **[2023.5.9]**

    - Paper: [Transfer Visual Prompt Generator across LLMs](https://arxiv.org/abs/2305.01278) 【[Code](https://github.com/VPGTrans/VPGTrans)】

- **[2023.5.8]**
    - PandaLM: the first large model for automated evaluation.([Code](https://github.com/WeOpenML/PandaLM))
    
    - Paper:[AutoML-GPT: Automatic Machine Learning with GPT](https://arxiv.org/abs/2305.02499)

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



[**Harnessing the Power of LLMs in Practice: A Survey on ChatGPT and Beyond**](https://arxiv.org/abs/2304.13712) （**2023.04.26**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-59-red)  [![](https://img.shields.io/badge/Github%20Stars-1.8k-blue)](https://github.com/mooler0410/llmspracticalguide)

[**A Survey of Large Language Models**](https://arxiv.org/abs/2303.18223) （**2023.03.31**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-353-red)  [![](https://img.shields.io/badge/Github%20Stars-1.0k-blue)](https://github.com/rucaibox/llmsurvey)

[**Augmented Language Models: a Survey**](https://doi.org/10.48550/arXiv.2302.07842) （**2023.02.15**）

![](https://img.shields.io/badge/Citations-4-green)

[**A Survey for In-context Learning**](https://doi.org/10.48550/arXiv.2301.00234) （**2022.12.31**）

![](https://img.shields.io/badge/Citations-0-green)

[**Towards Reasoning in Large Language Models: A Survey**](https://doi.org/10.48550/arXiv.2212.10403) （**2022.12.20**）

![](https://img.shields.io/badge/Citations-5-green)  [![](https://img.shields.io/badge/Github%20Stars-257-blue)](https://github.com/jeffhj/lm-reasoning)

[**Reasoning with Language Model Prompting: A Survey**](https://doi.org/10.48550/arXiv.2212.09597) （**2022.12.19**）

![](https://img.shields.io/badge/Citations-7-green)  [![](https://img.shields.io/badge/Github%20Stars-292-blue)](https://github.com/zjunlp/Prompt4ReasoningPapers)

[**Emergent Abilities of Large Language Models**](https://doi.org/10.48550/arXiv.2206.07682) （**2022.06.15**）

![](https://img.shields.io/badge/Citations-156-green)

[**Pre-train, Prompt, and Predict: A Systematic Survey of Prompting Methods in Natural Language Processing**](https://doi.org/10.1145/3560815) （**2021.07.28**）

![](https://img.shields.io/badge/Citations-462-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1.5k-red)  [![](https://img.shields.io/badge/Github%20Stars-190-blue)](https://github.com/mingkaid/rl-prompt)


</div>

👉[Complete paper list 🔗 for "Survey"](./PaperList/survey.md)👈

## Prompt Engineering

### Prompt Design

<div style="line-height:0.2em;">



[**WizardLM: Empowering Large Language Models to Follow Complex Instructions**](https://arxiv.org/abs/2304.12244) （**2023.04.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-15-red)  [![](https://img.shields.io/badge/Github%20Stars-913-blue)](https://github.com/nlpxucan/wizardlm)

[**LLM+P: Empowering Large Language Models with Optimal Planning Proficiency**](https://arxiv.org/abs/2304.11477) （**2023.04.22**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-6-red)  [![](https://img.shields.io/badge/Github%20Stars-93-blue)](https://github.com/Cranial-XIX/llm-pddl)

[**Progressive-Hint Prompting Improves Reasoning in Large Language Models**](https://arxiv.org/abs/2304.09797) （**2023.04.19**）

![](https://img.shields.io/badge/Citations-1-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-14-red)  [![](https://img.shields.io/badge/Github%20Stars-15-blue)](https://github.com/chuanyang-Zheng/Progressive-Hint)

[**Boosted Prompt Ensembles for Large Language Models**](https://doi.org/10.48550/arXiv.2304.05970) （**2023.04.12**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-16-blue)](https://github.com/awwang10/llmpromptboosting)

[**Prompt Pre-Training with Twenty-Thousand Classes for Open-Vocabulary Visual Recognition**](https://arxiv.org/abs/2304.04704) （**2023.04.10**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-18-red)  [![](https://img.shields.io/badge/Github%20Stars-165-blue)](https://github.com/amazon-science/prompt-pretraining)

[**REFINER: Reasoning Feedback on Intermediate Representations**](https://arxiv.org/abs/2304.01904) （**2023.04.04**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-13-red)  [![](https://img.shields.io/badge/Github%20Stars-28-blue)](https://github.com/debjitpaul/refiner)

[**Context-faithful Prompting for Large Language Models**](https://doi.org/10.48550/arXiv.2303.11315) （**2023.03.20**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-15-blue)](https://github.com/wzhouad/context-faithful-llm)

[**Reflexion: an autonomous agent with dynamic memory and self-reflection**](https://doi.org/10.48550/arXiv.2303.11366) （**2023.03.20**）

![](https://img.shields.io/badge/Citations-4-green)  [![](https://img.shields.io/badge/Github%20Stars-331-blue)](https://github.com/noahshinn024/reflexion)

[**A Prompt Pattern Catalog to Enhance Prompt Engineering with ChatGPT**](https://doi.org/10.48550/arXiv.2302.11382) （**2023.02.21**）

![](https://img.shields.io/badge/Citations-3-green)

[**GraphPrompt: Unifying Pre-Training and Downstream Tasks for Graph Neural Networks**](https://doi.org/10.48550/arXiv.2302.08043) （**2023.02.16**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Prompt Design"](./PaperList/PromptDesignList.md)👈

### Automatic Prompt 

<div style="line-height:0.2em;">



[**Automatic Prompt Augmentation and Selection with Chain-of-Thought from Labeled Data**](https://doi.org/10.48550/arXiv.2302.12822) （**2023.02.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Guiding Large Language Models via Directional Stimulus Prompting**](https://doi.org/10.48550/arXiv.2302.11520) （**2023.02.22**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-8-blue)](https://github.com/leezekun/directional-stimulus-prompting)

[**Evaluating the Robustness of Discrete Prompts**](https://doi.org/10.48550/arXiv.2302.05619) （**2023.02.11**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-3-blue)](https://github.com/livnlp/prompt-robustness)

[**Hard Prompts Made Easy: Gradient-Based Discrete Optimization for Prompt Tuning and Discovery**](https://doi.org/10.48550/arXiv.2302.03668) （**2023.02.07**）

![](https://img.shields.io/badge/Citations-2-green)  [![](https://img.shields.io/badge/Github%20Stars-398-blue)](https://github.com/YuxinWenRick/hard-prompts-made-easy)

[**Ask Me Anything: A simple strategy for prompting language models**](https://doi.org/10.48550/arXiv.2210.02441) （**2022.10.05**）

![](https://img.shields.io/badge/Citations-14-green)  [![](https://img.shields.io/badge/Github%20Stars-435-blue)](https://github.com/hazyresearch/ama_prompting)

[**STaR: Bootstrapping Reasoning With Reasoning**](https://doi.org/10.48550/arXiv.2203.14465) （**2022.03.28**）

![](https://img.shields.io/badge/Citations-56-green)  [![](https://img.shields.io/badge/Github%20Stars-14-blue)](https://github.com/ezelikman/STaR)

[**Making Pre-trained Language Models Better Few-shot Learners**](https://doi.org/10.18653/v1/2021.acl-long.295) （**2021.01.01**）

![](https://img.shields.io/badge/Citations-648-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-730-red)  [![](https://img.shields.io/badge/Github%20Stars-654-blue)](https://github.com/princeton-nlp/LM-BFF)

[**Eliciting Knowledge from Language Models Using Automatically Generated Prompts**](https://doi.org/10.18653/v1/2020.emnlp-main.346) （**2020.10.29**）

![](https://img.shields.io/badge/Citations-137-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-503-red)

[**Automatically Identifying Words That Can Serve as Labels for Few-Shot Text Classification**](https://doi.org/10.5282/UBM/EPUB.74034) （**2020.10.26**）

![](https://img.shields.io/badge/Citations-85-green)  [![](https://img.shields.io/badge/Github%20Stars-1.5k-blue)](https://github.com/timoschick/pet)


</div>

👉[Complete paper list 🔗 for "Automatic Prompt"](./PaperList/AutomaticPromptList.md)👈

### Chain of Thought

<div style="line-height:0.2em;">



[**Enhancing Chain-of-Thoughts Prompting with Iterative Bootstrapping in Large Language Models**](https://arxiv.org/abs/2304.11657) （**2023.04.23**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-15-red)  [![](https://img.shields.io/badge/Github%20Stars-47-blue)](https://github.com/gasolsun36/iter-cot)

[**Chain of Thought Prompt Tuning in Vision Language Models**](https://arxiv.org/abs/2304.07919) （**2023.04.16**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-13-red)

[**Investigating Chain-of-thought with ChatGPT for Stance Detection on Social Media**](https://doi.org/10.48550/arXiv.2304.03087) （**2023.04.06**）

![](https://img.shields.io/badge/Citations-0-green)

[**Automatic Prompt Augmentation and Selection with Chain-of-Thought from Labeled Data**](https://doi.org/10.48550/arXiv.2302.12822) （**2023.02.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Active Prompting with Chain-of-Thought for Large Language Models**](https://doi.org/10.48550/arXiv.2302.12246) （**2023.02.23**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-93-blue)](https://github.com/shizhediao/active-cot)

[**Multimodal Chain-of-Thought Reasoning in Language Models**](https://doi.org/10.48550/arXiv.2302.00923) （**2023.02.02**）

![](https://img.shields.io/badge/Citations-6-green)  [![](https://img.shields.io/badge/Github%20Stars-3.3k-blue)](https://github.com/amazon-science/mm-cot)

[**Synthetic Prompting: Generating Chain-of-Thought Demonstrations for Large Language Models**](https://doi.org/10.48550/arXiv.2302.00618) （**2023.02.01**）

![](https://img.shields.io/badge/Citations-2-green)

[**Faithful Chain-of-Thought Reasoning**](https://doi.org/10.48550/arXiv.2301.13379) （**2023.01.31**）

![](https://img.shields.io/badge/Citations-3-green)  [![](https://img.shields.io/badge/Github%20Stars-46-blue)](https://github.com/veronica320/faithful-cot)

[**Large Language Models Are Reasoning Teachers**](https://doi.org/10.48550/arXiv.2212.10071) （**2022.12.20**）

![](https://img.shields.io/badge/Citations-5-green)

[**Solving math word problems with process- and outcome-based feedback**](https://doi.org/10.48550/arXiv.2211.14275) （**2022.11.25**）

![](https://img.shields.io/badge/Citations-3-green)


</div>

👉[Complete paper list 🔗 for "Chain of Thought"](./PaperList/ChainofThoughtList.md)👈

### Knowledge Augmented Prompt

<div style="line-height:0.2em;">



[**LasUIE: Unifying Information Extraction with Latent Adaptive Structure-aware Generative Language Model**](https://arxiv.org/abs/2304.06248) （**2023.04.13**）

![](https://img.shields.io/badge/Citations-2-green)  [![](https://img.shields.io/badge/Github%20Stars-20-blue)](https://github.com/chocowu/lasuie)

[**Commonsense-Aware Prompting for Controllable Empathetic Dialogue Generation**](https://doi.org/10.48550/arXiv.2302.01441) （**2023.02.02**）

![](https://img.shields.io/badge/Citations-0-green)

[**REPLUG: Retrieval-Augmented Black-Box Language Models**](https://doi.org/10.48550/arXiv.2301.12652) （**2023.01.30**）

![](https://img.shields.io/badge/Citations-3-green)

[**Self-Instruct: Aligning Language Model with Self Generated Instructions**](https://doi.org/10.48550/arXiv.2212.10560) （**2022.12.20**）

![](https://img.shields.io/badge/Citations-9-green)  [![](https://img.shields.io/badge/Github%20Stars-2.0k-blue)](https://github.com/yizhongw/self-instruct)

[**One Embedder, Any Task: Instruction-Finetuned Text Embeddings**](https://doi.org/10.48550/arXiv.2212.09741) （**2022.12.19**）

![](https://img.shields.io/badge/Citations-2-green)  [![](https://img.shields.io/badge/Github%20Stars-443-blue)](https://github.com/HKUNLP/instructor-embedding)

[**The Impact of Symbolic Representations on In-context Learning for Few-shot Reasoning**](https://doi.org/10.48550/arXiv.2212.08686) （**2022.12.16**）

![](https://img.shields.io/badge/Citations-2-green)  [![](https://img.shields.io/badge/Github%20Stars-1-blue)](https://github.com/hlzhang109/lmlp)

[**Don’t Prompt, Search! Mining-based Zero-Shot Learning with Language Models**](https://doi.org/10.48550/arXiv.2210.14803) （**2022.10.26**）

![](https://img.shields.io/badge/Citations-1-green)

[**Knowledge Prompting in Pre-trained Language Model for Natural Language Understanding**](https://doi.org/10.48550/arXiv.2210.08536) （**2022.10.16**）

![](https://img.shields.io/badge/Citations-2-green)  [![](https://img.shields.io/badge/Github%20Stars-10-blue)](https://github.com/wjn1996/kp-plm)

[**Knowledge Injected Prompt Based Fine-tuning for Multi-label Few-shot ICD Coding**](https://doi.org/10.48550/arXiv.2210.03304) （**2022.10.07**）

![](https://img.shields.io/badge/Citations-2-green)  [![](https://img.shields.io/badge/Github%20Stars-27-blue)](https://github.com/whaleloops/KEPT)

[**Promptagator: Few-shot Dense Retrieval From 8 Examples**](https://doi.org/10.48550/arXiv.2209.11755) （**2022.09.23**）

![](https://img.shields.io/badge/Citations-16-green)


</div>

👉[Complete paper list 🔗 for "Knowledge Augmented Prompt"](./PaperList/KnowledgeAugmentedPromptList.md)👈


### Evaluation & Reliability

<div style="line-height:0.2em;">



[**AGIEval: A Human-Centric Benchmark for Evaluating Foundation Models**](https://arxiv.org/abs/2304.06364) （**2023.04.13**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-25-red)  [![](https://img.shields.io/badge/Github%20Stars-215-blue)](https://github.com/microsoft/agieval)

[**GPTEval: NLG Evaluation using GPT-4 with Better Human Alignment**](https://arxiv.org/abs/2303.16634) （**2023.03.29**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-39-red)

[**How Robust is GPT-3.5 to Predecessors? A Comprehensive Study on Language Understanding Tasks**](https://doi.org/10.48550/arXiv.2303.00293) （**2023.03.01**）

![](https://img.shields.io/badge/Citations-0-green)

[**Bounding the Capabilities of Large Language Models in Open Text Generation with Prompt Constraints**](https://doi.org/10.48550/arXiv.2302.09185) （**2023.02.17**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-20-blue)](https://github.com/salt-nlp/bound-cap-llm)

[**Evaluating the Robustness of Discrete Prompts**](https://doi.org/10.48550/arXiv.2302.05619) （**2023.02.11**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-3-blue)](https://github.com/livnlp/prompt-robustness)

[**Controlling for Stereotypes in Multimodal Language Model Evaluation**](https://doi.org/10.48550/arXiv.2302.01582) （**2023.02.03**）

![](https://img.shields.io/badge/Citations-0-green)

[**Large Language Models Can Be Easily Distracted by Irrelevant Context**](https://doi.org/10.48550/arXiv.2302.00093) （**2023.01.31**）

![](https://img.shields.io/badge/Citations-3-green)  [![](https://img.shields.io/badge/Github%20Stars-11-blue)](https://github.com/google-research-datasets/gsm-ic)

[**Emergent Analogical Reasoning in Large Language Models**](https://doi.org/10.48550/arXiv.2212.09196) （**2022.12.19**）

![](https://img.shields.io/badge/Citations-5-green)  [![](https://img.shields.io/badge/Github%20Stars-14-blue)](https://github.com/taylorwwebb/emergent_analogies_llm)

[**Discovering Language Model Behaviors with Model-Written Evaluations**](https://doi.org/10.48550/arXiv.2212.09251) （**2022.12.19**）

![](https://img.shields.io/badge/Citations-8-green)  [![](https://img.shields.io/badge/Github%20Stars-131-blue)](https://github.com/anthropics/evals)

[**Constitutional AI: Harmlessness from AI Feedback**](https://doi.org/10.48550/arXiv.2212.08073) （**2022.12.15**）

![](https://img.shields.io/badge/Citations-21-green)  [![](https://img.shields.io/badge/Github%20Stars-92-blue)](https://github.com/anthropics/constitutionalharmlessnesspaper)


</div>

👉[Complete paper list 🔗 for "Evaluation & Reliability"](./PaperList/EvaluationReliabilityList.md)👈

## In-context Learning

<div style="line-height:0.2em;">



[**Self-Refine: Iterative Refinement with Self-Feedback**](https://arxiv.org/abs/2303.17651) （**2023.03.30**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-50-red)  [![](https://img.shields.io/badge/Github%20Stars-209-blue)](https://github.com/madaan/self-refine)

[**Larger language models do in-context learning differently**](https://doi.org/10.48550/arXiv.2303.03846) （**2023.03.07**）

![](https://img.shields.io/badge/Citations-2-green)

[**Language Model Crossover: Variation through Few-Shot Prompting**](https://doi.org/10.48550/arXiv.2302.12170) （**2023.02.23**）

![](https://img.shields.io/badge/Citations-1-green)

[**How Does In-Context Learning Help Prompt Tuning?**](https://doi.org/10.48550/arXiv.2302.11521) （**2023.02.22**）

![](https://img.shields.io/badge/Citations-0-green)

[**PLACES: Prompting Language Models for Social Conversation Synthesis**](https://doi.org/10.48550/arXiv.2302.03269) （**2023.02.07**）

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-4-blue)](https://github.com/alexa/places)

[**Large Language Models Are Implicitly Topic Models: Explaining and Finding Good Demonstrations for In-Context Learning**](https://doi.org/10.48550/arXiv.2301.11916) （**2023.01.27**）

![](https://img.shields.io/badge/Citations-3-green)  [![](https://img.shields.io/badge/Github%20Stars-15-blue)](https://github.com/wangxinyilinda/concept-based-demonstration-selection)

[**Transformers as Algorithms: Generalization and Stability in In-context Learning**](https://arxiv.org/abs/2301.07067) （**2023.01.17**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-19-red)

[**OPT-IML: Scaling Language Model Instruction Meta Learning through the Lens of Generalization**](https://doi.org/10.48550/arXiv.2212.12017) （**2022.12.22**）

![](https://img.shields.io/badge/Citations-11-green)

[**Prompt-Augmented Linear Probing: Scaling Beyond The Limit of Few-shot In-Context Learners**](https://doi.org/10.48550/arXiv.2212.10873) （**2022.12.21**）

![](https://img.shields.io/badge/Citations-2-green)

[**In-context Learning Distillation: Transferring Few-shot Learning Ability of Pre-trained Language Models**](https://doi.org/10.48550/arXiv.2212.10670) （**2022.12.20**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "In-context Learning"](./PaperList/InContextLearningList.md)👈

## Multimodal Prompt

<div style="line-height:0.2em;">



[**Edit Everything: A Text-Guided Generative System for Images Editing**](https://arxiv.org/abs/2304.14006) （**2023.04.27**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-3-red)  [![](https://img.shields.io/badge/Github%20Stars-50-blue)](https://github.com/defengxie/edit_everything)

[**ChatVideo: A Tracklet-centric Multimodal and Versatile Video Understanding System**](https://arxiv.org/abs/2304.14407) （**2023.04.27**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-4-red)

[**mPLUG-Owl: Modularization Empowers Large Language Models with Multimodality**](https://arxiv.org/abs/2304.14178) （**2023.04.27**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-5-red)  [![](https://img.shields.io/badge/Github%20Stars-253-blue)](https://github.com/x-plug/mplug-owl)

[**Towards Robust Prompts on Vision-Language Models**](https://arxiv.org/abs/2304.08479) （**2023.04.17**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-12-red)

[**Visual Instruction Tuning**](https://arxiv.org/abs/2304.08485) （**2023.04.17**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-74-red)  [![](https://img.shields.io/badge/Github%20Stars-2.0k-blue)](https://github.com/haotian-liu/LLaVA)

[**Multimodal C4: An Open, Billion-scale Corpus of Images Interleaved With Text**](https://arxiv.org/abs/2304.06939) （**2023.04.14**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-38-red)  [![](https://img.shields.io/badge/Github%20Stars-655-blue)](https://github.com/allenai/mmc4)

[**Segment Everything Everywhere All at Once**](https://doi.org/10.48550/arXiv.2304.06718) （**2023.04.13**）

![](https://img.shields.io/badge/Citations-3-green)  [![](https://img.shields.io/badge/Github%20Stars-2.2k-blue)](https://github.com/ux-decoder/segment-everything-everywhere-all-at-once)

[**Efficient Multimodal Fusion via Interactive Prompting**](https://arxiv.org/abs/2304.06306) （**2023.04.13**）

![](https://img.shields.io/badge/Citations-0-green)

[**ChatGPT Beyond English: Towards a Comprehensive Evaluation of Large Language Models in Multilingual Learning**](https://arxiv.org/abs/2304.05613) （**2023.04.12**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-18-red)

[**Prompt Pre-Training with Twenty-Thousand Classes for Open-Vocabulary Visual Recognition**](https://doi.org/10.48550/arXiv.2304.04704) （**2023.04.10**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-165-blue)](https://github.com/amazon-science/prompt-pretraining)


</div>

👉[Complete paper list 🔗 for "Multimodal Prompt"](./PaperList/multimodalprompt.md)👈

## Prompt Application

<div style="line-height:0.2em;">



[**Emergent and Predictable Memorization in Large Language Models**](https://arxiv.org/abs/2304.11158) （**2023.04.21**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-6-red)

[**SpeechPrompt v2: Prompt Tuning for Speech Classification Tasks**](https://doi.org/10.48550/arXiv.2303.00733) （**2023.03.01**）

![](https://img.shields.io/badge/Citations-0-green)

[**Soft Prompt Guided Joint Learning for Cross-Domain Sentiment Analysis**](https://doi.org/10.48550/arXiv.2303.00815) （**2023.03.01**）

![](https://img.shields.io/badge/Citations-0-green)

[**EvoPrompting: Language Models for Code-Level Neural Architecture Search**](https://doi.org/10.48550/arXiv.2302.14838) （**2023.02.28**）

![](https://img.shields.io/badge/Citations-0-green)

[**More than you've asked for: A Comprehensive Analysis of Novel Prompt Injection Threats to Application-Integrated Large Language Models**](https://doi.org/10.48550/arXiv.2302.12173) （**2023.02.23**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-913-blue)](https://github.com/greshake/lm-safety)

[**Grimm in Wonderland: Prompt Engineering with Midjourney to Illustrate Fairytales**](https://doi.org/10.48550/arXiv.2302.08961) （**2023.02.17**）

![](https://img.shields.io/badge/Citations-0-green)

[**LabelPrompt: Effective Prompt-based Learning for Relation Classification**](https://doi.org/10.48550/arXiv.2302.08068) （**2023.02.16**）

![](https://img.shields.io/badge/Citations-0-green)

[**Prompt Tuning of Deep Neural Networks for Speaker-adaptive Visual Speech Recognition**](https://doi.org/10.48550/arXiv.2302.08102) （**2023.02.16**）

![](https://img.shields.io/badge/Citations-0-green)

[**Prompting for Multimodal Hateful Meme Classification**](https://doi.org/10.48550/arXiv.2302.04156) （**2023.02.08**）

![](https://img.shields.io/badge/Citations-1-green)

[**Toxicity Detection with Generative Prompt-based Inference**](https://doi.org/10.48550/arXiv.2205.12390) （**2022.05.24**）

![](https://img.shields.io/badge/Citations-2-green)


</div>

👉[Complete paper list 🔗 for "Prompt Application"](./PaperList/promptapplication.md)👈

## Foundation Models

<div style="line-height:0.2em;">



[**Improving Grounded Language Understanding in a Collaborative Environment by Interacting with Agents Through Help Feedback**](https://arxiv.org/abs/2304.10750) （**2023.04.21**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-4-red)

[**Segment Anything Model for Medical Image Analysis: an Experimental Study**](https://arxiv.org/abs/2304.10517) （**2023.04.20**）

![](https://img.shields.io/badge/Citations-1-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-18-red)  [![](https://img.shields.io/badge/Github%20Stars-3-blue)](https://github.com/mazurowski-lab/segment-anything-medical)

[**Chameleon: Plug-and-Play Compositional Reasoning with Large Language Models**](https://arxiv.org/abs/2304.09842) （**2023.04.19**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-51-red)  [![](https://img.shields.io/badge/Github%20Stars-618-blue)](https://github.com/lupantech/chameleon-llm)

[**Accuracy of Segment-Anything Model (SAM) in medical image segmentation tasks**](https://arxiv.org/abs/2304.09324) （**2023.04.18**）

![](https://img.shields.io/badge/Citations-1-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-10-red)

[**When SAM Meets Medical Images: An Investigation of Segment Anything Model (SAM) on Multi-phase Liver Tumor Segmentation**](https://arxiv.org/abs/2304.08506) （**2023.04.17**）

![](https://img.shields.io/badge/Citations-1-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)

[**The Segment Anything foundation model achieves favorable brain tumor autosegmentation accuracy on MRI to support radiotherapy treatment planning**](https://arxiv.org/abs/2304.07875) （**2023.04.16**）

![](https://img.shields.io/badge/Citations-0-green)

[**Deep learning universal crater detection using Segment Anything Model (SAM)**](https://doi.org/10.48550/arXiv.2304.07764) （**2023.04.16**）

![](https://img.shields.io/badge/Citations-0-green)

[**Segment Anything Model (SAM) for Digital Pathology: Assess Zero-shot Segmentation on Whole Slide Imaging**](https://doi.org/10.48550/arXiv.2304.04155) （**2023.04.09**）

![](https://img.shields.io/badge/Citations-5-green)

[**TagGPT: Large Language Models are Zero-shot Multimodal Taggers**](https://arxiv.org/abs/2304.03022) （**2023.04.06**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-8-red)  [![](https://img.shields.io/badge/Github%20Stars-19-blue)](https://github.com/tencentarc/taggpt)

[**Pythia: A Suite for Analyzing Large Language Models Across Training and Scaling**](https://arxiv.org/abs/2304.01373) （**2023.04.03**）

![](https://img.shields.io/badge/Citations-3-green)  [![](https://img.shields.io/badge/Github%20Stars-5.2k-blue)](https://github.com/eleutherai/gpt-neox)


</div>

👉[Complete paper list 🔗 for "Foundation Models"](./PaperList/foundationmodels.md)👈

<!-- ### 📌 Hard Prompt/ Discrete Prompt

<div style="line-height:0.2em;">



[**Hard Prompts Made Easy: Gradient-Based Discrete Optimization for Prompt Tuning and Discovery**](https://doi.org/10.48550/arXiv.2302.03668) （**2023.02.07**）

![](https://img.shields.io/badge/Citations-2-green)  [![](https://img.shields.io/badge/Github%20Stars-398-blue)](https://github.com/YuxinWenRick/hard-prompts-made-easy)

[**SPT: Semi-Parametric Prompt Tuning for Multitask Prompted Learning**](https://doi.org/10.48550/arXiv.2212.10929) （**2022.12.21**）

![](https://img.shields.io/badge/Citations-1-green)

[**ADEPT: A DEbiasing PrompT Framework**](https://doi.org/10.48550/arXiv.2211.05414) （**2022.11.10**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-6-blue)](https://github.com/EmpathYang/ADEPT)

[**PromptAttack: Prompt-based Attack for Language Models via Gradient Search**](https://doi.org/10.48550/arXiv.2209.01882) （**2022.09.05**）

![](https://img.shields.io/badge/Citations-0-green)

[**RLPrompt: Optimizing Discrete Text Prompts with Reinforcement Learning**](https://doi.org/10.48550/arXiv.2205.12548) （**2022.05.25**）

![](https://img.shields.io/badge/Citations-25-green)  [![](https://img.shields.io/badge/Github%20Stars-190-blue)](https://github.com/mingkaid/rl-prompt)

[**Personalized Prompt Learning for Explainable Recommendation**](https://arxiv.org/abs/2202.07371) （**2022.02.15**）

![](https://img.shields.io/badge/Citations-10-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-18-red)  [![](https://img.shields.io/badge/Github%20Stars-65-blue)](https://github.com/lileipisces/pepler)

[**Instance-aware Prompt Learning for Language Understanding and Generation**](https://arxiv.org/abs/2201.07126) （**2022.01.18**）

![](https://img.shields.io/badge/Citations-10-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-21-red)  [![](https://img.shields.io/badge/Github%20Stars-6-blue)](https://github.com/jinfeihu-stan/ipl)


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