# 🌠 Prompt Engineering  👉[中文页面](./promptengineering_zh.md)👈

# Table Of Contents

- [1. Introduction](#introduction)
- [2. Design Principle and Framework](#design-principle-and-framework)
- [3. Prompt Techniques](#prompt-techniques) 


<img width="200%" src="./figures/hr.gif" />

## 1. Introduction

Prompt engineering is a powerful tool that significantly enhances our interaction with generative large language models, boosting productivity. Human-machine collaboration is rapidly becoming the primary mode of production, an undeniable trend. Prompt engineering focuses on designing, creating, and refining prompts to elicit accurate, consistent, and unbiased outputs from large language models (LLMs).

> This concept also applies to other large generative models, such as text-to-image synthesizers. For conciseness, this discussion will primarily focus on language models.

LLMs are trained on extensive text datasets, enabling them to capture a vast amount of real-world information. Their ability to generate human-like text has led to their widespread adoption in applications like chatbots and virtual assistants. However, without proper prompt engineering, their outputs can be unpredictable and potentially problematic.

The core objective of prompt engineering is to craft effective prompts that guide LLMs to generate responses capable of solving complex, specific tasks.

A prompt can be any form of natural language—statements, instructions, questions, or even paragraphs—that stimulates the LLM's creativity and directs it toward exploring various topics and tasks.

> To simplify understanding for beginners, we will temporarily set aside the concept of soft prompts.

Upon receiving diverse prompts, LLMs can produce a wide array of output formats, including complete sentences, Q&A pairs, translations, conversational scripts, and other text generations, all possessing broad applications and immense creative potential.

Leveraging the knowledge and experience gained from vast language data during training, LLMs serve not only as conversational chatbots but also as highly effective problem-solvers.

### 💥 Highlight: High-quality prompts are essential for enhancing the problem-solving capabilities of LLMs.

<img width="200%" src="./figures/hr.gif" />

## 2. Design Principle and Framework 
A good prompt is one that is specific and provides enough context for LLMs to be able to generate a response that is relevant to the task.

### 2.1 Design principle
To ensure prompt effectiveness and accuracy, adhere to these principles:

- **1. Clear and specific instructions:** Clearly state the task or question. Avoid ambiguity or vagueness, which can lead to unclear or irrelevant answers.
- **2. Simple and clear wording:** Use straightforward, explicit language. Avoid overly complex or vague terms to enhance model comprehension.
- **3. Avoid complex sentence structures:** Minimize complex sentence types and grammatical structures to simplify model understanding.
- **4. Eliminate ambiguity:** Ensure prompts precisely convey your intent. Avoid ambiguous words to guarantee correct model interpretation and response.
- **5. Utilize keywords:** Incorporate relevant keywords to the conversation topic. This aids the LLM in understanding context and responding appropriately.
- **6. Consider the intended audience:** Tailor prompts to the target audience of the generated responses. Use appropriate language, terminology, and examples for better understanding.
- **7. Test and refine:** Experiment with prompts and iteratively refine them based on response quality. Continue until generated responses achieve high quality and relevance.

Adhering to these design principles will enhance the quality and accuracy of large language model outputs, thereby improving the user experience.
### 2.2 Framework
We propose a prompt design framework comprising five key components: Context, Instruction, Relevance, Constraints, and Demonstration. Adhering to the standardized structure of these components simplifies prompt design, leading to more effective and targeted prompts.

- 🕐**Context**:  
  - Context is paramount in prompt design. Provide sufficient background information relevant to the task, enabling the model to understand the situation and generate accurate, pertinent text.

- 🕜**Instruction**:  
  - Instructions are vital for guiding the model on expected actions. Be clear, concise, and specific. For complex reasoning tasks, consider breaking them into smaller, manageable steps to aid model comprehension.

- 🕑**Relevance**:  
  - Relevance is crucial when specific information needs referencing. This can include links to articles, data, or user-provided input. Utilizing such information allows the model to personalize its output, ensuring reliability and consistency with user needs.

- 🕝**Constraint**:    
  - Constraints help define what LLMs can and cannot do, ultimately yielding more accurate results. This may involve specifying output format, language style, or length. Additionally, defining difficulty levels and stylistic preferences can further refine the output.

- 🕒**Demonstration**: 
  - Demonstrations are invaluable for helping LLMs understand expectations through examples, especially when instructions alone cannot fully convey specific details or accuracy. By providing input-output pairs, LLMs can automatically identify patterns and generate text aligned with user expectations.

## 💥 Based on the complexity and characteristics of the task, you can select a few components from them to form your prompt. 

### 2.3 Application of the framework and principles

Subsequently, we started with a basic prompt that only contains the context and instructions, gradually enriching the structural framework of our prompts. In this way, we visualize the role played by the five key components of the prompt framework and the output of the large language model in different situations.


#### 2.3.1 Basic prompting：

To begin with, we use a prompt only containing  the context  and instructions as the base example. Define the model's role as a history teacher (Context) and ask to write a multiple-choice question for a history course (instructions).


👁️ **[Prompt example]**:  

    Context: Suppose you are a history teacher with more than 30 years of teaching experience.  
    Instructions: Write a multiple-choice question for a history course.

**Output:**   

    Question:
    
    During which period did the Industrial Revolution take place?

    A) Ancient Greece
    B) Renaissance
    C) Victorian Era
    D) Enlightenment

    Answer:C) Victorian Era
    Explanation:

    The Industrial Revolution refers to a significant shift in manufacturing and economic
    practices that occurred primarily in the late 18th and early 19th centuries. 
    It was a period of rapid industrialization and technological advancements, leading to the
    mechanization of production processes and the emergence of factories. This period 
    witnessed the development of steam power, the expansion of railways, and the mass
    production of goods. The Victorian Era, named after Queen Victoria of England, spanned 
    from 1837 to 1901, and it coincided with the height of the Industrial Revolution. 
    It was during this time that the impacts of industrialization were most prominent, 
    transforming societies and economies across Europe and the United States.

