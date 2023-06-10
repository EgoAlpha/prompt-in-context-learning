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

- **[2023.6.10]**
    - [Aquila, language model series, including the Aquila Basic Model (7B and 33B), AquilaChat dialogue model, and AquilaCode text-to-code generation model.](https://github.com/FlagAI-Open/FlagAI/tree/master/examples/Aquila)
    
- **[2023.6.9]**
    - Paper: [Video-LLaMA: An Instruction-tuned Audio-Visual Language Model for Video Understanding](https://arxiv.org/abs/2306.02858)

- **[2023.6.8]**
    - Paper: [FrugalGPT: How to Use Large Language Models While Reducing Cost and Improving Performance](https://arxiv.org/pdf/2305.05176.pdf)
    
- **[2023.6.7]**
    - Paper: [XPhoneBERT: A Pre-trained Multilingual Model for Phoneme Representations for Text-to-Speech](https://arxiv.org/abs/2305.19709)
    
- **[2023.6.6]**
    - Paper: [XuanYuan 2.0: A Large Chinese Financial Chat Model with Hundreds of Billions Parameters](https://arxiv.org/abs/2305.12002)
    - Paper: [UniControl: A Unified Diffusion Model for Controllable Visual Generation In the Wild](https://arxiv.org/abs/2305.11147)
    
- **[2023.6.5]**
    - Paper: [Controllable Text-to-Image Generation with GPT-4](https://arxiv.org/abs/2305.18583)

- **[2023.6.4]**
    - PandaGPT: One model unifies six modalities([Page](https://panda-gpt.github.io/)/[Paper](https://arxiv.org/abs/2305.16355))

- **[2023.6.3]**
    - Paper: [Direct Preference Optimization:Your Language Model is Secretly a Reward Model](https://arxiv.org/pdf/2305.18290.pdf)
- **[2023.6.2]**
    - Paper: [SwiftSage: A Generative Agent with Fast and Slow Thinking for Complex Interactive Tasks](https://arxiv.org/abs/2305.17390)

- **[2023.6.1]**
    - Paper: [Generating Images with Multimodal Language Models](https://arxiv.org/abs/2305.17216)

- **[2023.5.31]**
    - [Intel announces the Aurora genAI, which is generative AI model with 1 trillion parameters](https://wccftech.com/intel-aurora-genai-chatgpt-competitor-generative-ai-model-with-1-trillion-parameters/)
    
    - HuotuoGPT, towards Taming Language Model to Be a Doctor([Github](https://github.com/FreedomIntelligence/HuatuoGPT)/[Demo](https://www.huatuogpt.cn)/[Paper](https://arxiv.org/pdf/2305.15075.pdf))
    - Paper: [Large Language Models Meet NL2Code: A Survey](https://arxiv.org/abs/2212.09420)

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



[**LLMDet: A Large Language Models Detection Tool**](https://arxiv.org/abs/2305.15004) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**OverPrompt: Enhancing ChatGPT Capabilities through an Efficient In-Context Learning Approach**](https://arxiv.org/abs/2305.14973) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Frugal Prompting for Dialog Models**](https://arxiv.org/abs/2305.14919) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Machine Reading Comprehension using Case-based Reasoning**](https://arxiv.org/abs/2305.14815) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**MQuAKE: Assessing Knowledge Editing in Language Models via Multi-Hop Questions**](https://arxiv.org/abs/2305.14795) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**In-Context Demonstration Selection with Cross Entropy Difference**](https://arxiv.org/abs/2305.14726) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Abductive Commonsense Reasoning Exploiting Mutually Exclusive Explanations**](https://arxiv.org/abs/2305.14618) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Unraveling ChatGPT: A Critical Analysis of AI-Generated Goal-Oriented Dialogues and Annotations**](https://arxiv.org/abs/2305.14556) （**2023.05.23**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)

[**Interpretable Automatic Fine-grained Inconsistency Detection in Text Summarization**](https://arxiv.org/abs/2305.14548) （**2023.05.23**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-3-blue)](https://github.com/kenchan0226/finegrainedfact)

[**ChatCoT: Tool-Augmented Chain-of-Thought Reasoning on Chat-based Large Language Models**](https://arxiv.org/abs/2305.14323) （**2023.05.23**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-2-blue)](https://github.com/rucaibox/chatcot)


</div>

👉[Complete paper list 🔗 for "Survey"](./PaperList/survey.md)👈

## Prompt Engineering

### Prompt Design

<div style="line-height:0.2em;">



[**EXnet: Efficient In-context Learning for Data-less Text classification**](https://arxiv.org/abs/2305.14622) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Peek Across: Improving Multi-Document Modeling via Cross-Document Question-Answering**](https://arxiv.org/abs/2305.15387) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Enhancing Retrieval-Augmented Large Language Models with Iterative Retrieval-Generation Synergy**](https://arxiv.org/abs/2305.15294) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-4-red)

[**Revisiting Token Dropping Strategy in Efficient BERT Pretraining**](https://arxiv.org/abs/2305.15273) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-1-green)

[**Revisiting Parallel Context Windows: A Frustratingly Simple Alternative and Chain-of-Thought Deterioration**](https://arxiv.org/abs/2305.15262) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Boosting Cross-lingual Transferability in Multilingual Models via In-Context Learning**](https://arxiv.org/abs/2305.15233) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**SAIL: Search-Augmented Instruction Learning**](https://arxiv.org/abs/2305.15225) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)

[**Towards Adaptive Prefix Tuning for Parameter-Efficient Language Model Fine-tuning**](https://arxiv.org/abs/2305.15212) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Lawyer LLaMA Technical Report**](https://arxiv.org/abs/2305.15062) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-60-blue)](https://github.com/andrewzhe/lawyer-llama)

[**Self-ICL: Zero-Shot In-Context Learning with Self-Generated Demonstrations**](https://arxiv.org/abs/2305.15035) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Prompt Design"](./PaperList/PromptDesignList.md)👈

### Automatic Prompt 

<div style="line-height:0.2em;">



[**Flatness-Aware Prompt Selection Improves Accuracy and Sample Efficiency**](https://doi.org/10.48550/arXiv.2305.10713) （**2023.05.18**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-4-blue)](https://github.com/shadowkiller33/flatness)

[**Automatic Prompt Augmentation and Selection with Chain-of-Thought from Labeled Data**](https://doi.org/10.48550/arXiv.2302.12822) （**2023.02.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Guiding Large Language Models via Directional Stimulus Prompting**](https://doi.org/10.48550/arXiv.2302.11520) （**2023.02.22**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-11-blue)](https://github.com/leezekun/directional-stimulus-prompting)

[**Evaluating the Robustness of Discrete Prompts**](https://doi.org/10.48550/arXiv.2302.05619) （**2023.02.11**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-3-blue)](https://github.com/livnlp/prompt-robustness)

[**Hard Prompts Made Easy: Gradient-Based Discrete Optimization for Prompt Tuning and Discovery**](https://doi.org/10.48550/arXiv.2302.03668) （**2023.02.07**）

![](https://img.shields.io/badge/Citations-2-green)  [![](https://img.shields.io/badge/Github%20Stars-413-blue)](https://github.com/YuxinWenRick/hard-prompts-made-easy)

[**Ask Me Anything: A simple strategy for prompting language models**](https://doi.org/10.48550/arXiv.2210.02441) （**2022.10.05**）

![](https://img.shields.io/badge/Citations-14-green)  [![](https://img.shields.io/badge/Github%20Stars-453-blue)](https://github.com/hazyresearch/ama_prompting)

[**STaR: Bootstrapping Reasoning With Reasoning**](https://doi.org/10.48550/arXiv.2203.14465) （**2022.03.28**）

![](https://img.shields.io/badge/Citations-56-green)  [![](https://img.shields.io/badge/Github%20Stars-17-blue)](https://github.com/ezelikman/STaR)

[**Making Pre-trained Language Models Better Few-shot Learners**](https://doi.org/10.18653/v1/2021.acl-long.295) （**2021.01.01**）

![](https://img.shields.io/badge/Citations-648-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-742-red)  [![](https://img.shields.io/badge/Github%20Stars-657-blue)](https://github.com/princeton-nlp/LM-BFF)

[**Eliciting Knowledge from Language Models Using Automatically Generated Prompts**](https://doi.org/10.18653/v1/2020.emnlp-main.346) （**2020.10.29**）

![](https://img.shields.io/badge/Citations-137-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-518-red)

[**Automatically Identifying Words That Can Serve as Labels for Few-Shot Text Classification**](https://doi.org/10.5282/UBM/EPUB.74034) （**2020.10.26**）

![](https://img.shields.io/badge/Citations-85-green)  [![](https://img.shields.io/badge/Github%20Stars-1.5k-blue)](https://github.com/timoschick/pet)


</div>

👉[Complete paper list 🔗 for "Automatic Prompt"](./PaperList/AutomaticPromptList.md)👈

### Chain of Thought

<div style="line-height:0.2em;">



[**PESCO: Prompt-enhanced Self Contrastive Learning for Zero-shot Text Classification**](https://arxiv.org/abs/2305.14963) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**In-Context Demonstration Selection with Cross Entropy Difference**](https://arxiv.org/abs/2305.14726) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Abductive Commonsense Reasoning Exploiting Mutually Exclusive Explanations**](https://arxiv.org/abs/2305.14618) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Unraveling ChatGPT: A Critical Analysis of AI-Generated Goal-Oriented Dialogues and Annotations**](https://arxiv.org/abs/2305.14556) （**2023.05.23**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)

[**Interpretable Automatic Fine-grained Inconsistency Detection in Text Summarization**](https://arxiv.org/abs/2305.14548) （**2023.05.23**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-3-blue)](https://github.com/kenchan0226/finegrainedfact)

[**ChatCoT: Tool-Augmented Chain-of-Thought Reasoning on Chat-based Large Language Models**](https://arxiv.org/abs/2305.14323) （**2023.05.23**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-2-blue)](https://github.com/rucaibox/chatcot)

[**mPMR: A Multilingual Pre-trained Machine Reader at Scale**](https://arxiv.org/abs/2305.13645) （**2023.05.23**）

![](https://img.shields.io/badge/Citations-3-green)  [![](https://img.shields.io/badge/Github%20Stars-4-blue)](https://github.com/damo-nlp-sg/pmr)

[**Cross-functional Analysis of Generalisation in Behavioural Learning**](https://arxiv.org/abs/2305.12951) （**2023.05.22**）

![](https://img.shields.io/badge/Citations-0-green)

[**LM-Switch: Lightweight Language Model Conditioning in Word Embedding Space**](https://arxiv.org/abs/2305.12798) （**2023.05.22**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-3-red)

[**LogiCoT: Logical Chain-of-Thought Instruction-Tuning Data Collection with GPT-4**](https://arxiv.org/abs/2305.12147) （**2023.05.20**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-10-blue)](https://github.com/csitfun/logicot)


</div>

👉[Complete paper list 🔗 for "Chain of Thought"](./PaperList/ChainofThoughtList.md)👈

### Knowledge Augmented Prompt

<div style="line-height:0.2em;">



[**LLMDet: A Large Language Models Detection Tool**](https://arxiv.org/abs/2305.15004) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**OverPrompt: Enhancing ChatGPT Capabilities through an Efficient In-Context Learning Approach**](https://arxiv.org/abs/2305.14973) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**PESCO: Prompt-enhanced Self Contrastive Learning for Zero-shot Text Classification**](https://arxiv.org/abs/2305.14963) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Frugal Prompting for Dialog Models**](https://arxiv.org/abs/2305.14919) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Machine Reading Comprehension using Case-based Reasoning**](https://arxiv.org/abs/2305.14815) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**In-Context Demonstration Selection with Cross Entropy Difference**](https://arxiv.org/abs/2305.14726) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Enhancing Cross-lingual Natural Language Inference by Soft Prompting with Multilingual Verbalizer**](https://arxiv.org/abs/2305.12761) （**2023.05.22**）

![](https://img.shields.io/badge/Citations-0-green)

[**A Benchmark on Extremely Weakly Supervised Text Classification: Reconcile Seed Matching and Prompting Approaches**](https://arxiv.org/abs/2305.12749) （**2023.05.22**）

![](https://img.shields.io/badge/Citations-0-green)

[**SelfzCoT: a Self-Prompt Zero-shot CoT from Semantic-level to Code-level for a Better Utilization of LLMs**](https://doi.org/10.48550/arXiv.2305.11461) （**2023.05.19**）

![](https://img.shields.io/badge/Citations-0-green)

[**Controlling the Extraction of Memorized Data from Large Language Models via Prompt-Tuning**](https://doi.org/10.48550/arXiv.2305.11759) （**2023.05.19**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Knowledge Augmented Prompt"](./PaperList/KnowledgeAugmentedPromptList.md)👈


### Evaluation & Reliability

<div style="line-height:0.2em;">



[**SETI: Systematicity Evaluation of Textual Inference**](https://arxiv.org/abs/2305.15045) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Is GPT-4 a Good Data Analyst?**](https://arxiv.org/abs/2305.15038) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**From Words to Wires: Generating Functioning Electronic Devices from Natural Language Descriptions**](https://arxiv.org/abs/2305.14874) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)

[**Drafting Event Schemas using Language Models**](https://arxiv.org/abs/2305.14847) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Testing Causal Models of Word Meaning in GPT-3 and -4**](https://arxiv.org/abs/2305.14630) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Uncovering and Quantifying Social Biases in Code Generation**](https://arxiv.org/abs/2305.15377) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-1-green)

[**A Simple and Effective Framework for Strict Zero-Shot Hierarchical Classification**](https://arxiv.org/abs/2305.15282) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)

[**Testing the General Deductive Reasoning Capacity of Large Language Models Using OOD Examples**](https://arxiv.org/abs/2305.15269) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)

[**EvEval: A Comprehensive Evaluation of Event Semantics for Large Language Models**](https://arxiv.org/abs/2305.15268) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Eliciting the Translation Ability of Large Language Models via Multilingual Finetuning with Translation Instructions**](https://arxiv.org/abs/2305.15083) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "Evaluation & Reliability"](./PaperList/EvaluationReliabilityList.md)👈

## In-context Learning

<div style="line-height:0.2em;">



[**Peek Across: Improving Multi-Document Modeling via Cross-Document Question-Answering**](https://arxiv.org/abs/2305.15387) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**SummIt: Iterative Text Summarization via ChatGPT**](https://arxiv.org/abs/2305.14835) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**READ: Recurrent Adaptation of Large Transformers**](https://arxiv.org/abs/2305.15348) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-3-red)

[**Learning Answer Generation using Supervision from Automatic Question Answering Evaluators**](https://arxiv.org/abs/2305.15344) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Measuring and Mitigating Constraint Violations of In-Context Learning for Utterance-to-API Semantic Parsing**](https://arxiv.org/abs/2305.15338) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)

[**Self-Evolution Learning for Discriminative Language Model Pretraining**](https://arxiv.org/abs/2305.15275) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-1-green)

[**SenteCon: Leveraging Lexicons to Learn Human-Interpretable Language Representations**](https://arxiv.org/abs/2305.14728) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**PathAsst: Redefining Pathology through Generative Foundation AI Assistant for Pathology**](https://arxiv.org/abs/2305.15072) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-1-blue)](https://github.com/superjamessyx/generative-foundation-ai-assistant-for-pathology)

[**Not All Metrics Are Guilty: Improving NLG Evaluation with LLM Paraphrasing**](https://arxiv.org/abs/2305.15067) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-1-blue)](https://github.com/rucaibox/para-ref)

[**LLMDet: A Large Language Models Detection Tool**](https://arxiv.org/abs/2305.15004) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)


</div>

👉[Complete paper list 🔗 for "In-context Learning"](./PaperList/InContextLearningList.md)👈

## Multimodal Prompt

<div style="line-height:0.2em;">



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

[**Abductive Commonsense Reasoning Exploiting Mutually Exclusive Explanations**](https://arxiv.org/abs/2305.14618) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Goat: Fine-tuned LLaMA Outperforms GPT-4 on Arithmetic Tasks**](https://arxiv.org/abs/2305.14201) （**2023.05.23**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-14-red)

[**Unraveling ChatGPT: A Critical Analysis of AI-Generated Goal-Oriented Dialogues and Annotations**](https://arxiv.org/abs/2305.14556) （**2023.05.23**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)

[**Interpretable Automatic Fine-grained Inconsistency Detection in Text Summarization**](https://arxiv.org/abs/2305.14548) （**2023.05.23**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-3-blue)](https://github.com/kenchan0226/finegrainedfact)


</div>

👉[Complete paper list 🔗 for "Multimodal Prompt"](./PaperList/multimodalprompt.md)👈

## Prompt Application

<div style="line-height:0.2em;">



[**Peek Across: Improving Multi-Document Modeling via Cross-Document Question-Answering**](https://arxiv.org/abs/2305.15387) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**LLMDet: A Large Language Models Detection Tool**](https://arxiv.org/abs/2305.15004) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**OverPrompt: Enhancing ChatGPT Capabilities through an Efficient In-Context Learning Approach**](https://arxiv.org/abs/2305.14973) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**PESCO: Prompt-enhanced Self Contrastive Learning for Zero-shot Text Classification**](https://arxiv.org/abs/2305.14963) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Frugal Prompting for Dialog Models**](https://arxiv.org/abs/2305.14919) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Machine Reading Comprehension using Case-based Reasoning**](https://arxiv.org/abs/2305.14815) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**MQuAKE: Assessing Knowledge Editing in Language Models via Multi-Hop Questions**](https://arxiv.org/abs/2305.14795) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**In-Context Demonstration Selection with Cross Entropy Difference**](https://arxiv.org/abs/2305.14726) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Abductive Commonsense Reasoning Exploiting Mutually Exclusive Explanations**](https://arxiv.org/abs/2305.14618) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Unraveling ChatGPT: A Critical Analysis of AI-Generated Goal-Oriented Dialogues and Annotations**](https://arxiv.org/abs/2305.14556) （**2023.05.23**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)


</div>

👉[Complete paper list 🔗 for "Prompt Application"](./PaperList/promptapplication.md)👈

## Foundation Models

<div style="line-height:0.2em;">



[**Peek Across: Improving Multi-Document Modeling via Cross-Document Question-Answering**](https://arxiv.org/abs/2305.15387) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**LLMDet: A Large Language Models Detection Tool**](https://arxiv.org/abs/2305.15004) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**OverPrompt: Enhancing ChatGPT Capabilities through an Efficient In-Context Learning Approach**](https://arxiv.org/abs/2305.14973) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**PESCO: Prompt-enhanced Self Contrastive Learning for Zero-shot Text Classification**](https://arxiv.org/abs/2305.14963) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Frugal Prompting for Dialog Models**](https://arxiv.org/abs/2305.14919) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Machine Reading Comprehension using Case-based Reasoning**](https://arxiv.org/abs/2305.14815) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**MQuAKE: Assessing Knowledge Editing in Language Models via Multi-Hop Questions**](https://arxiv.org/abs/2305.14795) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**In-Context Demonstration Selection with Cross Entropy Difference**](https://arxiv.org/abs/2305.14726) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Abductive Commonsense Reasoning Exploiting Mutually Exclusive Explanations**](https://arxiv.org/abs/2305.14618) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Unraveling ChatGPT: A Critical Analysis of AI-Generated Goal-Oriented Dialogues and Annotations**](https://arxiv.org/abs/2305.14556) （**2023.05.23**）

![](https://img.shields.io/badge/Citations-0-green)  ![](https://img.shields.io/badge/Mendeley%20Readers-1-red)


</div>

👉[Complete paper list 🔗 for "Foundation Models"](./PaperList/foundationmodels.md)👈

<!-- ### 📌 Hard Prompt/ Discrete Prompt

<div style="line-height:0.2em;">



[**LLMDet: A Large Language Models Detection Tool**](https://arxiv.org/abs/2305.15004) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**OverPrompt: Enhancing ChatGPT Capabilities through an Efficient In-Context Learning Approach**](https://arxiv.org/abs/2305.14973) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**PESCO: Prompt-enhanced Self Contrastive Learning for Zero-shot Text Classification**](https://arxiv.org/abs/2305.14963) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**In-Context Demonstration Selection with Cross Entropy Difference**](https://arxiv.org/abs/2305.14726) （**2023.05.24**）

![](https://img.shields.io/badge/Citations-0-green)

[**Cross-functional Analysis of Generalisation in Behavioural Learning**](https://arxiv.org/abs/2305.12951) （**2023.05.22**）

![](https://img.shields.io/badge/Citations-0-green)

[**Enhancing Cross-lingual Natural Language Inference by Soft Prompting with Multilingual Verbalizer**](https://arxiv.org/abs/2305.12761) （**2023.05.22**）

![](https://img.shields.io/badge/Citations-0-green)

[**A Benchmark on Extremely Weakly Supervised Text Classification: Reconcile Seed Matching and Prompting Approaches**](https://arxiv.org/abs/2305.12749) （**2023.05.22**）

![](https://img.shields.io/badge/Citations-0-green)

[**LogiCoT: Logical Chain-of-Thought Instruction-Tuning Data Collection with GPT-4**](https://arxiv.org/abs/2305.12147) （**2023.05.20**）

![](https://img.shields.io/badge/Citations-0-green)  [![](https://img.shields.io/badge/Github%20Stars-10-blue)](https://github.com/csitfun/logicot)

[**SelfzCoT: a Self-Prompt Zero-shot CoT from Semantic-level to Code-level for a Better Utilization of LLMs**](https://doi.org/10.48550/arXiv.2305.11461) （**2023.05.19**）

![](https://img.shields.io/badge/Citations-0-green)

[**Controlling the Extraction of Memorized Data from Large Language Models via Prompt-Tuning**](https://doi.org/10.48550/arXiv.2305.11759) （**2023.05.19**）

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