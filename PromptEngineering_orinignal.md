# 🌠 Prompt Engineering

# Table Of Contents

- [1. Introduction](#introduction)
- [2. Design Principle and Framework](#design-principle-and-framework)
- [3. Prompt Techniques](#prompt-techniques)

<img width="200%" src="./figures/hr.gif" />

## 1. Introduction

Prompt engineering involves designing, creating, and optimizing prompts for the purpose of extracting accurate, consistent, and fair outputs from large language models (LLMs). 

> The aforementioned is also applicable to other large generative models, such as text-to-image synthesizers. For the sake of brevity, we will temporarily focus on language models.


LLMs are trained on vast amounts of text data, allowing them to encode a substantial amount of factual information about the world. Their popularity has surged in recent years due to their ability to generate human-like text, making them ideal for chatbots, virtual assistants, and similar applications. However, it is essential to note that without appropriate prompt engineering, the generated outputs can be unpredictable and potentially result in harmful consequences.

The goal of prompt engineering is to identify an appropriate prompt to be given to LLMs, in such a way that they generate responses that can effectively solve our specified complex tasks. 

A prompt can take on any form of sentence such as statements, instructions, questions, or even paragraphs, as long as it inspires the imagination of LLMs and guides them to explore a variety of topics and tasks.

> For the sake of making it easier for beginners to understand, we will temporarily set aside the concept of soft prompts.

After receiving various types of prompts, LLMs have the ability to generate a diverse range of output formats, including completed sentences, question-answers, translations, conversational scripts, and other text generation, all of which have wide-ranging applications and great creative potential. 

Depending on the knowledge and experience acquired from vast amounts of language data during training, LLMs are not just used for chatbot conversations, but also highly effective problem solvers. 

### 💥 Highlight: To enhance the problem-solving ability of LLMs, high-quality prompts are crucial.

<img width="200%" src="./figures/hr.gif" />

## 2. Design Principle and Framework 
A good prompt is one that is specific and provides enough context for LLMs to be able to generate a response that is relevant to the task.

### 2.1 Design principle
By following design principles, you can improve the quality and accuracy of the LLM’s responses and enhance the overall user experience.

- **Be clear and specific**: The prompt should clearly state the task or question that the model is expected to answer. Avoid ambiguity or vagueness in the prompt as this can lead to unclear or irrelevant responses.
-	**Provide context**: The prompt should provide enough context for the model to understand the task and generate a relevant response. This can include relevant background information, examples, or constraints.
-	**Use natural language**: Write the prompt in a natural and conversational style that the model can understand and respond to. Avoid using complex or technical language that may confuse the model.
-	**Be concise**: Keep the prompt concise and to the point. Avoid unnecessary details or information that may distract the model from the task at hand.
-	**Avoid complex sentence structure**: Using complex sentence structures can confuse the model, leading to poorly generated output. Using simple sentences and straightforward language makes it easier for the model to understand and generate the desired output.
-	**Avoid ambiguity**: Ensure that the prompt is specific and avoids ambiguity. Avoid using words with multiple meanings or phrases that can be interpreted in different ways.
-	**Use keywords**: Use keywords in the prompt that are relevant to the topic of the conversation. This helps the chatbot to understand the context and respond appropriately.
-	**Consider the intended audience**: Consider the intended audience for the generated responses and tailor the prompts accordingly. Use appropriate language, terminology, and examples that the audience is likely to understand and relate to.
-	**Use appropriate formatting**: Use appropriate formatting such as bullet points, numbered lists, or bold text to highlight key information in the prompt. This can help the model understand the structure and organization of the prompt.
-	**Test and refine**: Test the prompts with the model and refine them based on the quality of the generated responses. Iteratively refine the prompts until the generated responses are of high quality and relevance.

### 2.2 Framework
We propose a framework for prompt design that consists of five key components: context, instructions, relevance, constraints, and demonstration. This standardized structure can help streamline prompt design and ensure that a consistent process is followed, resulting in more effective prompts.

- 🕐**Context**:  
  - Context is key when designing a prompt. Make sure to provide enough background information surrounding to the designated task so that the model can understand the situation and generate text that is relevant and accurate. 

- 🕜**Instruction**:
  - Instruction is crucial as it guides the model on what to do and what is expected of it. It is important to be clear, concise and specific. When dealing with complex reasoning tasks, consider breaking the tasks down into smaller, more manageable steps to help the model understand the task at hand.

- 🕑**Relevance**:
  - Relevance is essential when specific information needs to be referenced. This information could be links to relevant articles or data, or specific input provided by the user. By utilizing this specific information, the model can tailor its output to be personalized, reliable, and consistent with the user's needs.

- 🕝**Constraint**:    
  - Constraint is helpful in guiding LLMs on what they can and cannot do, ultimately leading to more accurate results. This may involve specifying the format of the output, the type of language to be used, or even the length of the output. Additionally, specifying the difficulty level and style can further refine the output.

- 🕒**Demonstration**: 
  - Demonstration is valuable as it allows LLMs to understand what is expected through examples, particularly when instructions alone cannot effectively convey specific details and accuracy. By offering examples of input and output pairs, LLMs can automatically identify patterns and then generate text that is aligned with the user's expectations.

## 💥 Based on the complexity and characteristics of the task, you can select a few components from them to form your prompt. 

Usually, 'instruction' or 'demonstration' can both be used to convey our intent behind tasks or questions. We can choose to use either of them depending on the situation of completing the task or question. 

At the beginning of the prompt, we can directly write the content to express the intent of the instruction, without having to explicitly use the words 'instruction' or 'demonstration'.  

👁️ **[Prompt example]**:

```Write a 500-word short story that incorporates the theme of discovering hidden talents. Ensure that your story has a clear beginning, middle, and end, and that the characters are well-rounded and believable.``` 

```[Context]: You are tasked with writing a short story about a character who suddenly discovers a hidden talent they never knew they possessed. The story should have a clear plot and well-developed characters.```

```[Relevance]: To help you develop your story, please review the following articles: "The Power of Uncovering Hidden Talents" and "The Importance of Character Development in Fiction Writing." These articles will provide you with relevant insights and ideas for your story.``` 

```[Constraint]: Your story must be written in the third person point of view and should be appropriate for a general audience. Additionally, ensure that the story has a positive and inspiring tone.```

```
Output: 

  Emily had always considered herself an average person. She went to work, came home, and spent her evenings watching TV or scrolling through social media. But on this particular day, something changed. 
  As she walked home from work, she noticed a group of people gathered around a street performer. 
  Curiosity piqued, she pushed her way through the crowd to see what was happening. The performer was a young man playing a guitar, his fingers moving expertly over the strings. 
  Emily found herself drawn in by the music, the melody taking her to a place she had never been before. As the song ended, the performer looked up and met Emily's gaze. 
  He smiled and gestured for her to come closer.Emily hesitated, feeling self-conscious, but something about the performer's smile made her feel welcome. 
  She moved closer, and the performer handed her his guitar."Play something," he said, encouragingly. Emily shook her head. "I don't know how," she replied. "Everyone has music inside them," the performer said. "Just let it out."Emily looked down at the guitar in her hands, feeling a sense of unease. 
  She had never played an instrument before, and the thought of making a fool of herself in front of this crowd was daunting. But as she looked up, she saw the performer nodding at her, encouraging her to give it a try. 
  Taking a deep breath, Emily placed her fingers on the strings and began to strum. To her surprise, a melody began to form. She felt the music flowing through her, the notes coming easily as if they had been waiting to be released all along. 
  The crowd around her cheered, and Emily felt a sense of pride swell inside her. She had discovered a talent she never knew she possessed. From that moment on, she spent every spare moment practicing, determined to hone her skills and see where this new passion could take her. 
  Months passed, and Emily found herself playing at local bars and coffee shops, her talent drawing in crowds of people eager to hear her music. 
  She had never felt so alive, and every time she played, she felt a sense of fulfillment and purpose that she had never experienced before. One day, a music producer heard her play and offered her a record deal. 
  Emily couldn't believe it - this was everything she had ever dreamed of. She signed the contract and began working on her first album. 
  As her music career took off, Emily looked back on that chance encounter with the street performer and realized that it had changed her life forever. 
  She had discovered a hidden talent she never knew she possessed, and it had brought her more happiness and fulfillment than she could ever have imagined.
```

I like this story:  Unleash Your Hidden Talent! 

👁️ **[Prompt example]**:

```Circulation revenue has increased by 5% in Finland. [Positive]``` 
```Panostaja did not disclose the purchase price. [Neutral]```
```Paying off the national debt will be extremely painful. [Negative]``` 
```The acquisition will have an immediate positive impact. [???]```

```
Output:  
Neutral
```

<img width="200%" src="./figures/hr.gif" />

## 3. Prompt Techniques

### 3.1 Basic prompting

Prompt-based approaches offer a powerful and flexible tool for resolving a wide range of NLP tasks.  We can complete the task by expressing ourselves in natural language, so there's no need to adhere to a specific format. 

#### Sentiment Analysis: LLMs can be trained to identify the sentiment expressed in a piece of text, such as positive, negative, or neutral. This can be useful for analyzing customer feedback, social media posts, and product reviews.

👁️ **[Prompt example]**: 

```Analyze the sentiment of the following text:```

```Text:  'I absolutely loved the movie! The acting was fantastic and the plot kept me engaged throughout the entire film.'```

**Entity Recognition**: LLMs can identify entities in a text, such as people, places, organizations, and products. This can be used for named entity recognition in various domains, such as news articles or legal documents.

👁️ **[Prompt example]**:

```Analyze the following paragraph and identify all the people, places, and organizations mentioned in the text, and then output the results in json format. ```

```Text: 'The Apple event took place at the Steve Jobs Theater in Cupertino, California. Tim Cook, the CEO of Apple, introduced the new iPhone 13, which will be available for pre-order starting next week. The phone comes in several colors and features a faster processor and longer battery life.'```

**Relation Extraction**: LLMs can also extract relationships between entities in a piece of text, such as identifying that a person is the CEO of a company or that a product is made by a certain brand. This can be useful for tasks such as knowledge graph construction, where the relationships between entities are important for understanding the domain.

👁️ **[Prompt example]**:

```Analyze the following sentence and extract the relationship between two entities, and then output the results in JSON format.```  

```Text: 'Elon Musk founded SpaceX in 2002 with the goal of reducing space transportation costs and enabling the colonization of Mars.'``` 

**Text Summarization**: LLMs can also be used for text summarization, where they can automatically generate a summary of a longer piece of text, such as an article or report. This can be useful for quickly understanding the key points of a document without having to read the entire thing.

👁️ **[Prompt example]**: 

```Summarize the following paragraph:  {Paste your paragraph}```

**Text Classification**: LLMs can classify text into predefined categories, such as classifying news articles into different topics or categorizing customer inquiries into different types. This can be useful for tasks such as content moderation, where incoming text needs to be classified quickly and accurately.

👁️ **[Prompt example]**: 

```Classify the following keyword list in groups based on their search intent, whether commercial, transactional or informational: {Paste your keywords}```

**Text Clustering**: LLMs can group similar texts together based on their content or features. This feature can be useful in tasks such as data mining, topic modeling, and customer segmentation.

👁️ **[Prompt example]**:  

```Cluster the following set of news articles into distinct groups based on their content:``` 

```"Tesla's electric car sales continue to soar despite the pandemic"``` 

```"New study suggests coffee consumption may lower risk of heart disease"``` 

```"The latest iPhone model features a larger screen and improved camera"```

```"COVID-19 cases surge in India, overwhelming healthcare system" ```

```"Amazon announces plans to build a new fulfillment center in Texas"```

```"Scientists discover new species of bird in the Amazon rainforest"```

```"Global climate change conference to be held in Paris next month"``` 

```"Starbucks introduces plant-based milk options in all U.S. stores"```

**Machine Translation**: LLMs can be used for machine translation, where they can translate text from one language to another. This can be useful for businesses that operate globally, as well as for individuals who need to communicate with people who speak different languages.

👁️ **[Prompt example]**

```Translate the following paragraph into Chinese. {Paste your paragraph}```


**Question Answering**: LLMs can be used for question answering, where they can read a passage of text and answer questions about it. This can be useful for applications such as customer support, where customers can ask questions and receive quick, accurate answers.

👁️ **[Prompt example]**:  

```The Great Barrier Reef is the world's largest coral reef system, composed of over 2,900 individual reefs and 900 islands stretching for over 2,300 kilometers. It is located in the Coral Sea, off the coast of Australia. The reef is home to a diverse range of marine life, including over 1,500 species of fish, 600 types of coral, and numerous other species. What is the Great Barrier Reef and where is it located?```