Based on the content of such basic prompts, the large language model outputs the corresponding results. However, with such "free" prompting instructions, the form, format, and content of the questions in the results generated by the large language model are unstable .

#### 2.3.2 Addition of Relevance：

Based on the basic prompt, we added the relevance message "the question should be related to the Renaissance" to specify the relevant knowledge points for the output generated by the model.  

👁️ **[Prompt example]**:  

    Context: Suppose you are a history teacher with more than 30 years of teaching experience.  
    Instructions: Write a multiple-choice question for a history course.  
    Relevance: The question should be related to the Renaissance

**Output:**   

    Question:  
    Which influential artist is often regarded as the epitome of the Renaissance?  
    A) Leonardo da Vinci  B) Michelangelo  C) Vincent van Gogh  D) Pablo Picasso  
    Answer: A) Leonardo da Vinci  
    Explanation:  
    Leonardo da Vinci is widely regarded as the epitome of the Renaissance, a period in European history characterized by a renewed interest in classical art, literature, and learning. Da Vinci, born in 1452 in Italy, was a polymath who excelled in various fields such as painting, sculpture, anatomy, engineering, and architecture. His masterpieces, such as the Mona Lisa and The Last Supper, exemplify the artistic achievements of the Renaissance. Da Vinci's attention to detail, scientific approach, and mastery of techniques set new standards for artists of his time and subsequent generations. His work not only demonstrated exceptional artistic skill but also reflected the spirit of humanism and curiosity that defined the Renaissance period.

In this case, the stability of the content involved in the output results of the model is guaranteed.
#### 2.3.3 Clarify constraints：
Adding a constraint to the prompt makes it clear what rules or restrictions the model should follow. In our next example, we add the constraint "There should be more than two correct answers among the four options".  
👁️ **[Prompt example]**:  

    Context: Suppose you are a history teacher with more than 30 years of teaching experience.  
    Instructions: Write a multiple-choice question for a history course.  
    Relevance: The question should be related to the Renaissance.  
    Constraint: There should be more than two correct answers among the four options.

