# 🌠 Prompt Engineering

## Introduction

Prompt engineering involves designing, creating, and optimizing prompts for the purpose of extracting accurate, consistent, and fair outputs from large language models (LLMs). 

> The aforementioned is also applicable to other large generative models, such text-to-image synthesizers. For the sake of brevity, we will temporarily focus on language models.


LLMs are trained on vast amounts of text data, allowing them to encode a substantial amount of factual information about the world. Their popularity has surged in recent years due to their ability to generate human-like text, making them ideal for chatbots, virtual assistants, and similar applications. However, it is essential to note that without appropriate prompt engineering, the generated outputs can be unpredictable and potentially result in harmful consequences.

The goal of prompt engineering is to identify an appropriate prompt to be given to LLMs, in such a way that they generate responses that can effectively solve our specified complex tasks. 

A prompt can take on any form of sentence such as statements, instructions, questions, or even paragraph, as long as it inspires the imagination of LLMs and guides them to explore a variety of topics and tasks.

> For the sake of making it easier for beginners to understand, we will temporarily set aside the concept of soft prompts.**

After receiving various types of prompts, LLMs have the ability to generate a diverse range of output formats, including completed sentences, question-answers, translations, conversational scripts, and other text generation, all of which have wide-ranging applications and great creative potential. 

Depending on the knowledge and experience acquired from vast amounts of language data during training, LLMs are not just used for chatbot conversations, but also highly effective problem solvers. 

### 💥 Hightlight: To enhance the problem-solving ability of LLMs, high-quality prompts are crucial.

## Design Principle and Framework 
A good prompt is one that is specific and provides enough context for LLMs to be able to generate a response that is relevant to the task.

### Design principle
By following design principle, you can improve the quality and accuracy of the LLM’s responses and enhance the overall user experience.

- Be clear and specific: The prompt should clearly state the task or question that the model is expected to answer. Avoid ambiguity or vagueness in the prompt as this can lead to unclear or irrelevant responses.
-	Provide context: The prompt should provide enough context for the model to understand the task and generate a relevant response. This can include relevant background information, examples, or constraints.
-	Use natural language: Write the prompt in a natural and conversational style that the model can understand and respond to. Avoid using complex or technical language that may confuse the model.
-	Be concise: Keep the prompt concise and to the point. Avoid unnecessary details or information that may distract the model from the task at hand.
-	Avoid complex sentence structure: Using complex sentence structures can confuse the model, leading to poorly generated output. Using simple sentences and straightforward language makes it easier for the model to understand and generate the desired output.
-	Avoid ambiguity: Ensure that the prompt is specific and avoids ambiguity. Avoid using words with multiple meanings or phrases that can be interpreted in different ways.
-	Use keywords: Use keywords in the prompt that are relevant to the topic of the conversation. This helps the chatbot to understand the context and respond appropriately.
-	Consider the intended audience: Consider the intended audience for the generated responses and tailor the prompts accordingly. Use appropriate language, terminology, and examples that the audience is likely to understand and relate to.
-	Use appropriate formatting: Use appropriate formatting such as bullet points, numbered lists, or bold text to highlight key information in the prompt. This can help the model understand the structure and organization of the prompt.
-	Test and refine: Test the prompts with the model and refine them based on the quality of the generated responses. Iteratively refine the prompts until the generated responses are of high quality and relevance.

### Framework
We propose a framework for prompt design that consists of five key components: context, instructions, relevance, constraints, and demonstration. This standardized structure can help streamline prompt design and ensure that a consistent process is followed, resulting in more effective prompts.

- **Context**:  
  - Context is key when designing a prompt. Make sure to provide enough background information surrounding to the designated task so that the model can understands the situation and generate text that is relevant and accurate. 

- **Instruction**:
  - Instruction is crucial as it guides the model on what to do and what is expected of it. It is important to be clear, concise and specific. When dealing with complex reasoning tasks, consider breaking the tasks down into smaller, more manageable steps to help the model understand the task at hand.

- **Relevance**:
  - Relevance is essential when specific information needs to be referenced. This information could be links to relevant articles or data, or specific input provided by the user. By utilizing this specific information, the model can tailor its output to be personalized, reliable, and consistent with the user's needs.

- **Constraint**:    
  - Constraint is helpful as guiding LLMs on what it can and cannot do, ultimately leading to more accurate results. This may involve specifying the format of the output, the type of language to be used, or even the length of the output. Additionally, specifying the difficulty level and style can further refine the output.

- **Demonstration**: 
  - Demonstration is valuable as it allow LLMs to understand what is expected through examples, particularly when instructions alone cannot effectively convey specific details and accuracy. By offering examples of input and output pairs, LLMs can automatically identify patterns and then generate text that is aligned with the user's expectations.

## 💥 Based on the complexity and characteristics of the task, you can select a few components from them to form your prompt.*






