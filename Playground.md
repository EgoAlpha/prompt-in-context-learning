# 🔥 Playground
> **Prompt Engineering aims to carefully curate input prompts that can extract the best possible results from Large language models(LLMs).** 

### 🌀 <font size=6>A</font>s a prominent example of LLMs, ChatGPT has received widespread attention and skyrocketed in popularity. Nonetheless, in recent years, a significant number of LLMs have emerged, typically several tens of gigabytes in size and trained on massive amounts of textual data. Therefore, there are several alternatives available that we can use to practice prompt techniques using these models.

<img width="200%" src="./figures/hr.gif" />

## 📜 Table of Contents
- [TrustGPT From EgoAlpha](#trustgpt)
- [Directly Usage of LLMs](#directly-usage-of-llms)
- [Providing the Pre-train Weights](#providing-the-pre-train-weights)
- [Without Opensource Till Now](#without-opensource-till-now)
- [LLMs in Coding](#llms-in-coding)
- [Dataset in LLMs area](#dataset-in-llms-area)
- [LLMs from China](#llms-from-china)

<img width="200%" src="./figures/hr.gif" />

<div align="center">
<img src="./figures/TrustGPT.png" width="600px">
</div>

## TrustGPT
🌟 [TrustGPT](https://trustgpt.co/trust/index.html) can also serve as a playground for everyone's convenience to learn and practice advanced prompt techniques. You can also commit your issues from TrustGPT to this repo page. Thanks a lot.

We will gradually release the following features: 
1. Prompt example 
2. Question answering over your own document
3. Autonomous agent 
4. Access to various LLMs 

As resources are limited, we suggest using this playground for learning and practicing prompt techniques rather than for work. This will help more people access prompt engineering.

<img width="200%" src="./figures/hr.gif" />

## Directly Usage of LLMs
### 🤩 *These models in the table below are directly accessible via links, The page contains the usage guide and API interface of the model for the convenience of all developers and researchers to explore and experience. The Checkpoints can also obtained by corresponding links.*

|   Model  | Type | Lab | Playgrounds| Params(B) | Blog/Paper/Github | Checkpoints |Announced Time|
| :----: | :----: | :----:  | :----: | :----:|:----: |:----:|:----:|
| Gemma | Decoder| Google | [🔗](https://www.kaggle.com/models/google/gemma) | 2,7 |[Github]()|[Gemma-2B](https://huggingface.co/google/gemma-2b)/[Gemma-7B](https://huggingface.co/google/gemma-7b)|Feb-24|
| Yi series | Decoder| 01.Ai | [🔗](https://huggingface.co/01-ai/Yi-34B) | 6,34 |[Github](https://github.com/01-ai/Yi)|[Yi-34B](https://huggingface.co/01-ai/Yi-34B)/[Yi-6B](https://huggingface.co/01-ai/Yi-6B)|Nov-23|
| InternLM | Decoder| Shanghai Artificial Intelligence Laboratory | [🔗](https://huggingface.co/internlm/internlm-20b) | 20 |[Github](https://github.com/InternLM/InternLM)|[InternLM-20B](https://huggingface.co/internlm/internlm-chat-20b)|Aug-23|
| Mistral 7B | Decoder| | [🔗](https://huggingface.co/mistralai/Mistral-7B-v0.1) | 7 |[Paper](https://arxiv.org/pdf/2310.06825.pdf)/[Blog](https://mistral.ai/news/announcing-mistral-7b/)|[Mistral-7B-v0.1](https://huggingface.co/mistralai/Mistral-7B-v0.1)|Oct-23|
| Llama-2 | Decoder| Meta | [🔗](https://ai.meta.com/llama/#inside-the-model) | 7,13,70 |[Github](https://github.com/facebookresearch/llama)/[Paper](https://ai.meta.com/research/publications/llama-2-open-foundation-and-fine-tuned-chat-models/ )/[Blog](https://ai.meta.com/resources/models-and-libraries/llama-downloads/)|[Llama-7B, Llama-13B, Llama-70B](https://ai.meta.com/llama/#inside-the-model)|Jul-23|
| TigerBot | Decoder| - | [🔗](https://huggingface.co/TigerResearch/tigerbot-70b-base) | 70 |[Github](https://github.com/TigerResearch/TigerBot)|[TigerBot-70B](https://huggingface.co/TigerResearch/tigerbot-70b-base)|Jun-23|
| Falcon | Decoder| TII | [🔗](https://huggingface.co/tiiuae) | 1,7,40 |[Blog](https://falconllm.tii.ae/)|[Falcon-40B-instruct](https://huggingface.co/tiiuae/falcon-40b), [Falcon-7B-instruct](https://huggingface.co/tiiuae/falcon-7b-instruct),[Falcon-RW-1B](https://huggingface.co/tiiuae/falcon-rw-1b),[Falcon-RW-7B](https://huggingface.co/tiiuae/falcon-rw-7b)|May-23|
| GPT-J-6B | Decoder| EleutherAI | [🔗](https://github.com/EleutherAI/pythia) | 6 |[Blog](https://arankomatsuzaki.wordpress.com/2021/06/04/gpt-j/)|[GPT-J-6B](https://github.com/kingoflolz/mesh-transformer-jax/#gpt-j-6b), [GPT4All-J](https://github.com/nomic-ai/gpt4all#raw-model)|May-23|
| DLite | Decoder| EleutherAI | [🔗](https://github.com/EleutherAI/pythia) | 0.124-1.5 |[Blog](https://medium.com/ai-squared/announcing-dlite-v2-lightweight-open-llms-that-can-run-anywhere-a852e5978c6e)|[dlite-v2-1_5b](https://huggingface.co/aisquared/dlite-v2-1_5b)|May-23|
| OpenLLaMA | Decoder| H2O.AI | [🔗](https://huggingface.co/h2oai) | 3,7 |[Github](https://github.com/openlm-research/open_llama)|[OpenLLaMA-7b-preview-300bt](https://huggingface.co/openlm-research/open_llama_7b_preview_300bt)|May-23|
| RedPajama-INCITE | Decoder| Together | [🔗](https://huggingface.co/togethercomputer/RedPajama-INCITE-Instruct-7B-v0.1/blob/157bf3174feebb67f37e131ea68f84dee007c687/config.json#L13) | 3-7 |[Blog](https://www.together.xyz/blog/redpajama-models-v1)|[RedPajama-INCITE](https://huggingface.co/togethercomputer)|May-23|
| MPT-7B  | Decoder| mosaic | [🔗](https://huggingface.co/mosaicml/mpt-7b#how-is-this-model-different) | 7 |[Blog](https://www.mosaicml.com/blog/mpt-7b)|[MPT-7B](https://huggingface.co/mosaicml/mpt-7b), [MPT-7B-Instruct](https://huggingface.co/mosaicml/mpt-7b-instruct)|May-23|
| h2oGPT | Decoder| EleutherAI | [🔗](https://huggingface.co/h2oai) | 12-20 |[Blog](https://h2o.ai/blog/building-the-worlds-best-open-source-large-language-model-h2o-ais-journey/)|[h2oGPT](https://github.com/h2oai/h2ogpt)|May-23|
| Dolly | Decoder| EleutherAI | [🔗](https://github.com/EleutherAI/pythia) | 3,7,12 |[Blog](https://www.databricks.com/blog/2023/04/12/dolly-first-open-commercially-viable-instruction-tuned-llm)/[Github](https://github.com/databrickslabs/dolly#dolly)|[dolly-v2-12b](https://huggingface.co/databricks/dolly-v2-12b)|Apr-23|
| Pythia | Decoder| EleutherAI | [🔗](https://github.com/EleutherAI/pythia) | 0.07-12 |[Paper](https://arxiv.org/abs/2304.01373)/[Github](https://github.com/EleutherAI/pythia)|[pythia 70M - 12B](https://github.com/EleutherAI/pythia)|Apr-23|
| FastChat-T5 | Decoder| EleutherAI | [🔗](https://github.com/EleutherAI/pythia) | 3 |[Blog](https://twitter.com/lmsysorg/status/1652037026705985537?s=20)|[fastchat-t5-3b-v1.0](https://huggingface.co/lmsys/fastchat-t5-3b-v1.0)|Apr-23|
| StableLM-Alpha | Decoder| EleutherAI | [🔗](https://stability.ai/blog/stability-ai-launches-the-first-of-its-stablelm-suite-of-language-models)| 3-65 |[Github](https://github.com/Stability-AI/StableLM#stablelm-alpha)|[StableLM-Alpha](https://github.com/Stability-AI/StableLM#stablelm-alpha)|Apr-23|
| oasst-sft-6-llama-30b | Decoder| HuggingFace | [🔗](https://huggingface.co/chat/) | 30 |[Github](https://huggingface.co/OpenAssistant/oasst-sft-6-llama-30b-xor)|-|Apr-23|
| Cerebras-GPT | Decoder| HuggingFace | [🔗](https://huggingface.co/cerebras/) | 0.111-13 |[Paper](https://arxiv.org/abs/2304.03208)|[Cerebras-GPT: A Family of Open, Compute-efficient, Large Language Models](https://www.cerebras.net/blog/cerebras-gpt-a-family-of-open-compute-efficient-large-language-models/)|Mar-23|
| OpenAssistant(Pythia family) | Decoder| LAION AI  | [🔗](https://open-assistant.io/chat) | 12 |[Paper](https://drive.google.com/file/d/10iR5hKwFqAKhL3umx8muOWSRm7hs5FqX/view )/[Github](https://github.com/LAION-AI/Open-Assistant)|[OA-Pythia-12B-SFT-8](https://huggingface.co/OpenAssistant/pythia-12b-sft-v8-7k-steps), [OA-Pythia-12B-SFT-4](https://huggingface.co/OpenAssistant/oasst-sft-4-pythia-12b-epoch-3.5), [OA-Pythia-12B-SFT-1](https://huggingface.co/OpenAssistant/oasst-sft-1-pythia-12b)|Apr-23|
| GPT-4 | Decoder| OpenAI | [🔗](https://openai.com/waitlist/gpt-4-api) | 20 |[Paper](https://cdn.openai.com/papers/gpt-4.pdf)|-|Mar-23|
| OpenChatKit | Decoder| Together | [🔗](https://huggingface.co/spaces/togethercomputer/OpenChatKit) | 20 |[Github](https://github.com/togethercomputer/OpenChatKit)|-|Mar-23|
| Alpaca | Decoder| Stanford | [🔗](https://alpaca-ai-custom1.ngrok.io/) | 7 |[Github](https://github.com/tatsu-lab/stanford_alpaca)|-|Mar-23|
| ChatGPT | Decoder| OpenAI | [🔗](https://platform.openai.com/playground) | 175 |[Paper](https://arxiv.org/abs/2005.14165)|-|Nov-22|
| GPT-JT | Decoder | Together | [🔗](https://huggingface.co/spaces/togethercomputer/GPT-JT) | 6 |[Github](https://huggingface.co/togethercomputer/GPT-JT-6B-v1)|-|Nov-22|
| Flan-T5 | Encoder-Decoder | Google Research | [🔗](https://huggingface.co/google/flan-t5-xxl?text=Please+answer+the+following+question+What+is+the+boiling+point+of+Nitrogen%3F) | 11|[Paper](https://arxiv.org/abs/2210.11416)/[Github](https://huggingface.co/google/flan-t5-xxl/tree/main)|[Flan-T5](https://github.com/google-research/t5x/blob/main/docs/models.md#flan-t5-checkpoints)|Oct-22|
| Flan-UL2 | Encoder-Decoder | Google Research | [🔗](https://huggingface.co/google/flan-ul2#citation) | 20|[Paper](https://arxiv.org/pdf/2205.05131v1.pdf)/[Github](https://github.com/google-research/google-research/tree/master/ul2)|[Flan-UL2](https://github.com/google-research/google-research/tree/master/ul2#checkpoints)|Oct-22|
| CodeGeeX | Decoder | Tsinghua | [🔗](https://huggingface.co/spaces/THUDM/CodeGeeX) | 13 | [Github](https://github.com/THUDM/CodeGeeX)|[CodeGeeX register path](https://models.aminer.cn/codegeex/download/request)|Sep-22|
| GLM-130B | Encoder-Decoder | Tsinghua & Zhipu | [🔗](https://huggingface.co/spaces/THUDM/GLM-130B) | 130 |[Paper](https://arxiv.org/abs/2210.02414)/[Github](https://huggingface.co/spaces/THUDM/GLM-130B)|-|Aug-22|
| BLOOM(tr11-176B-ml) | Decoder | BigScience | [🔗](https://huggingface.co/spaces/huggingface/bloom_demo) | 176|[Github](https://github.com/bigscience-workshop/bigscience/tree/master/train/tr11-176B-ml)|[BLOOM](https://huggingface.co/bigscience/bloom)|Jul-22|
| PaLM | Decoder | Google Research | [🔗](https://cloud.google.com/vertex-ai) | 540|[Paper](https://developers.googleblog.com/2023/03/announcing-palm-api-and-makersuite.html)|-|Apr-22|
| GPT-NeoX-20B | Decoder | EleutherAI | [🔗](https://huggingface.co/EleutherAI/gpt-neox-20b) | 20|[Paper](https://arxiv.org/abs/2304.04165)|[GPT-NEOX-20B](https://huggingface.co/EleutherAI/gpt-neox-20b)|Apr-22|
| CodeT5 | Encoder-Decoder | Salesforce Research Asia | [🔗](https://huggingface.co/Salesforce/codet5-base) | small:0.06,base:0.22|[Paper](https://arxiv.org/abs/2109.00859)|-|Mar-22|
| ERNIE3.0 | Encoder-Decoder | Baidu | [🔗](https://huggingface.co/swtx/ernie-3.0-base-chinese) | 10|[Paper](https://arxiv.org/abs/2112.12731)|-|Dec-21|
| CodeX | Decoder | OpenAI | [🔗](https://platform.openai.com/playground) | 12|[Paper](https://arxiv.org/abs/2107.03374)|-|Aug-21|
| RWKV | Decoder | OpenAI | [🔗](https://platform.openai.com/playground) | 0.1-14|[Github](https://github.com/BlinkDL/RWKV-LM)|[RWKV, ChatRWKV](https://github.com/BlinkDL/RWKV-LM#rwkv-parallelizable-rnn-with-transformer-level-llm-performance-pronounced-as-rwakuv-from-4-major-params-r-w-k-v)|Aug-21|
| GPT-3 | Decoder | OpenAI | [🔗](https://huggingface.co/models?sort=downloads&search=gpt3) | 175|[Paper](https://arxiv.org/abs/2005.14165)|-|May-20|
| T5 | Encoder-Decoder | Google | [🔗](https://huggingface.co/t5-base) | 11|[Paper](https://arxiv.org/abs/1910.10683)|[T5](https://github.com/google-research/t5x/blob/main/docs/models.md#flan-t5-checkpoints)|Oct-19|
| RoBERTa | Encoder | MetaAI | [🔗](https://huggingface.co/xlm-roberta-base) | 0.355|[Paper](https://arxiv.org/abs/1907.11692)|[roberta-series](https://huggingface.co/models?sort=downloads&search=RoBERTa)|Jul-19|
| GPT-2 | Decoder| OpenAI | [🔗](https://huggingface.co/openai-gpt) | 1.5|[Paper](https://d4mucfpksywv.cloudfront.net/better-language-models/language_models_are_unsupervised_multitask_learners.pdf)|[GPT_2 Series](https://huggingface.co/models?sort=downloads&search=GPT2)|Feb-19|
| BERT | Encoder | Google | [🔗](https://huggingface.co/bert-base-uncased) | 0.3|[Paper](https://arxiv.org/abs/1810.04805)|[BERT Series](https://huggingface.co/models?sort=downloads&search=BERT)|Oct-18|
| GPT-1 | Decoder| OpenAI | [🔗](https://huggingface.co/models) | 0.117|[Paper](https://gwern.net/doc/www/s3-us-west-2.amazonaws.com/d73fdc5ffa8627bce44dcda2fc012da638ffb158.pdf)|[GPT_1_seriers](https://huggingface.co/models?sort=downloads&search=GPT1)|Jun-18|

<img width="200%" src="./figures/hr.gif" />

## Providing the Pre-train weights
### 🤨 *The models in the table below all provide pre-trained weights on which developers can fine-tune (without changing the original backbone architecture), and people can visually see the work of a good team of researchers by using the pre-trained weights of the models directly for a good Demo.*

| Model  | Type | Lab | Github| Params(B) |Paper/Code|Announced Time|
| :----: | :----: | :----:  | :----: | :----: |:----:|:----:|
| Gorilla-OpenFunctions series | Decoder| Gorilla LLM | [🔗](https://huggingface.co/gorilla-llm/gorilla-openfunctions-v2) | - |[Paper](https://arxiv.org/abs/2305.15334)/[Github](https://gorilla.cs.berkeley.edu/leaderboard)|-|May-23|
| LLaMA-65B| Decoder | MetaAI | [🔗](https://research.facebook.com/publications/llama-open-and-efficient-foundation-language-models/) | 65|[Paper](https://scontent-hkg4-1.xx.fbcdn.net/v/t39.8562-6/333078981_693988129081760_4712707815225756708_n.pdf?_nc_cat=108&ccb=1-7&_nc_sid=ad8a9d&_nc_ohc=4srK2r5szdYAX8tuGSV&_nc_ht=scontent-hkg4-1.xx&oh=00_AfAUdcLc_-aVJHTm60I_1mIOLIEcecJ1N9s8-G4drVrd3Q&oe=6409B2E2)/[Code](https://github.com/facebookresearch/llama)|Feb-23|
| OPT-IML | Decoder| MetaAI | [🔗](https://github.com/facebookresearch/metaseq/tree/main/projects/OPT-IML) | 175|[Paper](https://arxiv.org/pdf/2212.12017.pdf)/-|Dec-22|
| ERNIE-Code | Encoder-Decoder | Baidu | [🔗](https://github.com/thunlp/ERNIE) | 0.56|[Paper](https://arxiv.org/abs/2212.06742#baidu)/-|Dec-22|
| Galactica | Decoder| MetaAI | [🔗](https://galactica.org/) | 120|[Paper](https://galactica.org/static/paper.pdf)/-|Nov-22|
| mT0 | Encoder-Decoder | BigScience | [🔗](https://github.com/bigscience-workshop/xmtf) | 13|[Paper](https://arxiv.org/abs/2211.01786)/-|Nov-22|
| BLOOMZ | Decoder | BigScience | [🔗](https://github.com/bigscience-workshop/xmtf)| 176|[Paper](https://arxiv.org/abs/2211.01786)/-|Nov-22|
| Atlas | Encoder-Decoder | MetaAI | [🔗](https://github.com/facebookresearch/atlas) | 11|[Paper](https://arxiv.org/abs/2208.03299)/-|Aug-22|
| OPT-175B | Decoder  | MetaAI | [🔗](https://huggingface.co/docs/transformers/model_doc/opt)| 175|[Paper](https://arxiv.org/abs/2205.01068)/-|May-22|
| RETRO | Encoder-Decoder | DeepMind | [🔗](https://github.com/lucidrains/RETRO-pytorch) | 7.5|[Paper](https://arxiv.org/abs/2112.04426)/-|Dec-21|
| FLAN | Encoder-Decoder | Google | [🔗](https://github.com/google-research/FLAN) | 137|[Paper](https://arxiv.org/abs/2109.01652)/-|Sep-21|

<img width="200%" src="./figures/hr.gif" />

## Without Opensource Till Now
### 😣 *The following table show that the related models and codes are not open-source till now.*

| Model  | Type | Lab | Report| Params(B) |Paper/Code|Announced Time|
| :----: | :----: | :----:| :----: | :----: |:----:|:----:|
| Med-PaLM | Encoder | Google & DeepMind | [🔗](https://gpt3demo.com/apps/med-palm) | 540|[Paper](https://arxiv.org/abs/2212.13138)/-|Dec-22|
| GLaM | Encoder | Google Inc | [🔗](https://ai.googleblog.com/2021/12/more-efficient-in-context-learning-with.html) | 1200|[Paper](https://arxiv.org/abs/2112.06905)/-|Dec-22|
| RL-CAI | Encoder| Anthropic | [🔗](https://lifearchitect.ai/anthropic/) | 52|[Paper](https://arxiv.org/abs/2212.08073)/-|Dec-22|
| Sparrow | Decoder | DeepMind | [🔗](https://www.deepmind.com/blog/building-safer-dialogue-agents) | 70|[Paper](https://storage.googleapis.com/deepmind-media/DeepMind.com/Authors-Notes/sparrow/sparrow-final.pdf)/-|Sep-22|
| PaLI | Encoder-Decoder | Google | [🔗](https://ai.googleblog.com/2022/09/pali-scaling-language-image-learning-in.html) | 17|[Paper](https://arxiv.org/abs/2209.06794)/-|Sep-22|
| Gato(Cat) | Encoder-Decoder | DeepMind | [🔗](https://www.deepmind.com/blog/a-generalist-agent) | 1|[Paper](https://storage.googleapis.com/deepmind-media/A%20Generalist%20Agent/Generalist%20Agent.pdf)/-|May-22|
| Chinchilla | Encoder | DeepMind | [🔗](https://deepmind.github.io/dramatron/details.html) | 70|[Paper](https://arxiv.org/abs/2203.15556)/-|Mar-22|
| Gopher | Encoder  | DeepMind | [🔗](https://www.deepmind.com/blog/language-modelling-at-scale-gopher-ethical-considerations-and-retrieval) | 280|[Paper](https://arxiv.org/abs/2112.11446)/-|Dec-21|
| LaMDA | Decoder | GoogleAI |[🔗](https://www.youtube.com/watch?v=aUSSfo5nCdM)| 137|[Paper](https://arxiv.org/abs/2201.08239)/-|Jun-21|

<img width="200%" src="./figures/hr.gif" />

## LLMs in Coding
### 🎭 *The following table shows the LLMs for Coding.* 

| Model |  Checkpoints | Paper/Blog | Params (B)|Announced Time |
| :---: | :---: | :---: | :---: | :---: |
| StarCoder |  [starcoder](https://huggingface.co/bigcode/starcoder) | [Blog](https://huggingface.co/blog/starcoder) | 15 | May-23 |
| StarChat Alpha |  [starchat-alpha](https://huggingface.co/HuggingFaceH4/starchat-alpha) | [Blog](https://huggingface.co/blog/starchat-alpha) | 16 | May-23 |
| Replit Code |  [replit-code-v1-3b](https://huggingface.co/replit/replit-code-v1-3b) | [Blog](https://www.latent.space/p/reza-shabani#details) | 2.7 | May-23 |
| CodeT5+ |  [CodeT5+](https://github.com/salesforce/CodeT5/tree/main/CodeT5+)     | [Paper](https://arxiv.org/abs/2305.07922) | 0.22 - 16 | May-23 |
| CodeGen2 |  [codegen2 1B-16B](https://github.com/salesforce/CodeGen2) | [Paper](https://arxiv.org/abs/2305.02309) | 1 - 16 | Apr-23 |
| SantaCoder |  [santacoder](https://huggingface.co/bigcode/santacoder) |[Paper](https://arxiv.org/abs/2301.03988) | 1.1| Jan-23 |

<img width="200%" src="./figures/hr.gif" />

## Dataset in LLMs Area
### 📈 *The following table shows the Dataset of the LLM area, with instruction-tunning and alignment-tuning.*

| Dataset |   Paper/Blog | Dataset | Samples (K) | Announced Time |Type|
| :---: | :---: | :---: | :---: | :---: | :---:|
| MPT-7B-Instruct |  [Blog](https://www.mosaicml.com/blog/mpt-7b) | [dolly_hhrlhf](https://huggingface.co/datasets/mosaicml/dolly_hhrlhf) | 59 | May-23 |instruction-tuning|
| databricks-dolly-15k |  [Blog](https://www.databricks.com/blog/2023/04/12/dolly-first-open-commercially-viable-instruction-tuned-llm) |  [databricks-dolly-15k](https://huggingface.co/datasets/databricks/databricks-dolly-15k) | 15 |  Apr-23 |instruction-tuning|
| OpenAssistant Conversations Dataset |  [Blog](https://drive.google.com/file/d/10iR5hKwFqAKhL3umx8muOWSRm7hs5FqX/view) | [oasst1](https://huggingface.co/datasets/OpenAssistant/oasst1) | 161 |Apr-23 |alignment-tuning|
| OIG (Open Instruction Generalist)   |  [Blog](https://laion.ai/blog/oig-dataset/) | [OIG](https://huggingface.co/datasets/laion/OIG) | 44,000 | Mar-23 |instruction-tuning|

<img width="200%" src="./figures/hr.gif" />

## LLMs from China
### 🇨🇳 *The following table shows the LLMs from China, including the research lab, firms, and some universities.*

>Note： The part of contents of the list are from [here](https://github.com/wgwang/LLMs-In-China), and we have made appropriate modifications and supplements, hereby noted.

|Source|Model & Link|Description|
|:-:|:-:|:-:|
|复旦大学|[MOSS](https://github.com/OpenLMLab/MOSS)|[Playground](https://moss.fastnlp.top/)|
|贝壳|[BELLE](https://github.com/LianjiaTech/BELLE)|基于BLOOMZ或[LLaMA](https://mp.weixin.qq.com/s/dKInMi6P80GXecUtR3WQsA)系列的多个模型|
|哈尔滨工业大学|[本草](https://github.com/SCIR-HI/Huatuo-Llama-Med-Chinese)|医学；基于[LLaMA](https://mp.weixin.qq.com/s/dKInMi6P80GXecUtR3WQsA)；另有基于 ChatGLM 的[Med-ChatGLM](https://github.com/SCIR-HI/Med-ChatGLM)|
|云知声|[山海](https://shanhai.unisound.com/) |通用大模型|
|百度| [文心一言](https://yiyan.baidu.com)|[申请账号](https://yiyan.baidu.com)|
|科大讯飞|[星火](https://xinghuo.xfyun.cn)|[申请账号](https://xinghuo.xfyun.cn/desk) |
|清华大学|[ChatGLM](https://chatglm.cn/),[NowcastNet](https://www.nature.com/articles/s41586-023-06184-4)| [开源6B](https://github.com/THUDM/ChatGLM-6B)，[ChatGLM2-6B](https://github.com/THUDM/ChatGLM2-6B), [智谱AI](http://open.bigmodel.ai/),[气象,临近预报大模型](https://mp.weixin.qq.com/s/MwJWjCLNqJM3lZ33RwK4Bg)|
|华为|[盘古](https://openi.pcl.ac.cn/PCL-Platform.Intelligence/PanGu-Alpha),[盘古气象](https://www.nature.com/articles/s41586-023-06185-3),[盘古-Σ](https://arxiv.org/pdf/2303.10845.pdf)|华为+鹏城,[华为云盘古](https://www.huaweicloud.com/product/pangu.html)|
|达观数据|[曹植](http://www.datagrand.com/products/aigc/)|[试用需账号](https://aigc.datagrand.com/) |
|阿里云|[通义千问](https://tongyi.aliyun.com/)|[试用需账号]( https://tongyi.aliyun.com)|
|浙江大学|[启真](https://github.com/CMKRG/QiZhenGPT),[PromptProtein](https://github.com/HICAI-ZJU/PromptProtein)|医学大模型提供基于LLaMA-7B、CaMA-13B和ChatGLM-6B 三个版本,用于PromptProtein的[模型](https://github.com/HICAI-ZJU/OpenProtein)|
|百川智能|[baichuan-7B](https://github.com/baichuan-inc/baichuan-7B),[Baichuan-13B](https://github.com/baichuan-inc/Baichuan-13B)|模型下载：[Baichuan-13B-Base](https://huggingface.co/baichuan-inc/Baichuan-13B-Base),[Baichuan-13B-Chat](https://huggingface.co/baichuan-inc/Baichuan-13B-Chat),[Baichuan-7B](https://huggingface.co/baichuan-inc/Baichuan-7B),开源可商用|
|上海人工智能实验室|[书生·浦语](https://internlm.org/), [OpenMEDLab浦医](https://github.com/openmedlab) |[技术报告](https://github.com/InternLM/InternLM-techreport),[开源的InternLM-7B](https://github.com/InternLM/InternLM),[HuggingFace下载模型权重](https://huggingface.co/internlm/internlm-7b)|
|OpenBMB|[CPM](https://live.openbmb.org/),[CPM-Bee](https://github.com/OpenBMB/CPM-Bee)|[面壁智能](https://modelbest.cn/),[CPM-Bee-10B](https://huggingface.co/openbmb/cpm-bee-10b)|
|港中文深圳|[华佗](https://github.com/FreedomIntelligence/HuatuoGPT)，[凤凰](https://github.com/FreedomIntelligence/LLMZoo)|香港中文大学（深圳）和深圳市大数据研究院，医学,[Demo](https://www.huatuogpt.cn/),华佗和凤凰都基于BLOOMZ|
|中国科学院自动化研究所| [紫东·太初](https://gitee.com/zidongtaichu/multi-modal-models)|紫东太初2.0号称100B参数，全模态|
|虎博科技|[TigerBot](https://github.com/TigerResearch/TigerBot)|基于[BLOOM](https://mp.weixin.qq.com/s/ia-yrmXbnlooRA3K1hoTwQ)|
|东北大学|[TechGPT](https://github.com/neukg/TechGPT),[PICA](https://github.com/NEU-DataMining/PICA)|TechGPT->BELLE->[LLaMA](https://mp.weixin.qq.com/s/dKInMi6P80GXecUtR3WQsA)，图谱构建和阅读理解问答;PICA->ChatGLM2-6B情感大模型|
|上海交通大学|[K2](https://github.com/davendw49/k2),[白玉兰](https://mp.weixin.qq.com/s/3eON8L4b7-d-1URwgdR6Bg)|[Demo](https://k2.acemap.info/)，GeoLLaMA，基于[LLaMA](https://mp.weixin.qq.com/s/dKInMi6P80GXecUtR3WQsA)，[HuggingFace](https://huggingface.co/daven3/k2_it_adapter) |
|IDEA研究院|[封神榜MindBot](https://fengshenbang-lm.com/) |[姜子牙](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1.1)系列模型 |
|智源人工智能研究院|[悟道·天鹰](https://github.com/FlagAI-Open/FlagAI/tree/master/examples/Aquila),[悟道·EMU](https://github.com/baaivision/Emu)|悟道3.0,视界视觉，AQUILA天鹰座，[Aquila-7B](https://model.baai.ac.cn/model-detail/100098),[AquilaChat-7B](https://model.baai.ac.cn/model-detail/100101),[AquilaCode-7B-NV](https://model.baai.ac.cn/model-detail/100102),[AquilaCode-7B-TS](https://model.baai.ac.cn/model-detail/100099),[HuggingFace](https://huggingface.co/BAAI),[EMU](https://huggingface.co/BAAI/Emu)基于[LLaMA](https://mp.weixin.qq.com/s/dKInMi6P80GXecUtR3WQsA)|
|度小满|[轩辕](https://huggingface.co/xyz-nlp/XuanYuan2.0) |基于[BLOOM](https://mp.weixin.qq.com/s/ia-yrmXbnlooRA3K1hoTwQ)|
|23|360| [智脑](https://ai.360.cn/),[一见](https://github.com/360CVGroup/SEEChat)||
|艾写科技|[Anima](https://github.com/lyogavin/Anima)|基于Guanaco->基于[LLaMA](https://mp.weixin.qq.com/s/dKInMi6P80GXecUtR3WQsA)，使用QLoRA|
|西湖心辰|[西湖](https://xinchenai.com/)|通用大模型|
|晓多科技+国家超算成都中心|[晓模型XPT](https://www.xiaoduoai.com/blog/12433.html)|试用需要账号，[位置](https://www.xiaoduoai.com/x_model)|
|稀宇科技|[MiniMax](https://api.minimax.chat/)|GLOW虚拟社交|
|北京语言大学 |[桃李](https://github.com/blcuicall/taoli) |基于[LLaMA](https://mp.weixin.qq.com/s/dKInMi6P80GXecUtR3WQsA),北语+清华+东北、北京交大|
|商汤科技 | [SenseNova日日新](https://techday.sensetime.com/list)|商汤科技版ChatGPT |
|国家超级计算天津中心|[天河天元](https://mp.weixin.qq.com/s/A9jnnL3-LjcDLsDD2PCa6g)| 目前官网查询不到|
|星环科技|[无涯、求索](https://mp.weixin.qq.com/s/6rYmk58OypU_Wwu0L7-nTw)|无涯——金融；求索——大数据分析|
|慧言科技+天津大学|[海河·谛听](https://mp.weixin.qq.com/s/FCnXXmT0jRfk4tTRIAK9FA)| -|
|恒生电子|LightGPT|- |
|电信智科|[星河](https://mp.weixin.qq.com/s/ntd0z5CJOY6peou4bOVJqA)|通用视觉，中国电信|
|左手医生|[左医GPT](https://mp.weixin.qq.com/s/Tv9nIG_9K-Lf5AKatjichA)|医疗，[试用需Key](https://gpt.zuoshouyisheng.com/)|
|智慧眼|[砭石](https://mp.weixin.qq.com/s/lid0nUBwXEdoUhnw_guteA)|医疗领域|
|好未来|[MathGPT](https://mp.weixin.qq.com/s/evLrZAFKa9mCplcqZnpZMw)|学而思|
|数慧时空|[长城](https://mp.weixin.qq.com/s/KYB-noOt7gB0l5hh-rwfkQ)|自然资源，遥感|
|理想科技|大道Dao|运维大模型|
|硅基智能|[炎帝](https://mp.weixin.qq.com/s/XNu3UrSKm4jy1ayJJ6-HMg)|旅游行业大模型|
| 中工互联|[智工](https://mp.weixin.qq.com/s/ANsZeqj4V_NeVCquwX-aSQ)|与复旦NLP实验室联合，工业领域|
|创业黑马|[天启](https://mp.weixin.qq.com/s/lYqCe9skc0MOSzmmTiGAug) | 创业黑马与360合作,科创服务行业|
|追一科技|[博文Bowen](https://mp.weixin.qq.com/s/cYVh6K6edmColgMEOaGFKg) | -|
|上海科技大学|[DoctorGLM](https://github.com/xionghonglin/DoctorGLM)|医学大模型，[论文](https://arxiv.org/pdf/2304.01097.pdf)|
|华东师范大学 |[EmoGPT](https://mp.weixin.qq.com/s/xP-qm5YUj8fZD9YQ7t08NQ),[EduChat](https://github.com/icalk-nlp/EduChat)|EmoGPT是上海市心理健康与危机干预重点实验室与镜象科技公司合作完成, 教学教育大模型EduChat基于BELLE（BELLE基于LLaMA）|
|昆仑万维 | [天工](https://github.com/SkyWorkAIGC)|与奇点智源联合研发||
|智媒开源研究院| [智媒](https://github.com/IMOSR/Media-LLaMA)|基于LLaMA，面向自媒体|
|医疗算网|Uni-talk|上海联通+华山医院+上海超算中心+华为|
|蚂蚁集团|贞仪|据传语言和多模态两个|
|香港科技大学|[罗宾Robin](https://huggingface.co/OptimalScale)|基于[LLaMA](https://mp.weixin.qq.com/s/dKInMi6P80GXecUtR3WQsA),[港科大开源LMFlow](https://github.com/OptimalScale/LMFlow)|
|腾讯|混元|-|
|拓尔思|[拓天](https://mp.weixin.qq.com/s/beQardxjpner6vvk_LTOJA)| 中文通用大模型|
|乐言科技|乐言 | TRSGPT|
|清博智能 | [先问](https://mp.weixin.qq.com/s/Et-nVHjxDP3W-PFWmDo3YQ)|基于结构化数据|
|智子引擎 | [元乘象](https://chatimg.aixiaoqingxu.com/)|手机号快速登录，使用方便|
|拓世科技 |[拓世](https://tskjgroup.com/article_news?id=822)|[数万亿参数量，通用领域](https://tskjgroup.com/article_news?id=900)|
|循环智能| [盘古](https://www.rcrai.com/product/ai/pangu)|循环智能,清华大学,华为 |
|印象笔记|[大象GPT](https://mp.weixin.qq.com/s/O3nRSKBM29bCWKuRRi_PBg)| AGI智能化产品|
|第四范式|[式说](https://www.4paradigm.com/product/SageGPT.html)|以生成式AI重构企业软件（AI-Generated Software），提升企业软件的体验和开发效率。|
|字节跳动 |Grace|内部代号|
|出门问问|[序列猴子](https://write.mobvoi.com/)| AI写作助理大模型|
|数说故事|[SocialGPT](https://mp.weixin.qq.com/s/Tt3dcwefIvdlyB_IwaFYRQ)| 聚焦社交对话大模型|
|云从科技|[从容](https://www.cloudwalk.com/news/show/id/178)|通用大模型|
|浪潮信息|[源](https://air.inspur.com/) |论文支撑——[源](https://github.com/Shawn-Inspur/Yuan-1.0)|
|中国农业银行|[小数ChatABC](https://mp.weixin.qq.com/s/CXyZRIqhwrcGAKxzUC-qgg)|金融行业大模型 |
|麒麟合盛 |[天燕AiLMe](https://www.apusai.com/)| 需要账号登录，[登录位置](https://ailme.apusai.com/#/login)|
|台智云|[福尔摩斯FFM](https://tws.twcc.ai/afs/)|华硕子公司|
|医联科技|[medGPT](https://www.medlinker.com/news/198)| 国内首款AI医生|
|理想汽车|MindGPT| -|
|深思考人工智能|[Dongni](https://www.dongni.ai/)| 登录需要账号|
|长虹|长虹超脑 |-|
|孩子王|KidsGPT|- |
|中科闻歌|[雅意](https://mp.weixin.qq.com/s/IGYV3t3JRlq4quvNJmZ4vA)|媒体、金融、宣传等领域的大模型应用|
|中国联通 |鸿湖|-|
|思必驰|[DFM-2](https://mp.weixin.qq.com/s/FxLw5UfJpYS1tCPDMkhvXA)|通用大模型|
|中科创达|魔方Rubik| -|
|电科太极 |[小可](https://mp.weixin.qq.com/s/8ci7g7R9j3pxkQC4UOLh2A)|党政企行业应用 |
|中国移动|九天|-|
|中国电信|TeleChat|-|
|容联云|赤兔|客服，营销|
|云天励飞|天书|-|
|维智科技|CityGPT|城市大模型|
|澜舟科技| [孟子](https://www.langboat.com/portal/mengzi-model) |自研大规模预训练语言模型|
|京东|[言犀](https://www.jdcloud.com/cn/news/detail/1235)|面向不同过产业大模型|
|智臻智能|[华藏](https://mp.weixin.qq.com/s/MZO2tvun05WnJkSe0seJnw)|小i机器人|
|新华三H3C|百业灵犀|-|
|鹏城实验室|鹏城·脑海|Peng Cheng Mind|
|宇视科技|[梧桐](https://mp.weixin.qq.com/s/H8FsrEyJsIijy0Cowyu3GQ)|AIoT行业 |
|网易有道|子曰 |- |
|美亚柏科|[天擎](https://mp.weixin.qq.com/s/D3ki3G4Q7QZPAVJ8iwTvDg)|公共安全|
|赛灵力科技 |达尔文|赛灵力,清华珠三角研究院,赛业生物,大湾区科技创新服务中心|
|佳都科技 |佳都知行 |交通领域|
|知乎|知海图|知乎和面壁科技合作|
|实在智能 |塔斯| TARS|
|网易伏羲|玉言|- |
|北京大学信息工程学院|[ChatLaw](https://github.com/PKU-YuanGroup/ChatLaw)|[ChatLaw-13B](https://huggingface.co/JessyTsu1/ChatLaw-13B)基于Ziya-LLaMA-13B-v1->LLaMA,[ChatLaw-33B](https://huggingface.co/JessyTsu1/ChatLaw-33B)基于Anima33B->Guanaco->[LLaMA](https://mp.weixin.qq.com/s/dKInMi6P80GXecUtR3WQsA)|
|华南理工大学|[扁鹊](https://github.com/scutcyr/BianQue),[灵心SoulChat](https://github.com/scutcyr/SoulChat)|医疗大模型|
|中国科学院计算技术研究所|[百聆](https://github.com/ictnlp/BayLing)|基于 [LLaMA](https://mp.weixin.qq.com/s/dKInMi6P80GXecUtR3WQsA)，权重Diff下载[7B](https://huggingface.co/ICTNLP/bayling-7b-diff)和[13B](https://huggingface.co/ICTNLP/bayling-13b-diff),[demo](http://nlp.ict.ac.cn/bayling/demo/) |
|沪渝人工智能研究院|[兆言](https://mp.weixin.qq.com/s/RtcdWGrfIW5unyvxVplCSg)|也称：上海交通大学重庆人工智能研究院|
|企查查|知彼阿尔法|-|
|超对称技术公司| [乾元](https://bbt.ssymmetry.com/)|BBT-1-1B金融模型，BBT-2-12B-TF金融模型，BBT-2-12B-TC代码模型，BBT-2-12B-Image文生图模型，BBT-2-12B-Science科学论文模型，BBT-2.5-13B-Text中英双语基础模型|
|清睿智能|[ArynGPT](https://mp.weixin.qq.com/s/FFRfzwoXBM2dGs9O7F-Z5A) |英语智能对话口语老师|
|微盟|[WAI](https://wai.weimob.com/)|-|
|蜜度|[文修](https://mp.weixin.qq.com/s/aHSw9Kxib3Zj84qDGn3Dyg)|智能校对|
|中国电子云|[星智](https://mp.weixin.qq.com/s/qNoTD4BY2DX5ziSe1ZPSLw)|政务大模型|
|西北工业大学+华为 |[秦岭·翱翔](https://www.nwpu.edu.cn/info/1198/65828.htm) |流体力学大模型,湍流+流场 |
|奇点智源| [Singularity OpenAPI](https://openapi.singularity-ai.com/)|[瑶光和天枢](https://openapi.singularity-ai.com/index.html#/documentIndex)|
|联汇科技 |欧姆|[OmModel欧姆多模态（视觉语言）大模型](https://om.linker.cc/)|
|阅文集团|网文大模型|[国内首个网文行业大模型](https://app.gmdaily.cn/as/opened/n/ba6a7ddbbef54233b2fec2cb43e9d3c7)|
|北京交通大学|[TransGPT](https://github.com/DUOMO/TransGPT)|[国内首个综合交通领域的大模型](https://github.com/DUOMO/TransGPT)|

---



> # Please keep adding relevant information, we greatly appreciate your contributions.