**Output:**  

    Question:  
    Which artistic techniques were commonly employed by Renaissance painters? (Select all that apply.)  
    A) Linear perspective   B) Chiaroscuro   C) Pointillism   D) Sfumato  
    Answer:A) Linear perspective  B) Chiaroscuro  D) Sfumato  
    Explanation:  
    During the Renaissance, artists employed various techniques to achieve realistic and visually captivating artworks. Three of the options provided were commonly used during this period.  
    A) Linear perspective: Renaissance painters embraced the use of linear perspective to create depth and dimension in their compositions. By employing this technique, artists could accurately depict the illusion of distance and create the impression of three-dimensional space on a two-dimensional surface.  
    B) Chiaroscuro: Chiaroscuro, meaning "light-dark" in Italian, is a technique that involves the strong contrast between light and shadow. Renaissance painters used this technique to model forms, create a sense of volume, and evoke a dramatic effect in their paintings.  
    D) Sfumato: Sfumato is a technique characterized by the subtle blending of colors and tones to create soft, hazy transitions. It is particularly associated with the works of Leonardo da Vinci. Sfumato was employed to give a sense of atmospheric perspective and to achieve a smooth and realistic appearance, especially in portrayals of human faces.  
    C) Pointillism: Pointillism, a technique developed in the late 19th century, is not directly associated with the Renaissance. It involves the use of small, distinct dots of pure color that, when viewed from a distance, blend together to create a cohesive image. This technique was utilized by post-Impressionist painters such as Georges Seurat and Paul Signac.
    Thus, options A, B, and D are the correct answers as they represent the artistic techniques commonly employed by Renaissance painters.

On the premise of stabilizing the output content ( the addition of Relevance ), the format of the questions is further specified as multiple choice questions, and the final output format is limited.

#### 2.3.4 List of Demonstration：

Based on the framework of the above four key components, we can further include demonstration for reference to clarify for the model the specific details of the output results and the output format that cannot be easily described in natural language.

👁️ **[Prompt example]**:  

    Context: Suppose you are a history teacher with more than 30 years of teaching experience.  
    Instructions: Write a multiple-choice question for a history course.  
    Relevance: The question should be related to the Renaissance.  
    Constraint: There should be more than two correct answers among the four options.  
    Demonstration:  
    Question: During the Renaissance, which of the following cities was a cultural center?  
     (A) London (B) Paris (C) Florence (D) Amsterdam   
    The correct answer is: A and C.  
     Answer Explanation：During the Renaissance, Florence was one of the most important cultural centers in Europe, where many important artists, scholars and thinkers worked and lived, including Leonardo da Vinci, Michelangelo and Dante. London also rose rapidly during the Renaissance to become a cultural and commercial center of Europe, attracting many cultural celebrities and merchants. Therefore, options A and C are the correct answers.  
**Output:**  

    Question:  
    During the Renaissance, which of the following cities were renowned cultural centers? (Select all that apply.)  
    A) Rome  B) Paris  C) Florence  D) Venice  
    The correct answer is: A, C, and D.  
    Answer Explanation:  
    During the Renaissance, several cities emerged as vibrant cultural centers, fostering artistic, intellectual, and scholarly advancements. The options provided represent significant cities during this period.  
    A) Rome: Rome, with its rich history as the center of the Roman Empire and the Catholic Church, continued to be a hub of artistic and intellectual activity during the Renaissance. It attracted artists, architects, and scholars who were inspired by the classical ruins and the patronage of the Church.  
    C) Florence: Florence, located in Italy, was one of the most important cultural centers during the Renaissance. It was renowned for its patronage of the arts by wealthy families such as the Medici. Many influential artists, scholars, and thinkers, including Leonardo da Vinci, Michelangelo, and Dante, lived and worked in Florence.  
    D) Venice: Venice, known for its unique location as a major port and hub of trade in the Mediterranean, played a significant role in the Renaissance. The city's prosperity and cosmopolitan atmosphere attracted artists, merchants, and intellectuals from diverse backgrounds, fostering a vibrant cultural scene.  
    B) Paris: While Paris would go on to become a cultural center in subsequent centuries, it did not reach its Renaissance cultural prominence until a later period. The Renaissance primarily thrived in Italy, and Paris rose to prominence as a cultural hub during later periods, such as the Enlightenment.  
    Therefore, options A, C, and D are the correct answers as they represent cities that were renowned cultural centers during the Renaissance.

As we can see, the large language model will follow the format of the given demonstration strictly and output the final result we need.

> Sometimes, we can make the large language model understand the task instructions we want to give simply by enumerating multiple examples (or even a single example).


