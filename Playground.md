# 🔥 Playground
> **Prompt Engineering aims to carefully curate input prompts that can extract the best possible results from Large language models(LLMs).** 

🌟 [TrustGPT](https://trustgpt.co/trust/index.html) can also serve as a playground for everyone's convenience to learn and practice advanced prompt techniques. You can also commit your issues from TrustGPT to this repo page. Thanks a lot.

We will gradually release the following features: 
1. Prompt example 
2. Question answering over your own document
3. Autonomous agent 
4. Access to various LLMs 

As resources are limited, we suggest using this playground for learning and practicing prompt techniques rather than for work. This will help more people access prompt engineering.

### 🌀 <font size=6>A</font>s a prominent example of LLMs, ChatGPT has received widespread attention and skyrocketed in popularity. Nonetheless, in recent years, a significant number of LLMs have emerged, typically several tens of gigabytes in size and trained on massive amounts of textual data. Therefore, there are several alternatives available that we can use to practice prompt techniques using these models.

<img width="200%" src="./figures/hr.gif" />


### 🤩 *The models in the table below are directly accessible via links, The page contains the usage guide and API interface of the model for the convenience of all developers and researchers to expolre and experience.*

|   Model  | Type | Lab | Playgrounds| Parameters(B) |Paper/Code|Announced Time|
| ---- | ---- | ----  | ---- | ---- |----|----|
| oasst-sft-6-llama-30b | Decoder| HuggingFace | [🔗](https://huggingface.co/chat/) | 30 |-/[Code](https://huggingface.co/OpenAssistant/oasst-sft-6-llama-30b-xor)|Apr-27|
| OpenAssistant | Decoder| LAION AI  | [🔗](https://open-assistant.io/chat) | - |[Paper](https://drive.google.com/file/d/10iR5hKwFqAKhL3umx8muOWSRm7hs5FqX/view )/[Code](https://github.com/LAION-AI/Open-Assistant)|Apr-17|
| GPT-4 | Decoder| OpenAI | [🔗](https://openai.com/waitlist/gpt-4-api) | 20 |[Paper](https://cdn.openai.com/papers/gpt-4.pdf)/-|Mar-14|
| OpenChatKit | Decoder| Together | [🔗](https://huggingface.co/spaces/togethercomputer/OpenChatKit) | 20 |-/[Code](https://github.com/togethercomputer/OpenChatKit)|Mar-13|
| Alpaca | Decoder| Stanford | [🔗](https://alpaca-ai-custom1.ngrok.io/) | 7 |-/[Code](https://github.com/tatsu-lab/stanford_alpaca)|Mar-13|
| ChatGPT | Decoder| OpenAI | [🔗](https://platform.openai.com/playground) | 175 |[Paper](https://arxiv.org/abs/2005.14165)/-|Nov-22|
| GPT-JT | Decoder | Together | [🔗](https://huggingface.co/spaces/togethercomputer/GPT-JT) | 6 |-/[Code](https://huggingface.co/togethercomputer/GPT-JT-6B-v1)|Nov-22|
| Flan-T5 | Encoder-Decoder | Google Research | [🔗](https://huggingface.co/google/flan-t5-xxl?text=Please+answer+the+following+question+What+is+the+boiling+point+of+Nitrogen%3F) | 11|[Paper](https://arxiv.org/abs/2210.11416)/[Code](https://huggingface.co/google/flan-t5-xxl/tree/main)|Oct-22|
| Flan-UL2 | Encoder-Decoder | Google Research | [🔗](https://huggingface.co/google/flan-ul2#citation) | 20|[Paper](https://arxiv.org/pdf/2205.05131v1.pdf)/[Code](https://github.com/google-research/google-research/tree/master/ul2)|Oct-22|
| CodeGeeX | Decoder | Tsinghua | [🔗](https://huggingface.co/spaces/THUDM/CodeGeeX) | 13 | -/[Code](https://github.com/THUDM/CodeGeeX)|Sep-22|
| GLM-130B | Encoder-Decoder | Tsinghua & Zhipu | [🔗](https://huggingface.co/spaces/THUDM/GLM-130B) | 130 |[Paper](https://arxiv.org/abs/2210.02414)/[Code](https://huggingface.co/spaces/THUDM/GLM-130B)|Aug-22|
| BLOOM(tr11-176B-ml) | Decoder | BigScience | [🔗](https://huggingface.co/spaces/huggingface/bloom_demo) | 176|-/[Code](https://github.com/bigscience-workshop/bigscience/tree/master/train/tr11-176B-ml)|Jul-22|
| PaLM | Decoder | Google Research | [🔗](https://cloud.google.com/vertex-ai) | 540|[Paper](https://developers.googleblog.com/2023/03/announcing-palm-api-and-makersuite.html)/-|Apr-22|
| CodeT5 | Encoder-Decoder | Salesforce Research Asia | [🔗](https://huggingface.co/Salesforce/codet5-base) | small:0.06,base:0.22|[Paper](https://arxiv.org/abs/2109.00859)/-|Mar-22|
| ERNIE3.0 | Encoder-Decoder | Baidu | [🔗](https://huggingface.co/swtx/ernie-3.0-base-chinese) | 10|[Paper](https://arxiv.org/abs/2112.12731)/-|Dec-21|
| CodeX | Decoder | OpenAI | [🔗](https://platform.openai.com/playground) | 12|[Paper](https://arxiv.org/abs/2107.03374)/-|Aug-21|
| GPT-3 | Decoder | OpenAI | [🔗](https://huggingface.co/models?sort=downloads&search=gpt3) | 175|[Paper](https://arxiv.org/abs/2005.14165)/-|May-20|
| T5 | Encoder-Decoder | Google | [🔗](https://huggingface.co/t5-base) | 11|[Paper](https://arxiv.org/abs/1910.10683)/-|Oct-19|
| RoBERTa | Encoder | MetaAI | [🔗](https://huggingface.co/xlm-roberta-base) | 0.355|[Paper](https://arxiv.org/abs/1907.11692)/-|Jul-19|
| GPT-2 | Decoder| OpenAI | [🔗](https://huggingface.co/openai-gpt) | 1.5|[Paper](https://d4mucfpksywv.cloudfront.net/better-language-models/language_models_are_unsupervised_multitask_learners.pdf)/-|Feb-19|
| BERT | Encoder | Google | [🔗](https://huggingface.co/bert-base-uncased) | 0.3|[Paper](https://arxiv.org/abs/1810.04805)/-|Oct-18|
| GPT-1 | Decoder| OpenAI | [🔗](https://huggingface.co/models) | 0.117|[Paper](https://gwern.net/doc/www/s3-us-west-2.amazonaws.com/d73fdc5ffa8627bce44dcda2fc012da638ffb158.pdf)/-|Jun-18|



<img width="200%" src="./figures/hr.gif" />

## 🤨 *The models in the table below all provide pre-trained weights on which developers can fine-tune (without changing the original backbone architecture), and people can visually see the work of a good team of researchers by using the pre-trained weights of the models directly for a good Demo.*

| Model  | Type | Lab | Github| Parameters(B) |Paper/Code|Announced Time|
| ---- | ---- | ----  | ---- | ---- |----|----|
| LLaMA-65B| Decoder | MetaAI | [🔗](https://research.facebook.com/publications/llama-open-and-efficient-foundation-language-models/) | 65|[Paper](https://scontent-hkg4-1.xx.fbcdn.net/v/t39.8562-6/333078981_693988129081760_4712707815225756708_n.pdf?_nc_cat=108&ccb=1-7&_nc_sid=ad8a9d&_nc_ohc=4srK2r5szdYAX8tuGSV&_nc_ht=scontent-hkg4-1.xx&oh=00_AfAUdcLc_-aVJHTm60I_1mIOLIEcecJ1N9s8-G4drVrd3Q&oe=6409B2E2)/[Code](https://github.com/facebookresearch/llama)|Feb-23|
| OPT-IML | Decoder| MetaAI | [🔗](https://github.com/facebookresearch/metaseq/tree/main/projects/OPT-IML) | 175|[Paper](https://arxiv.org/pdf/2212.12017.pdf)/-|Dec-22|
| ERNIE-Code | Encoder-Decoder | Baidu | [🔗](https://github.com/thunlp/ERNIE) | 0.56|[Paper](https://arxiv.org/abs/2212.06742#baidu)/-|Dec-22|
| Galactica | Decoder| MetaAI | [🔗](https://galactica.org/) | 120|[Paper](https://galactica.org/static/paper.pdf)/-|Nov-22|
| mT0 | Encoder-Decoder | BigScience | [🔗](https://github.com/bigscience-workshop/xmtf) | 13|[Paper](https://arxiv.org/abs/2211.01786)/-|Nov-22|
| BLOOMZ | Decoder | BigScience | [🔗](https://github.com/bigscience-workshop/xmtf)| 176|[Paper](https://arxiv.org/abs/2211.01786)/-|Nov-22|
| Atlas | Encoder-Decoder | MetaAI | [🔗](https://github.com/facebookresearch/atlas) | 11|[Paper](https://arxiv.org/abs/2208.03299)/-|Aug-22|
| OPT-175B | Decoder  | MetaAI | [🔗](https://huggingface.co/docs/transformers/model_doc/opt)| 175|[Paper](https://arxiv.org/abs/2205.01068)/-|May-22|
| GPT-NeoX-20B | Decoder | EleutherAI | [🔗](https://huggingface.co/docs/transformers/model_doc/gpt_neox) | 20|[Paper](https://arxiv.org/abs/2204.06745)/-|Feb-22|
| RETRO | Encoder-Decoder | DeepMind | [🔗](https://github.com/lucidrains/RETRO-pytorch) | 7.5|[Paper](https://arxiv.org/abs/2112.04426)/-|Dec-21|
| FLAN | Encoder-Decoder | Google | [🔗](https://github.com/google-research/FLAN) | 137|[Paper](https://arxiv.org/abs/2109.01652)/-|Sep-21|

<img width="200%" src="./figures/hr.gif" />

## 😣 *The following table show that the related models and codes are not open-source till now.*

| Model  | Type | Lab | Report| Parameters(B) |Paper/Code|Announced Time|
| ---- | ---- | ----  | ---- | ---- |----|----|
| Med-PaLM | Encoder | Google & DeepMind | [🔗](https://gpt3demo.com/apps/med-palm) | 540|[Paper](https://arxiv.org/abs/2212.13138)/-|Dec-22|
| GLaM | Encoder | Google Inc | [🔗](https://ai.googleblog.com/2021/12/more-efficient-in-context-learning-with.html) | 1200|[Paper](https://arxiv.org/abs/2112.06905)/-|Dec-22|
| RL-CAI | Encoder| Anthropic | [🔗](https://lifearchitect.ai/anthropic/) | 52|[Paper](https://arxiv.org/abs/2212.08073)/-|Dec-22|
| Sparrow | Decoder | DeepMind | [🔗](https://www.deepmind.com/blog/building-safer-dialogue-agents) | 70|[Paper](https://storage.googleapis.com/deepmind-media/DeepMind.com/Authors-Notes/sparrow/sparrow-final.pdf)/-|Sep-22|
| PaLI | Encoder-Decoder | Google | [🔗](https://ai.googleblog.com/2022/09/pali-scaling-language-image-learning-in.html) | 17|[Paper](https://arxiv.org/abs/2209.06794)/-|Sep-22|
| Gato(Cat) | Encoder-Decoder | DeepMind | [🔗](https://www.deepmind.com/blog/a-generalist-agent) | 1|[Paper](https://storage.googleapis.com/deepmind-media/A%20Generalist%20Agent/Generalist%20Agent.pdf)/-|May-22|
| Chinchilla | Encoder | DeepMind | [🔗](https://deepmind.github.io/dramatron/details.html) | 70|[Paper](https://arxiv.org/abs/2203.15556)/-|Mar-22|
| Gopher | Encoder  | DeepMind | [🔗](https://www.deepmind.com/blog/language-modelling-at-scale-gopher-ethical-considerations-and-retrieval) | 280|[Paper](https://arxiv.org/abs/2112.11446)/-|Dec-21|
| LaMDA | Decoder | GoogleAI |[🔗](https://www.youtube.com/watch?v=aUSSfo5nCdM)| 137|[Paper](https://arxiv.org/abs/2201.08239)/-|Jun-21|

