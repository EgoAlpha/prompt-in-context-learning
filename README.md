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
        <a href="./chatgptprompt_zh.md">็ฎไฝไธญๆ</a>
    <p>
</h4>

<p align="center">

  <a href="#๐-papers">๐ Papers</a> |
  <a href="./Playground.md">โก๏ธ  Playground</a> |
  <a href="./PromptEngineering.md">๐  Prompt Engineering</a> |
  <a href="./chatgptprompt.md">๐ ChatGPT Prompt</a> 

</p>

</div>

<div align="center">

<!-- ![Build](https://img.shields.io/appveyor/build/gruntjs/grunt) -->

![version](https://img.shields.io/badge/version-v1.0.0-blue)
![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)

<!-- ![license](https://img.shields.io/bower/l/bootstrap?style=plastic) -->

</div>

> **โญ๏ธ Shining โญ๏ธ:** This is fresh, daily-updated resources for in-context learning and prompt engineering. As Artificial General Intelligence (AGI) is approaching, letโs take action and become a super learner so as to position ourselves at the forefront of this exciting era and strive for personal and professional greatness.

The resources include:

*๐[Papers](#๐-papers)๐*:  The latest papers about in-context learning or prompt engineering. 

*๐[Playground](./Playground.md)๐*:  Large language models that enable prompt experimentation. 

*๐[Prompt Engineering](./PromptEngineering.md)๐*: Prompt techniques for leveraging large language models. 

*๐[ChatGPT Prompt](./chatgptprompt.md)๐*: Prompt examples that can be applied in our work and daily lives. 

In the future, there will likely be two types of people on Earth (perhaps even on Mars, but that's a question for Musk): 
Those who enhance their abilities through the use of AI; 
Those whose jobs are replaced by AI automation.

```

๐EgoAlpha: Hello! human๐ค, are you ready?

```  

# ๐ข News

- **[2023.3.13]** [LLaMA has been fine-tuned by Stanford](https://github.com/tatsu-lab/stanford_alpaca)

- **[2023.3.10]** [Announcing OpenChatKit by Together](https://huggingface.co/spaces/togethercomputer/OpenChatKit)

- **[2023.3.9]**  GPT-4 is coming next week and it will be multimodal,announced by OpenAI.

- **[2023.3.8]** [Visual ChatGPT: Talking, Drawing and Editing with Visual Foundation Models](https://arxiv.org/abs/2303.04671)

- **[2023.3.7]** [Larger language models do in-context learning differently](https://arxiv.org/abs/2303.03846)

- **[2023.3.6]** [Multitask Prompt Tuning Enables Parameter-Efficient Transfer Learning](https://arxiv.org/abs/2303.02861)

<img width="200%" src="./figures/hr.gif" />

# ๐ Papers

- [Survey](#Survey)

- [Prompt Engineering](#prompt-engineering)

- [In-context learning](#in-context-learning)

- [Multimodal Prompt](#multimodal-prompt)

- [Prompt Application](#prompt-application)

<!-- - [Knowledge Augmented Prompts](#knowledge-augmented-prompts)

- [Prompt for Knowledge Graph](#prompt-for-knowledge-graph) -->

---

## Survey

<div style="line-height:0.2em;">



[**Reasoning with Language Model Prompting: A Survey**](https://doi.org/10.48550/arXiv.2212.09597) ๏ผ**2022.12.19**๏ผ

![](https://img.shields.io/badge/Citations-7-green)  [![](https://img.shields.io/badge/Github%20Stars-166-blue)](https://github.com/zjunlp/Prompt4ReasoningPapers)

[**Emergent Abilities of Large Language Models**](https://doi.org/10.48550/arXiv.2206.07682) ๏ผ**2022.06.15**๏ผ

![](https://img.shields.io/badge/Citations-151-green)  [![](https://img.shields.io/badge/Github%20Stars-755-blue)](https://github.com/zhaoolee/garss)

[**Pre-train, Prompt, and Predict: A Systematic Survey of Prompting Methods in Natural Language Processing**](https://doi.org/10.1145/3560815) ๏ผ**2021.07.28**๏ผ

![](https://img.shields.io/badge/Citations-444-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1.4k-red)  [![](https://img.shields.io/badge/Github%20Stars-140-blue)](https://github.com/mingkaid/rl-prompt)

[**Towards Reasoning in Large Language Models: A Survey**](https://api.semanticscholar.org/3ee9c65366efbb17adf370c39f20dbef60d53670) 

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-195-blue)](https://github.com/jeffhj/lm-reasoning)

[**A survey for in-context learning**](https://doi.org/10.48550/arXiv.2301.00234) 

![](https://img.shields.io/badge/Citations-0-green)

[**Augmented Language Models: a Survey**](https://api.semanticscholar.org/2029349c55c1dba3493c5b3bd25152f18ba21ae2) 

![](https://img.shields.io/badge/Citations-0-green)


</div>

๐[Complete paper list ๐ for "Survey"](./PaperList/survey.md)๐

## Prompt Engineering

### ๐ Prompt Design

<div style="line-height:0.2em;">



[**A Prompt Pattern Catalog to Enhance Prompt Engineering with ChatGPT**](https://doi.org/10.48550/arXiv.2302.11382) ๏ผ**2023.02.21**๏ผ

![](https://img.shields.io/badge/Citations-1-green)

[**GraphPrompt: Unifying Pre-Training and Downstream Tasks for Graph Neural Networks**](https://doi.org/10.48550/arXiv.2302.08043) ๏ผ**2023.02.16**๏ผ

![](https://img.shields.io/badge/Citations-0-green)

[**Commonsense-Aware Prompting for Controllable Empathetic Dialogue Generation**](https://doi.org/10.48550/arXiv.2302.01441) ๏ผ**2023.02.02**๏ผ

![](https://img.shields.io/badge/Citations-0-green)

[**Progressive Prompts: Continual Learning for Language Models**](https://doi.org/10.48550/arXiv.2301.12314) ๏ผ**2023.01.29**๏ผ

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-1.7k-blue)](https://github.com/zjunlp/DeepKE/tree/main/example/ner/few-shot)

[**Batch Prompting: Efficient Inference with Large Language Model APIs**](https://doi.org/10.48550/arXiv.2301.08721) ๏ผ**2023.01.19**๏ผ

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-22-blue)](https://github.com/hkunlp/batch-prompting)

[**Successive Prompting for Decomposing Complex Questions**](https://doi.org/10.48550/arXiv.2212.04092) ๏ผ**2022.12.08**๏ผ

![](https://img.shields.io/badge/Citations-8-green)

[**Knowledge Prompting in Pre-trained Language Model for Natural Language Understanding**](https://doi.org/10.48550/arXiv.2210.08536) ๏ผ**2022.10.16**๏ผ

![](https://img.shields.io/badge/Citations-2-green)  [![](https://img.shields.io/badge/Github%20Stars-10-blue)](https://github.com/wjn1996/kp-plm)

[**Promptagator: Few-shot Dense Retrieval From 8 Examples**](https://doi.org/10.48550/arXiv.2209.11755) ๏ผ**2022.09.23**๏ผ

![](https://img.shields.io/badge/Citations-15-green)

[**Interactive and Visual Prompt Engineering for Ad-hoc Task Adaptation with Large Language Models**](https://doi.org/10.1109/TVCG.2022.3209479) ๏ผ**2022.08.16**๏ผ

![](https://img.shields.io/badge/Citations-10-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-22-red)

[**DocPrompting: Generating Code by Retrieving the Docs**](https://arxiv.org/abs/2207.05987) ๏ผ**2022.07.13**๏ผ

![](https://img.shields.io/badge/Citations-4-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-11-red)  [![](https://img.shields.io/badge/Github%20Stars-132-blue)](https://github.com/shuyanzhou/docprompting)


</div>

๐[Complete paper list ๐ for "Prompt Design"](./PaperList/PromptDesignList.md)๐

### ๐ Automatic Prompt 

<div style="line-height:0.2em;">



[**Automatic Prompt Augmentation and Selection with Chain-of-Thought from Labeled Data**](https://doi.org/10.48550/arXiv.2302.12822) ๏ผ**2023.02.24**๏ผ

![](https://img.shields.io/badge/Citations-0-green)

[**Guiding Large Language Models via Directional Stimulus Prompting**](https://doi.org/10.48550/arXiv.2302.11520) ๏ผ**2023.02.22**๏ผ

![](https://img.shields.io/badge/Citations-0-green)

[**Evaluating the Robustness of Discrete Prompts**](https://doi.org/10.48550/arXiv.2302.05619) ๏ผ**2023.02.11**๏ผ

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-2-blue)](https://github.com/livnlp/prompt-robustness)

[**Hard Prompts Made Easy: Gradient-Based Discrete Optimization for Prompt Tuning and Discovery**](https://doi.org/10.48550/arXiv.2302.03668) ๏ผ**2023.02.07**๏ผ

![](https://img.shields.io/badge/Citations-2-green)  [![](https://img.shields.io/badge/Github%20Stars-360-blue)](https://github.com/YuxinWenRick/hard-prompts-made-easy)

[**The Unreliability of Explanations in Few-shot Prompting for Textual Reasoning**](https://arxiv.org/abs/2205.03401) ๏ผ**2022.05.06**๏ผ

![](https://img.shields.io/badge/Citations-10-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-26-red)  [![](https://img.shields.io/badge/Github%20Stars-1-blue)](https://github.com/xiye17/textualexplincontext)

[**Making Pre-trained Language Models Better Few-shot Learners**](https://doi.org/10.18653/v1/2021.acl-long.295) ๏ผ**2021.01.01**๏ผ

![](https://img.shields.io/badge/Citations-642-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-703-red)  [![](https://img.shields.io/badge/Github%20Stars-630-blue)](https://github.com/princeton-nlp/LM-BFF)

[**Eliciting Knowledge from Language Models Using Automatically Generated Prompts**](https://doi.org/10.18653/v1/2020.emnlp-main.346) ๏ผ**2020.10.29**๏ผ

![](https://img.shields.io/badge/Citations-136-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-475-red)  [![](https://img.shields.io/badge/Github%20Stars-340-blue)](https://github.com/ucinlp/autoprompt)

[**Automatically Identifying Words That Can Serve as Labels for Few-Shot Text Classification**](https://doi.org/10.5282/UBM/EPUB.74034) ๏ผ**2020.10.26**๏ผ

![](https://img.shields.io/badge/Citations-84-green)  [![](https://img.shields.io/badge/Github%20Stars-1.5k-blue)](https://github.com/timoschick/pet)


</div>

๐[Complete paper list ๐ for "Automatic Prompt"](./PaperList/AutomaticPromptList.md)๐

### ๐ Chain of Thought

<div style="line-height:0.2em;">



[**Synthetic Prompting: Generating Chain-of-Thought Demonstrations for Large Language Models**](https://doi.org/10.48550/arXiv.2302.00618) ๏ผ**2023.02.01**๏ผ

![](https://img.shields.io/badge/Citations-2-green)

[**Large Language Models Are Reasoning Teachers**](https://doi.org/10.48550/arXiv.2212.10071) ๏ผ**2022.12.20**๏ผ

![](https://img.shields.io/badge/Citations-5-green)  [![](https://img.shields.io/badge/Github%20Stars-55-blue)](https://github.com/zinengtang/VidLanKD)

[**The Impact of Symbolic Representations on In-context Learning for Few-shot Reasoning**](https://doi.org/10.48550/arXiv.2212.08686) ๏ผ**2022.12.16**๏ผ

![](https://img.shields.io/badge/Citations-2-green)

[**Complementary Explanations for Effective In-Context Learning**](https://doi.org/10.48550/arXiv.2211.13892) ๏ผ**2022.11.25**๏ผ

![](https://img.shields.io/badge/Citations-5-green)

[**Prompting GPT-3 To Be Reliable**](https://doi.org/10.48550/arXiv.2210.09150) ๏ผ**2022.10.17**๏ผ

![](https://img.shields.io/badge/Citations-9-green)  [![](https://img.shields.io/badge/Github%20Stars-47-blue)](https://github.com/noviscl/gpt3-reliability)

[**Challenging BIG-Bench Tasks and Whether Chain-of-Thought Can Solve Them**](https://doi.org/10.48550/arXiv.2210.09261) ๏ผ**2022.10.17**๏ผ

![](https://img.shields.io/badge/Citations-27-green)  [![](https://img.shields.io/badge/Github%20Stars-64-blue)](https://github.com/suzgunmirac/big-bench-hard)

[**Automatic Chain of Thought Prompting in Large Language Models**](https://doi.org/10.48550/arXiv.2210.03493) ๏ผ**2022.10.07**๏ผ

![](https://img.shields.io/badge/Citations-23-green)  [![](https://img.shields.io/badge/Github%20Stars-287-blue)](https://github.com/amazon-research/auto-cot)

[**Measuring and Narrowing the Compositionality Gap in Language Models**](https://doi.org/10.48550/arXiv.2210.03350) ๏ผ**2022.10.07**๏ผ

![](https://img.shields.io/badge/Citations-27-green)  [![](https://img.shields.io/badge/Github%20Stars-163-blue)](https://github.com/ofirpress/self-ask)

[**Language Models are Multilingual Chain-of-Thought Reasoners**](https://doi.org/10.48550/arXiv.2210.03057) ๏ผ**2022.10.06**๏ผ

![](https://img.shields.io/badge/Citations-21-green)  [![](https://img.shields.io/badge/Github%20Stars-64-blue)](https://github.com/google-research/url-nlp)

[**Decomposed Prompting: A Modular Approach for Solving Complex Tasks**](https://doi.org/10.48550/arXiv.2210.02406) ๏ผ**2022.10.05**๏ผ

![](https://img.shields.io/badge/Citations-25-green)  [![](https://img.shields.io/badge/Github%20Stars-19-blue)](https://github.com/allenai/decomp)


</div>

๐[Complete paper list ๐ for "Chain of Thought"](./PaperList/ChainofThoughtList.md)๐

### ๐ Evaluation & Reliability

<div style="line-height:0.2em;">



[**Language Model Crossover: Variation through Few-Shot Prompting**](https://doi.org/10.48550/arXiv.2302.12170) ๏ผ**2023.02.23**๏ผ

![](https://img.shields.io/badge/Citations-1-green)

[**Evaluating the Robustness of Discrete Prompts**](https://doi.org/10.48550/arXiv.2302.05619) ๏ผ**2023.02.11**๏ผ

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-2-blue)](https://github.com/livnlp/prompt-robustness)

[**PLACES: Prompting Language Models for Social Conversation Synthesis**](https://doi.org/10.48550/arXiv.2302.03269) ๏ผ**2023.02.07**๏ผ

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-4-blue)](https://github.com/alexa/places)

[**Controlling for Stereotypes in Multimodal Language Model Evaluation**](https://doi.org/10.48550/arXiv.2302.01582) ๏ผ**2023.02.03**๏ผ

![](https://img.shields.io/badge/Citations-0-green)

[**Large Language Models Can Be Easily Distracted by Irrelevant Context**](https://doi.org/10.48550/arXiv.2302.00093) ๏ผ**2023.01.31**๏ผ

![](https://img.shields.io/badge/Citations-3-green)  [![](https://img.shields.io/badge/Github%20Stars-5-blue)](https://github.com/google-research-datasets/gsm-ic)

[**Emergent Analogical Reasoning in Large Language Models**](https://doi.org/10.48550/arXiv.2212.09196) ๏ผ**2022.12.19**๏ผ

![](https://img.shields.io/badge/Citations-5-green)  [![](https://img.shields.io/badge/Github%20Stars-8-blue)](https://github.com/taylorwwebb/emergent_analogies_llm)

[**Discovering Language Model Behaviors with Model-Written Evaluations**](https://doi.org/10.48550/arXiv.2212.09251) ๏ผ**2022.12.19**๏ผ

![](https://img.shields.io/badge/Citations-6-green)  [![](https://img.shields.io/badge/Github%20Stars-101-blue)](https://github.com/anthropics/evals)

[**Constitutional AI: Harmlessness from AI Feedback**](https://doi.org/10.48550/arXiv.2212.08073) ๏ผ**2022.12.15**๏ผ

![](https://img.shields.io/badge/Citations-15-green)  [![](https://img.shields.io/badge/Github%20Stars-64-blue)](https://github.com/anthropics/constitutionalharmlessnesspaper)

[**On Second Thought, Let's Not Think Step by Step! Bias and Toxicity in Zero-Shot Reasoning**](https://doi.org/10.48550/arXiv.2212.08061) ๏ผ**2022.12.15**๏ผ

![](https://img.shields.io/badge/Citations-1-green)

[**Solving math word problems with process- and outcome-based feedback**](https://doi.org/10.48550/arXiv.2211.14275) ๏ผ**2022.11.25**๏ผ

![](https://img.shields.io/badge/Citations-3-green)


</div>

๐[Complete paper list ๐ for "Evaluation & Reliability"](./PaperList/EvaluationReliabilityList.md)๐

## In-context Learning

<div style="line-height:0.2em;">



[**How Robust is GPT-3.5 to Predecessors? A Comprehensive Study on Language Understanding Tasks**](https://doi.org/10.48550/arXiv.2303.00293) ๏ผ**2023.03.01**๏ผ

![](https://img.shields.io/badge/Citations-0-green)

[**Language Model Crossover: Variation through Few-Shot Prompting**](https://doi.org/10.48550/arXiv.2302.12170) ๏ผ**2023.02.23**๏ผ

![](https://img.shields.io/badge/Citations-1-green)

[**How Does In-Context Learning Help Prompt Tuning?**](https://doi.org/10.48550/arXiv.2302.11521) ๏ผ**2023.02.22**๏ผ

![](https://img.shields.io/badge/Citations-0-green)

[**Bounding the Capabilities of Large Language Models in Open Text Generation with Prompt Constraints**](https://doi.org/10.48550/arXiv.2302.09185) ๏ผ**2023.02.17**๏ผ

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-14-blue)](https://github.com/salt-nlp/bound-cap-llm)

[**Large Language Models Are Implicitly Topic Models: Explaining and Finding Good Demonstrations for In-Context Learning**](https://doi.org/10.48550/arXiv.2301.11916) ๏ผ**2023.01.27**๏ผ

![](https://img.shields.io/badge/Citations-1-green)  [![](https://img.shields.io/badge/Github%20Stars-10-blue)](https://github.com/wangxinyilinda/concept-based-demonstration-selection)

[**OPT-IML: Scaling Language Model Instruction Meta Learning through the Lens of Generalization**](https://doi.org/10.48550/arXiv.2212.12017) ๏ผ**2022.12.22**๏ผ

![](https://img.shields.io/badge/Citations-9-green)

[**Prompt-Augmented Linear Probing: Scaling Beyond The Limit of Few-shot In-Context Learners**](https://doi.org/10.48550/arXiv.2212.10873) ๏ผ**2022.12.21**๏ผ

![](https://img.shields.io/badge/Citations-2-green)

[**Self-adaptive In-context Learning**](https://doi.org/10.48550/arXiv.2212.10375) ๏ผ**2022.12.20**๏ผ

![](https://img.shields.io/badge/Citations-3-green)  [![](https://img.shields.io/badge/Github%20Stars-4-blue)](https://github.com/shark-nlp/self-adaptive-icl)

[**Is GPT-3 a Good Data Annotator?**](https://doi.org/10.48550/arXiv.2212.10450) ๏ผ**2022.12.20**๏ผ

![](https://img.shields.io/badge/Citations-2-green)  [![](https://img.shields.io/badge/Github%20Stars-76-blue)](https://github.com/blazejosinski/lm_nav)

[**One Embedder, Any Task: Instruction-Finetuned Text Embeddings**](https://doi.org/10.48550/arXiv.2212.09741) ๏ผ**2022.12.19**๏ผ

![](https://img.shields.io/badge/Citations-2-green)


</div>

๐[Complete paper list ๐ for "In-context Learning"](./PaperList/InContextLearningList.md)๐

## Multimodal Prompt

<div style="line-height:0.2em;">



[**Visual ChatGPT: Talking, Drawing and Editing with Visual Foundation Models**](https://arxiv.org/abs/2303.04671) ๏ผ**2023.03.08**๏ผ

![](https://img.shields.io/badge/Citations-0-green)

[**Multimodal Chain-of-Thought Reasoning in Language Models**](https://doi.org/10.48550/arXiv.2302.00923) ๏ผ**2023.02.02**๏ผ

![](https://img.shields.io/badge/Citations-4-green)  [![](https://img.shields.io/badge/Github%20Stars-3.0k-blue)](https://github.com/amazon-science/mm-cot)

[**CoHOZ**](https://doi.org/10.1145/3503161.3548021) ๏ผ**2022.10.10**๏ผ

![](https://img.shields.io/badge/Citations-0-green)

[**VIMA: General Robot Manipulation with Multimodal Prompts**](https://doi.org/10.48550/arXiv.2210.03094) ๏ผ**2022.10.06**๏ผ

![](https://img.shields.io/badge/Citations-15-green)

[**Learning to Prompt for Vision-Language Models**](https://doi.org/10.1007/s11263-022-01653-1) ๏ผ**2022.09.01**๏ผ

![](https://img.shields.io/badge/Citations-1-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-397-red)  [![](https://img.shields.io/badge/Github%20Stars-762-blue)](https://github.com/kaiyangzhou/coop)

[**Visual Prompt Tuning**](https://doi.org/10.48550/arXiv.2203.12119) ๏ผ**2022.03.23**๏ผ

![](https://img.shields.io/badge/Citations-102-green)  [![](https://img.shields.io/badge/Github%20Stars-350-blue)](https://github.com/KMnP/vpt)

[**Multimodal Few-Shot Learning with Frozen Language Models**](https://arxiv.org/abs/2106.13884) ๏ผ**2021.06.25**๏ผ

![](https://img.shields.io/badge/Citations-173-green)

[**Similarity-Aware Multimodal Prompt Learning for Fake News Detection**](https://doi.org/10.2139/ssrn.4347542) 

![](https://img.shields.io/badge/Citations-0-green)


</div>

๐[Complete paper list ๐ for "Multimodal Prompt"](./PaperList/MultimodalPromptList.md)๐

## Prompt Application

<div style="line-height:0.2em;">



[**SpeechPrompt v2: Prompt Tuning for Speech Classification Tasks**](https://doi.org/10.48550/arXiv.2303.00733) ๏ผ**2023.03.01**๏ผ

![](https://img.shields.io/badge/Citations-0-green)

[**Soft Prompt Guided Joint Learning for Cross-Domain Sentiment Analysis**](https://doi.org/10.48550/arXiv.2303.00815) ๏ผ**2023.03.01**๏ผ

![](https://img.shields.io/badge/Citations-0-green)

[**EvoPrompting: Language Models for Code-Level Neural Architecture Search**](https://doi.org/10.48550/arXiv.2302.14838) ๏ผ**2023.02.28**๏ผ

![](https://img.shields.io/badge/Citations-0-green)

[**More than you've asked for: A Comprehensive Analysis of Novel Prompt Injection Threats to Application-Integrated Large Language Models**](https://doi.org/10.48550/arXiv.2302.12173) ๏ผ**2023.02.23**๏ผ

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-350-blue)](https://github.com/greshake/lm-safety)

[**Grimm in Wonderland: Prompt Engineering with Midjourney to Illustrate Fairytales**](https://doi.org/10.48550/arXiv.2302.08961) ๏ผ**2023.02.17**๏ผ

![](https://img.shields.io/badge/Citations-0-green)

[**LabelPrompt: Effective Prompt-based Learning for Relation Classification**](https://doi.org/10.48550/arXiv.2302.08068) ๏ผ**2023.02.16**๏ผ

![](https://img.shields.io/badge/Citations-0-green)

[**Prompt Tuning of Deep Neural Networks for Speaker-adaptive Visual Speech Recognition**](https://doi.org/10.48550/arXiv.2302.08102) ๏ผ**2023.02.16**๏ผ

![](https://img.shields.io/badge/Citations-0-green)

[**Prompting for Multimodal Hateful Meme Classification**](https://doi.org/10.48550/arXiv.2302.04156) ๏ผ**2023.02.08**๏ผ

![](https://img.shields.io/badge/Citations-0-green)

[**Learning to Transfer Prompts for Text Generation**](https://doi.org/10.48550/arXiv.2205.01543) ๏ผ**2022.05.03**๏ผ

![](https://img.shields.io/badge/Citations-11-green)  [![](https://img.shields.io/badge/Github%20Stars-18-blue)](https://github.com/rucaibox/transfer-prompts-for-text-generation)

[**RelationPrompt: Leveraging Prompts to Generate Synthetic Data for Zero-Shot Relation Triplet Extraction**](https://doi.org/10.48550/arXiv.2203.09101) ๏ผ**2022.03.17**๏ผ

![](https://img.shields.io/badge/Citations-14-green)  [![](https://img.shields.io/badge/Github%20Stars-86-blue)](https://github.com/declare-lab/relationprompt)


</div>

๐[Complete paper list ๐ for "Prompt Application"](./PaperList/promptapplication.md)๐

<!-- ### ๐ Hard Prompt/ Discrete Prompt

<div style="line-height:0.2em;">



[**Hard Prompts Made Easy: Gradient-Based Discrete Optimization for Prompt Tuning and Discovery**](https://doi.org/10.48550/arXiv.2302.03668) ๏ผ**2023.02.07**๏ผ

![](https://img.shields.io/badge/Citations-2-green)  [![](https://img.shields.io/badge/Github%20Stars-360-blue)](https://github.com/YuxinWenRick/hard-prompts-made-easy)

[**SPT: Semi-Parametric Prompt Tuning for Multitask Prompted Learning**](https://doi.org/10.48550/arXiv.2212.10929) ๏ผ**2022.12.21**๏ผ

![](https://img.shields.io/badge/Citations-1-green)

[**RLPrompt: Optimizing Discrete Text Prompts with Reinforcement Learning**](https://doi.org/10.48550/arXiv.2205.12548) ๏ผ**2022.05.25**๏ผ

![](https://img.shields.io/badge/Citations-25-green)  [![](https://img.shields.io/badge/Github%20Stars-140-blue)](https://github.com/mingkaid/rl-prompt)

[**Personalized Prompt Learning for Explainable Recommendation**](https://arxiv.org/abs/2202.07371) ๏ผ**2022.02.15**๏ผ

![](https://img.shields.io/badge/Citations-10-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-12-red)  [![](https://img.shields.io/badge/Github%20Stars-57-blue)](https://github.com/lileipisces/pepler)

[**Instance-aware Prompt Learning for Language Understanding and Generation**](https://arxiv.org/abs/2201.07126) ๏ผ**2022.01.18**๏ผ

![](https://img.shields.io/badge/Citations-10-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-21-red)  [![](https://img.shields.io/badge/Github%20Stars-6-blue)](https://github.com/jinfeihu-stan/ipl)

[**PromptAttack: Prompt-based Attack for Language Models via Gradient Search**](https://api.semanticscholar.org/251269b9e16ab1da20cb57a669b2bfdbd0d1cd72) 

![](https://img.shields.io/badge/Citations-0-green)

[**ADEPT: A DEbiasing PrompT Framework**](https://api.semanticscholar.org/1abd4fa45ce20175452aa238870db2aebe9c0fe0) 

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-3-blue)](https://github.com/EmpathYang/ADEPT)


</div>

๐[Complete paper list ๐ for "Hard Prompt"](./PaperList/HardPromptList.md)๐

### ๐ Soft Prompt/ Continuous Prompt

<div style="line-height:0.2em;">



[**Dr ChatGPT, tell me what I want to hear: How prompt knowledge impacts health answer correctness**](https://doi.org/10.48550/arXiv.2302.13793) ๏ผ**2023.02.23**๏ผ

![](https://img.shields.io/badge/Citations-1-green)

[**How Does In-Context Learning Help Prompt Tuning?**](https://doi.org/10.48550/arXiv.2302.11521) ๏ผ**2023.02.22**๏ผ

![](https://img.shields.io/badge/Citations-0-green)

[**Scalable Prompt Generation for Semi-supervised Learning with Language Models**](https://doi.org/10.48550/arXiv.2302.09236) ๏ผ**2023.02.18**๏ผ

![](https://img.shields.io/badge/Citations-0-green)

[**Towards Unifying Medical Vision-and-Language Pre-training via Soft Prompts**](https://doi.org/10.48550/arXiv.2302.08958) ๏ผ**2023.02.17**๏ผ

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-5-blue)](https://github.com/zhjohnchan/ptunifier)

[**SwitchPrompt: Learning Domain-Specific Gated Soft Prompts for Classification in Low-Resource Domains**](https://doi.org/10.48550/arXiv.2302.06868) ๏ผ**2023.02.14**๏ผ

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-44-blue)](https://github.com/boschresearch/switchprompt)

[**Parameter-Efficient Low-Resource Dialogue State Tracking by Prompt Tuning**](https://doi.org/10.48550/arXiv.2301.10915) ๏ผ**2023.01.26**๏ผ

![](https://img.shields.io/badge/Citations-0-green)

[**Toward Human Readable Prompt Tuning: Kubrick's The Shining is a good movie, and a good prompt too?**](https://doi.org/10.48550/arXiv.2212.10539) ๏ผ**2022.12.20**๏ผ

![](https://img.shields.io/badge/Citations-1-green)

[**Controlled Text Generation using T5 based Encoder-Decoder Soft Prompt Tuning and Analysis of the Utility of Generated Text in AI**](https://doi.org/10.48550/arXiv.2212.02924) ๏ผ**2022.12.06**๏ผ

![](https://img.shields.io/badge/Citations-0-green)

[**Decomposed Soft Prompt Guided Fusion Enhancing for Compositional Zero-Shot Learning**](https://doi.org/10.48550/arXiv.2211.10681) ๏ผ**2022.11.19**๏ผ

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-3-blue)](https://github.com/forest-art/dfsp)

[**FPT: Improving Prompt Tuning Efficiency via Progressive Training**](https://doi.org/10.48550/arXiv.2211.06840) ๏ผ**2022.11.13**๏ผ

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-8-blue)](https://github.com/thunlp/fastprompttuning)


</div>

๐[Complete paper list ๐ for "Soft Prompt"](./PaperList/SoftPromptList.md)๐ -->

<!-- ## Knowledge Augmented Prompts

// __PAPER_LIST__:{field:'Prompt Design',size:10,state:'corrected',type:'lite'}

๐[Complete paper list ๐ for "Knowledge Augmented Prompts"](./PaperList/KnowledgeAugmentedPromptList.md)๐

## Prompt for Knowledge Graph

// __PAPER_LIST__:{field:'Prompt Design',size:10,state:'corrected',type:'lite'}

๐[Complete paper list ๐ for "Prompt for Knowledge Graph"](./PaperList/PromptKnowledgeGraphList.md)๐ -->

<img width="200%" src="./figures/hr.gif" />

<!-- # ๐ Citation

If you find our work helps, please star our project and cite our paper. Thanks a lot!

```

็ปผ่ฟฐ่ฎบๆๅฏไปฅๆพๅจ่ฟไธชไฝ็ฝฎ

``` -->

<!-- <img width="200%" src="./figures/hr.gif" /> -->

# โ๏ธ Contact

This repo is maintained by [EgoAlpha Lab](https://github.com/EgoAlpha). Questions and discussions are welcome via `helloegoalpha@gmail.com`.

We are willing to engage in discussions with friends from the academic and industrial communities, and explore the latest developments in prompt engineering and in-context learning together.

<img width="200%" src="./figures/hr.gif" />

# ๐ Acknowledgements

Thanks to the PhD students from [EgoAlpha Lab](https://github.com/EgoAlpha) and other workers who participated in this repo. We will improve the project in the follow-up period and maintain this community well. We also would like to express our sincere gratitude to the authors of the relevant resources. Your efforts have broadened our horizons and enabled us to perceive a more wonderful world.


<!-- <img width="200%" src="./figures/hr.gif" /> -->

<!-- # ๐จโ๐ฉโ๐งโ๐ฆ Contributors

## Main Contributors
* [Yu Liu]()
* [Yifei Cao](https://github.com/cyfedu1024)
* [Jizhe Yu]()
* [Yuan Yao]()
* [He Qi]() -->


<!-- ## Guest Contributors
* [No] -->

<!-- <img width="200%" src="./figures/hr.gif" />

# ๐ License

This project is open source and available under the MIT

<div align="center">
<img src="./figures/rocket.png"/>
</div> -->