👁️ **[Prompt example]**:  

    Gu Ailing won the first crown of the New Year of the Rabbit. Scoring break advantage.  
    ---- sports   
    Data released by the National Health Insurance Bureau showed that from January to March 2023, the total income of the basic medical insurance fund (including maternity insurance) was 910.48 billion yuan, an increase of 9.5% year-on-year.  
    ---- medical   
    Berkshire Hathaway reduced its stake in BYD shares from 10.05% to 9.87%. The HKEx Disclosure Ease requires disclosure when a major shareholder increases or decreases its shareholding only if it crosses a certain round number percentage.  
    ---- Finance  
    Edge computing products have served customers in industries such as online education, video, gaming, and connected cars.
    ----  
**Output:**   

    Technology

## 3. Prompt Techniques
#### Basic prompting


Prompt-based approaches offer a powerful and flexible tool for resolving a wide range of NLP tasks.  We can complete the task by expressing ourselves in natural language, so there's no need to adhere to a specific format. 

**Sentiment Analysis**: LLMs can be trained to identify the sentiment expressed in a piece of text, such as positive, negative, or neutral. This can be useful for analyzing customer feedback, social media posts, and product reviews.

👁️ **[Prompt example]**: 

    Analyze the sentiment of the following text:

    Text:  'I absolutely loved the movie! The acting was fantastic and the plot kept me engaged throughout the entire film.'

**Output:**   

    Sentiment: Positive

    The sentiment of the provided text is clearly positive. The use of words like "absolutely loved," "fantastic," and "engaged" indicates a strong positive sentiment towards the movie. The person expressing their opinion seems to have thoroughly enjoyed the film, praising both the acting and the plot. Overall, the sentiment conveyed in the text is highly positive.  
**Entity Recognition**: LLMs can identify entities in a text, such as people, places, organizations, and products. This can be used for named entity recognition in various domains, such as news articles or legal documents.

👁️ **[Prompt example]**:
    
    Analyze the following paragraph and identify all the people, places, and organizations mentioned in the text, and then output the results in json format. ```

    Text: 'The Apple event took place at the Steve Jobs Theater in Cupertino, California. Tim Cook, the CEO of Apple, introduced the new iPhone 13, which will be available for pre-order starting next week. The phone comes in several colors and features a faster processor and longer battery life.'

**Output:**   

    {"people": ["Tim Cook"],"places": ["Steve Jobs Theater","Cupertino, California"],"organizations": ["Apple"]}

**Relation Extraction**: LLMs can also extract relationships between entities in a piece of text, such as identifying that a person is the CEO of a company or that a product is made by a certain brand. This can be useful for tasks such as knowledge graph construction, where the relationships between entities are important for understanding the domain.

👁️ **[Prompt example]**:


    Analyze the following sentence and extract the relationship between two entities, and then output the results in JSON format.```  

    Text: 'Elon Musk founded SpaceX in 2002 with the goal of reducing space transportation costs and enabling the colonization of Mars.'``` 

**Output:** 

    {
      "entity1": "Elon Musk",
      "entity2": "SpaceX",
      "relationship": "founded"
    }

**Text Summarization**: LLMs can also be used for text summarization, where they can automatically generate a summary of a longer piece of text, such as an article or report. This can be useful for quickly understanding the key points of a document without having to read the entire thing.

👁️ **[Prompt example]**:   

    Summarize the following paragraph:  
    Do we know where the kite in our hearts really is? We will not get it again if we miss it in life, maybe we will repent and redeem ourselves, but all these seem to be too late. Whenever the kite is released in the sky, shouldn't we ask ourselves whether we really treasure what we have.
    Each of us has done something in our youth that we will be ashamed of in the future. These things may be like a shadow that accompanies you for the rest of your life, so that you can only look down at it. But time will not turn around, their best efforts to make up for it, how is not a kind of self-help? The beauty and friendship of childhood, because of cowardly negligence and ruined, if you are given another chance, you are willing to go out of your way to regain that former self?
    But people are like that, always living within a certain time limit, where the world may be a few years later even they can not understand, but this is what we can not break through. For you, a thousand times, all over the body will still be righteous, maybe this is life, life is not just doing things worthwhile!

**Output:**   

    The paragraph reflects on the importance of appreciating and cherishing the valuable things in life. It highlights the idea that once an opportunity or something meaningful is missed, it may be difficult to regain it. The author suggests that individuals often carry regrets and shame from past actions, which can overshadow their lives. They express the notion that time cannot be reversed, but making efforts to make up for past mistakes is a form of self-help. The paragraph also mentions the loss of childhood innocence and friendships due to neglect, and poses the question of whether one would go to great lengths to regain their former self if given the chance. It concludes by acknowledging the limitations of human existence within the constraints of time, emphasizing the importance of righteousness and suggesting that life is not solely about accomplishing worthwhile tasks.  

**Text Clustering**: LLMs can group similar texts together based on their content or features. This feature can be useful in tasks such as data mining, topic modeling, and customer segmentation.

👁️ **[Prompt example]**:  

    Cluster the following set of news articles into distinct groups based on their content:``` 

    "Tesla's electric car sales continue to soar despite the pandemic"``` 

    "New study suggests coffee consumption may lower risk of heart disease"``` 

    "The latest iPhone model features a larger screen and improved camera"```

    "COVID-19 cases surge in India, overwhelming healthcare system" ```

    "Amazon announces plans to build a new fulfillment center in Texas"```

    "Scientists discover new species of bird in the Amazon rainforest"```

    "Global climate change conference to be held in Paris next month"``` 

    "Starbucks introduces plant-based milk options in all U.S. stores"```

**Output:**
       
    Based on their content, the news articles can be clustered into the following groups:

    1. Electric Vehicles and Technology:  
    "Tesla's electric car sales continue to soar despite the pandemic"  
    "The latest iPhone model features a larger screen and improved camera"  

    2. Health and Well-being:  
    "New study suggests coffee consumption may lower risk of heart disease"  
    "Starbucks introduces plant-based milk options in all U.S. stores"

    3. COVID-19 and Healthcare:  
    "COVID-19 cases surge in India, overwhelming healthcare system"  

    4. Environment and Wildlife:  
    "Scientists discover new species of bird in the Amazon rainforest"  
    "Global climate change conference to be held in Paris next month"

    5. Business and Economy:  
    "Amazon announces plans to build a new fulfillment center in Texas"  

    These clusters group the articles based on their shared themes, such as electric vehicles/technology, health and well-being, COVID-19/healthcare, environment/wildlife, and business/economy.

**Machine Translation**: LLMs can be used for machine translation, where they can translate text from one language to another. This can be useful for businesses that operate globally, as well as for individuals who need to communicate with people who speak different languages.

👁️ **[Prompt example]**

    Translate the following paragraph into Chinese.   
    Tales from Shakespeare is an English children's book written by Charles Lamb and his sister Mary Lamb in 1807. The book is designed to make the stories of Shakespeare's plays familiar to the young. However, as noted in the author's Preface, "[Shakespeare's] words are used whenever it seemed possible to bring them in; and in whatever has been added to give them the regular。  
**Output:**   

    《莎士比亚故事集》是一本英文儿童读物，由查尔斯·兰姆和他的姐姐玛丽·兰姆于1807年写成。这本书旨在使莎士比亚的剧作故事对年轻人更加熟悉。然而，正如作者的前言中所指出的那样，"莎士比亚的话语在任何可能引入的地方都被使用了；而且在添加的任何内容中都会使它们变得更加规范。  


**Question Answering**: LLMs can be used for question answering, where they can read a passage of text and answer questions about it. This can be useful for applications such as customer support, where customers can ask questions and receive quick, accurate answers.

👁️ **[Prompt example]**:  

    The Great Barrier Reef is the world's largest coral reef system, composed of over 2,900 individual reefs and 900 islands stretching for over 2,300 kilometers. It is located in the Coral Sea, off the coast of Australia. The reef is home to a diverse range of marine life, including over 1,500 species of fish, 600 types of coral, and numerous other species. 
    Question:What is the Great Barrier Reef and where is it located?

**Output:**   

    The Great Barrier Reef is indeed the world's largest coral reef system. It is composed of over 2,900 individual reefs and 900 islands, extending for more than 2,300 kilometers (1,400 miles). The reef is situated in the Coral Sea, off the northeastern coast of Australia. It stretches parallel to the coast of Queensland, running from the northern tip of Cape York Peninsula in the north to Bundaberg in the south. The Great Barrier Reef is a UNESCO World Heritage site and is widely regarded as one of the world's most remarkable natural wonders due to its immense size and ecological significance.

> In order to take full advantage of LLM's powerful generation capabilities, we can look at more aspects or domains of generation tasks in addition to natural language tasks.


### 3.2 Generate the specified programming language
The large language model can write Python (or other programming language) code for the corresponding task based on natural language descriptions. In this kind of task, the code generated by the large language model can sometimes be wrong, but we can feed the wrong code directly to the large language model, and it will humbly admit the error to debug and correct the code.  
In the following example, we require the model to implement the aggregation of the contents of a large number of EXCEL tables according to our prompt, to aggregate all EXCEL transcripts into a total transcript table, and to reorder them according to the total score.  

👁️ **[Prompt example]**:  

    Suppose you are a programmer who is skilled in writing programs in Python language.  
    I need to summarize all the EXCEL table data in the given folder, into a given EXCEL table, write Python requirements as follows:  
    1. In the sub-table, the columns are candidate number, candidate name, training mode, major number, major name, major ID, major course name, English score, political score, math score, major course score, total score and remarks. But there is no marking in the first line .  
    2. The format of the total table should be the same as the sub-table, and the data in the sub-table should be ranked from highest to lowest according to the total score.   
    3. Make a progress bar to indicate the amount of data that has been copied.  
**Output:**
   
    import pandas as pd
    from tqdm import tqdm
    import os
    def summarize\_excel\_tables(input\_folder, output\_file):

    # Initialize an empty DataFrame for storing the summarized data
    summarized_data = pd.DataFrame()

    # Get a list of all Excel files in the input folder
    excel_files = [file for file in os.listdir(input_folder) if file.endswith('.xlsx')]

    # Iterate over each Excel file in the folder
    for file in tqdm(excel_files, desc='Processing files', unit='file'):
        # Read the Excel file into a DataFrame
        file_path = os.path.join(input_folder, file)
        df = pd.read_excel(file_path)

        # Perform any necessary data processing or filtering on the DataFrame
        # ...

        # Append the processed DataFrame to the summarized data
        summarized_data = summarized_data.append(df, ignore_index=True)

    # Sort the summarized data by the 'total score' column in descending order
    summarized_data = summarized_data.sort_values(by='total score', ascending=False)

    # Write the summarized data to the output Excel file
    summarized_data.to_excel(output_file, index=False)

    # Example usage
    input_folder = '/path/to/input/folder'
    output_file = '/path/to/output/file.xlsx'
    summarize_excel_tables(input_folder, output_file)

### 3.3 Office software macro command generation

The  complex work in the daily office software, we can also use the exact prompts, so that the model for us to achieve the specified operation content.  
In the example, we asked the large language model to write an EXCEL macro command to the table in English scores between 50-70 in red, and in the same line of the comments field to write "to be processed.  
👁️ **[Prompt example]**:   
  
    Suppose you are a data clerk skilled in the use of EXCEL macro command writing.
    Write a macro command VBA for my EXCEL table.
    Red mark and bold all data in columns H between 50 and 70. Also in these rows, write "pending" in column M.

**Output:** 

    Sub HighlightPendingData()
         Dim lastRow As Long
         Dim ws As Worksheet
         Dim cell As Range
    
    ' Set the worksheet to operate on
    Set ws = ThisWorkbook.Sheets("Sheet1") ' Replace "Sheet1" with your actual sheet name
    
    ' Find the last row in column H
    lastRow = ws.Cells(ws.Rows.Count, "H").End(xlUp).Row
    
    ' Loop through the rows and check the data in column H
    For Each cell In ws.Range("H50:H" & lastRow)
        ' Check if the value is between 50 and 70
        If cell.Value >= 50 And cell.Value <= 70 Then
            ' Apply formatting: red font and bold
            cell.Font.Color = RGB(255, 0, 0)
            cell.Font.Bold = True
            
            ' Write "pending" in column M for the corresponding row
            ws.Range("M" & cell.Row).Value = "pending"
        End If
    Next cell
    End Sub
### 3.4 Generation of SQL commands
In database management, we can also use the exact prompt and ask the large language model to write the SQL commands for us for the corresponding functions.  
**Create  tables**

👁️ **[Prompt example]**: 

    Assuming that you are a database administrator skilled in MySQL language, write MySQL language according to my requirements.  
    Create two basic tables :  
    Table 1: The name is Student_Information, the table header contains Student_number (8 bits), name, gender, age, Major, Contact_information. Student_number and age are int type, the rest are char type. student_number is the main key.   
    Table 2: The name is Exam_Results, the table header contains Student_number, English, Mathematics, Linear_Algebra, Software_Engineering, Deep_Learning, prompt_Engineering, and Total_Results. Student_number is the main key, and the grades of all subjects except Total_Results are recorded according to the percentage system.

**Output:**
 
     -- Table 1: Student_Information
    CREATE TABLE Student_Information (
    Student_number INT(8) PRIMARY KEY,
    name CHAR(50),
    gender CHAR(10),
    age INT,
    Major CHAR(50),
    Contact_information CHAR(100)
    );

    -- Table 2: Exam_Results
    CREATE TABLE Exam_Results (
    Student_number INT(8) PRIMARY KEY,
    English FLOAT,
    Mathematics FLOAT,
    Linear_Algebra FLOAT,
    Software_Engineering FLOAT,
    Deep_Learning FLOAT,
    prompt_Engineering FLOAT,
    Total_Results FLOAT,
    FOREIGN KEY (Student_number) REFERENCES Student_Information(Student_number)
    );


**Generate simulation data**


 
👁️ **[Prompt example]**: 

    Generate 20 simulated data for Student_Information

**Output:** 


    INSERT INTO Student_Information (Student_number, name, gender, age, Major, Contact_information) VALUES
    (1001, 'John Doe', 'Male', 20, 'Computer Science', 'john.doe@example.com'),
    (1002, 'Jane Smith', 'Female', 19, 'Engineering', 'jane.smith@example.com'),
    (1003, 'Michael Johnson', 'Male', 21, 'Physics', 'michael.johnson@example.com'),
    (1004, 'Emily Williams', 'Female', 20, 'Biology', 'emily.williams@example.com'),
    (1005, 'David Brown', 'Male', 22, 'Chemistry', 'david.brown@example.com'),
    (1006, 'Olivia Davis', 'Female', 19, 'Mathematics', 'olivia.davis@example.com'),
    (1007, 'Daniel Miller', 'Male', 21, 'Computer Engineering', 'daniel.miller@example.com'),
    (1008, 'Sophia Wilson', 'Female', 20, 'Business Administration',   'sophia.wilson@example.com'),
    (1009, 'Matthew Taylor', 'Male', 19, 'Economics', 'matthew.taylor@example.com'),
    (1010, 'Ava Anderson', 'Female', 22, 'English Literature', 'ava.anderson@example.com'),
    (1011, 'Joseph Martinez', 'Male', 20, 'Political Science', 'joseph.martinez@example.com'),
    (1012, 'Mia Thompson', 'Female', 19, 'Sociology', 'mia.thompson@example.com'),
    (1013, 'William Clark', 'Male', 21, 'History', 'william.clark@example.com'),
    (1014, 'Abigail Rodriguez', 'Female', 20, 'Psychology', 'abigail.rodriguez@example.com'),
    (1015, 'James Lewis', 'Male', 22, 'Art', 'james.lewis@example.com'),
    (1016, 'Charlotte Lee', 'Female', 19, 'Music', 'charlotte.lee@example.com'),
    (1017, 'Benjamin Walker', 'Male', 21, 'Film Studies', 'benjamin.walker@example.com'),
    (1018, 'Evelyn Hall', 'Female', 20, 'Communication', 'evelyn.hall@example.com'),
    (1019, 'Alexander Young', 'Male', 19, 'Journalism', 'alexander.young@example.com'),
    (1020, 'Harper Hernandez', 'Female', 22, 'Graphic Design', 'harper.hernandez@example.com');



👁️ **[Prompt example]**: 

    Generate 20 simulated data for Exam_Results based on the simulated data generated in Student_Information


**Output:** 

    INSERT INTO Exam_Results (Student_number, English, Mathematics, Linear_Algebra, Software_Engineering, Deep_Learning, prompt_Engineering, Total_Results) VALUES
    (1001, 85.5, 90.2, 92.3, 88.7, 89.1, 91.5, 527.3),
	(1002, 78.9, 87.4, 89.8, 82.3, 85.2, 88.1, 511.7),
	(1003, 92.7, 95.1, 91.9, 93.5, 94.8, 92.4, 560.4),
	(1004, 80.3, 88.2, 84.6, 86.7, 82.9, 87.5, 510.2),
	(1005, 86.8, 91.5, 88.7, 89.4, 87.1, 90.6, 534.1),
	(1006, 79.6, 83.7, 86.9, 82.1, 85.8, 84.3, 502.4),
	(1007, 88.1, 90.6, 92.8, 89.3, 90.7, 91.2, 542.7),
	(1008, 82.5, 86.7, 83.9, 85.6, 84.1, 87.9, 510.7),
	(1009, 75.2, 79.5, 81.7, 78.4, 80.6, 79.1, 474.5),
	(1010, 93.4, 95.8, 91.2, 92.1, 94.5, 92.7, 559.7),
	(1011, 81.9, 88.7, 84.3, 87.9, 85.1, 89.2, 517.1),
	(1012, 85.7, 90.2, 88.6, 89.8, 87.4, 90.1, 531.8),
	(1013, 89.2, 92.1, 91.4, 90.5, 92.3, 90.7, 546.2),
	(1014, 78.5, 85.9, 87.2, 82.6, 84.7, 86.4, 505.3),
	(1015, 91.6, 94.5, 92.3, 93.1, 91.8, 94.2, 557.5),
	(1016, 87.3, 89.8, 86.5, 88.1, 85.9, 87.6, 525.2),
	(1017, 82.1, 86.9, 83.6, 85.7, 84.3, 87.9, 510.5),
	(1018, 79.8, 83.4, 86.7, 82.3, 85.6, 84.8, 502.6),
	(1019, 84.5, 89.1, 88.2, 88.7, 86.5, 89.3, 526.3),
	(1020, 77.9, 84.2, 86.5, 82.8, 84.6, 85.3, 501.3);




**Writing query commands**



👁️ **[Prompt example]**: 

    Write the query command:
    Find Contact_information for students whose Total_Results are less than 530 and whose English is less than 85.


**Output:**   

    Certainly! Here's the query command to find the Contact_information for students whose Total_Results are less than 530 and whose English score is less than 85:

    SELECT Contact_information
    FROM Student_Information SI
	INNER JOIN Exam_Results ER ON SI.Student_number = ER.Student_number
	WHERE ER.Total_Results < 530 AND ER.English < 85;

	This query performs an INNER JOIN between the Student_Information and Exam_Results tables on the Student_number column. It selects the Contact_information column from the Student_Information table for the students who meet the specified conditions: Total_Results less than 530 and English score less than 85.

	Feel free to modify or adjust the query based on your specific needs.

**Data Visualization**


👁️ **[Prompt example]**: 

    Using the Python language, generate a histogram of the results of each subject in the Exam_Results table  
**Output:** 

	import matplotlib.pyplot as plt
	import mysql.connector

	# Connect to the MySQL database
	connection = mysql.connector.connect(
    host="your_host",
    user="your_username",
    password="your_password",
    database="your_database"
	)

	# Create a cursor object to execute SQL queries
	cursor = connection.cursor()

	# Execute the SQL query to fetch the results for each subject
	cursor.execute("SELECT English, Mathematics, Linear_Algebra, Software_Engineering, Deep_Learning, prompt_Engineering FROM Exam_Results")

	# Fetch all the rows from the resultset
	rows = cursor.fetchall()

	# Prepare the data for histogram
	subjects = ['English', 'Mathematics', 'Linear Algebra', 'Software Engineering', 'Deep Learning', 'Prompt Engineering']
	results = [[row[i] for row in rows] for i in range(len(subjects))]

	# Generate the histogram
	plt.figure(figsize=(10, 6))
	plt.hist(results, bins=10, alpha=0.7, label=subjects)
	plt.xlabel('Result')
	plt.ylabel('Frequency')
	plt.title('Histogram of Exam Results')
	plt.legend()
	
	# Display the histogram
	plt.show()
	
	# Close the cursor and connection
	cursor.close()
	connection.close()



  

<img width="200%" src="./figures/hr.gif" />


>**In the above, we have only listed a few common usage methods and the basic ideas of prompt engineering. The powerful potential of the large language model gives us endless possibilities, further exploration and improvement of the content related to prompt engineering will further demonstrate the endless charm of the large language model.
We will continue to improve our content to present you with more ideas and methods of Prompt Engineering. If you or your team is interested in Prompt Engineering, we look forward to communicating with you and exploring  unique understanding, targeted applications, or further thoughts.**.
  
