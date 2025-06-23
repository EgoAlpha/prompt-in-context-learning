# 🌠 提示工程  👉[English Page](./promptengineering.md)👈

# 内容目录

- [1.简介](#简介)
- [2.设计原则与框架](#设计原则与框架)
- [3.提示技术的运用](#提示技术的运用) 

<img width="200%" src="./figures/hr.gif" />

## 1. 简介

提示工程是驾驭生成式大型语言模型的有力工具，能显著提升生产效率。未来，人机协作将成为主流生产方式，此趋势不可逆转。提示工程涵盖设计、创建及优化提示，旨在从大型语言模型（LLM）中获取精准、连贯且适宜的输出。

> 上述原则同样适用于图像文本合成器等其他大型生成模型。为简洁起见，本文将聚焦于语言模型。

大型语言模型在海量文本数据上训练而成，蕴含了丰富的现实世界信息。其生成类人文本的能力，使其成为聊天机器人、虚拟助手等应用的理想之选，近年来备受青睐。然而，若无恰当的提示工程，模型输出将难以预测，甚至可能与预期大相径庭。

提示工程的核心目标在于，为大型语言模型设计出恰当的提示，使其能高效解决指定的复杂任务。

提示可以是任何形式的自然语言文本，如陈述、指令、问题乃至段落，只要能激发模型的创造力，引导其探索并解决各类问题。

> 为便于初学者理解，本文暂不讨论“软提示”（Soft Prompt）的概念。

接收到各类提示后，大型语言模型能生成多样化的输出，包括完整句子、问答、翻译、对话脚本等，这些都具有广泛的应用前景和巨大的创造潜力。在训练过程中，LLM从海量语言数据中汲取知识与经验，使其不仅能作为聊天机器人与人对话，更能成为值得信赖的问题解决者。

### 💥 请注意：高质量的提示对于提升大型语言模型解决问题的能力至关重要。

<img width="200%" src="./figures/hr.gif" />


## 2.设计原则与提示框架 
　　一个好的提示是准确且具体的，并且包含足够的背景信息，让大语言模型能够产生与任务相关的反应。

### 2.1设计原则
为了确保提示语的有效性和准确性，我们需要遵循以下几个原则：

- **1. 指令清晰具体：**提示应该清楚地说明模型要回答的任务或问题。避免在提示中出现模棱两可或含糊不清的情况，因为这可能导致不清楚或不相关的回答。
- **2. 用词简洁明确：**我们应该使用简单、清晰和明确的语言来表达意思，避免使用过于复杂或模糊的词汇，以帮助模型更好地理解我们的提示。
- **3. 避免复杂句型：**我们应该尽量避免使用复杂的句型和语法结构，以减少模型理解的难度和复杂度。
- **4. 避免模糊不清：**提示语言需要确切地表达我们的意图，避免使用模棱两可或意图不明确的词语，以确保模型能够正确理解和回答问题。
- **5. 善用关键词：**我们应该使用与任务或指令相关的关键词，以帮助模型更快地理解并回答我们的问题和下达的任务。
- **6. 考虑受众对象：**我们应该控制模型输出答案的用词难度，以确保更多的人可以理解和应用。
- **7. 测试和完善：**我们需要进行反复尝试和调优，以确保最终的提示语言能够被模型准确理解并生成正确的回答。

在设计提示时，遵循以上设计原则，可以提高大语言模型输出结果的质量和准确性，从而提高我们的用户体验。

### 2.2提示框架
　　我们提出了由五个关键部分组成的提示设计框架，其中包括：背景介绍、任务指示、参考信息、输出约束和列举例子。按照这五个关键部分标准化的结构，可以帮助简化提示设计，从而产生更加有效和具有针对性的提示设计。

- **1. 背景介绍**:
  - 在设计提示时，背景介绍是关键。确保提供足够的与指定任务相关的背景信息，以便模型能够理解指令的执行背景，并生成更加相关和准确的文本。

- **2. 任务指示**:
  - 任务指示是至关重要的，因为它指导模型具体应该做什么以及对它的期望是什么。要确保我们的任务指示内容清楚、简明和具体。当处理复杂的推理任务时，考虑将任务分解成更小的、更容易管理的步骤，以帮助模型理解接收到的任务。

- **3. 参考信息**:
  - 当需要我们在提示中增加参考信息时，提供给LLM信息的相关性是很重要的。这些信息可以是相关文章或数据的链接，或者是用户提供的具体输入。通过利用这些特定的信息，可以定制模型的输出，使其具有个性化和可靠性，并与用户的需求相一致。

- **4. 输出约束**:
  - 输出约束有助于指导LLM明确能做什么和不能做什么，保证我们在最终输出中，获得更准确的结果。这可能涉及到指定输出的格式，使用的语言类型，甚至是输出的长度。此外，指定难度等级和风格，也可以进一步完善我们获得的最终输出。
- **5. 列举例子**:
  - 列举例子是很有价值的，因为它可以让LLM通过实例了解我们的预期结果，特别是当我们想得到的最终输出难以描述或者单独的指示不能有效地传达具体的细节和准确性时。通过提供一组（或多组）同时包含输入和输出的例子，LLM可以根据我们提供的示例，自动识别模式并且生成与用户期望一致的文本。

## 💥 根据任务的复杂性和不同特点，我们可以从框架中这五个关键部分中选择一些成分来组成你的提示。 

### 2.3框架与原则的应用

　　接下来，我们从一个只包含背景介绍和任务指示的基础提示开始，逐步丰富我们提示语的结构框架。以此来直观的感受，提示框架中五个关键部分所发挥的作用和不同情况下大语言模型的输出结果。

#### 2.3.1基础提示：

　　首先，我们将只包含背景介绍和任务指令的提示作为基础示例。将模型的角色定义为一名历史老师（背景介绍），并要求编写一道历史课程的选择题（任务指示）。


👁️ **[Prompt example]**:  

    背景介绍: 假设你是一名有着30年执教经验的历史老师。  
    任务指令:  编写一道历史课程的选择题。

**Output:**   

    在19世纪末期的欧洲，以下哪个国家最早实现了工业化？  
    A. 英国 B. 德国 C. 法国 D. 意大利  
    答案：A. 英国  
    解析：在19世纪末期，英国是欧洲第一个实现工业化的国家。英国在18世纪末期开始工业化进程，通过技术创新和贸易扩张，逐渐成为全球最大的工业制造国和商业中心。其他欧洲国家在随后的几十年内也逐渐实现了工业化，但英国始终是工业化的领导者。

　　根据这样的基础提示内容，大语言模型输出了相应的结果。但是，在这样相对“自由”的提示指令下，大语言模型多次生成结果中题目的形式、格式和涉及内容并不稳定。
#### 2.3.2参考信息的加入：
　　我们在基础提示的基础上，加入了“题目要涉及文艺复兴知识点”这一参考信息，来指定模型生成的输出内容的相关知识点。

👁️ **[Prompt example]**:  

    背景介绍: 假设你是一名有着30年执教经验的历史老师。  
    任务指令:  编写一道历史课程的选择题。  
    参考信息 :题目要涉及到“文艺复兴”的相关知识点。

**Output:**   

    文艺复兴是欧洲历史上的一次重大文化运动，其主要特点是：  
    A. 推崇信仰和宗教教义，重视神学研究和修道生活。  
    B. 崇尚自然和人类理性，推崇人文主义思想和人类中心主义观念。  
    C. 注重工商业的发展和经济利益的追求，推崇资本主义和市场经济。  
    D. 追求强大的军事力量和领土扩张，推崇帝国主义和殖民主义。  
    正确答案是：B.   
    解析：  
    文艺复兴是发生在欧洲文化史上的一次重要运动，其主要特点是崇尚自然和人类理性，推崇人文主义思想和人类中心主义观念。这种思想体系的建立，反映了当时欧洲人对于传统信仰和知识体系的质疑，同时也是对人类自身在自然界和社会中的地位进行重新思考的结果。因此，选项B是正确答案。

　　这种情况下，模型的输出结果保证了所涉及内容的稳定性。
#### 2.3.3输出约束的明确：
　　在提示中加入输出约束，可以明确模型应该遵循的规则或限制。我们在示例中，添加“四个选项中应当包含两个以上的正确答案”这一约束条件。

👁️ **[Prompt example]**:  

    背景介绍:假设你是一名有着30年执教经验的历史老师。  
    任务指令:编写一道历史课程的选择题。  
    参考信息:题目要涉及到“文艺复兴”的相关知识点。  
    输出约束:题目的四个选项中，应当包含两个以上的正确答案。  


**Output:**   

    以下哪些人物或事件与文艺复兴有关？（选择两个或以上正确答案）  
    A. 威廉·莎士比亚    B. 列奥纳多·达·芬奇    C. 拉斐尔    D. 贞德  
    正确答案：B、C  
    解析：  
    B. 列奥纳多·达·芬奇是意大利文艺复兴时期最重要的艺术家之一，涉及绘画、雕塑、建筑等领域，与文艺复兴有着紧密的联系。  
    C. 拉斐尔是意大利文艺复兴时期最著名的画家之一，被誉为“艺术之王”，与文艺复兴有着紧密的联系。  
    因此，选项B和C是正确答案。  

　　在稳定了输出内容（参考信息的加入）前提下，进一步明确了题目的形式为多项选择题，对最终的输出格式进行了限定。

#### 2.3.4列举例子：
　　在以上四个关键部分框架的基础上，我们可以进一步加入了可供参考的示例，为模型明确输出结果的具体细节和用自然语言不容易描述的输出格式。

👁️ **[Prompt example]**:  

    背景介绍:假设你是一名有着30年执教经验的历史老师。  
    任务指令:仿照下面的例子，编写一道历史课程的选择题。  
    参考信息:题目要涉及到“文艺复兴”的相关知识点。  
    输出约束:题目的四个选项中，应当包含两个以上的正确答案。  
    列举例子 :   
    题目：在文艺复兴时期，以下哪些城市是文化中心？  
     (A) 伦敦 (B) 巴黎 (C) 佛罗伦萨 (D) 阿姆斯特丹   
    正确答案是：A、C。  
     答案解析：在文艺复兴时期，佛罗伦萨是欧洲最重要的文化中心之一，许多重要的艺术家、学者和思想家都在这里工作和生活，包括达芬奇、米开朗基罗和但丁。伦敦也在文艺复兴时期迅速崛起，成为欧洲的文化和商业中心，吸引了许多文化名流和商人。因此，选项A和C是正确答案。

**Output:**   

    题目：文艺复兴时期的艺术家和文学家有哪些？   
    (A)高乐 
    (B) 莎士比亚
    (C) 达芬奇 
    (D) 伽利略  
    正确答案：B、C  
    答案解析：文艺复兴是15世纪末到16世纪初欧洲出现的一种新的文化、思想和艺术运动。该运动的代表人物包括艺术家    达芬奇、拉斐尔等，文学家莎士比亚、但丁等。高乐是法国作曲家，伽利略是天文学家，他们并不是文艺复兴运动的代表人物。因此，选项B、C为正确答案。

　　可以看到，大语言模型会严格按照所给示例的格式，输出了我们所需要的最终结果。

> 有时，我们可以仅仅通过多示例（甚至单一示例）的列举，就可以让大语言模型理解我们想要下达的任务指令。

👁️ **[Prompt example]**:  

    谷爱凌夺得兔年新春第一冠 得分断层优势。  
    ----体育   
    国家医保局公布的数据显示，2023年1—3月，基本医疗保险基金(含生育保险)总收入9100.48亿元，同比增长9.5%。  
    ----医疗   
    伯克希尔·哈撒韦将比亚迪股份的持股比例由 10.05% 降至 9.87%。港交所披露易规定，大股东增减持股票只有横跨    某个整数百分比时，需要作出披露。  
    ----金融  
    边缘计算产品已服务于在线教育、视频、游戏、车联网等行业客户。
    ----

**Output:**   

    科技

## 3.提示技术的运用


### 3.1基本提示
　　基于提示的方法为解决广泛的NLP任务提供了一个强大而灵活的工具。我们可以通过自然语言的指令描述来完成任务，所以不需要遵守特定的格式。

####情感分析：
　　大语言模型可以识别一段文本中所表达的情绪，如积极、消极或中立。这对于分析客户反馈、社交媒体帖子和产品评论非常有用。

👁️ **[Prompt example]**:   

    分析以下文本的情感：  
    文字：  我绝对喜欢这部电影! 演技非常棒，剧情让我在整部影片中都很投入。
 
**Output:**   

    这段文字表达了积极的情感，特别是强烈的喜欢和投入感。具体来说，可以从以下几个方面来分析：  
    1. 喜欢： "我绝对喜欢"这句话明确表明了作者对这部电影的态度，而且使用了强调词"绝对"，进一步突出了这种情感。   
    2. 演技非常棒：这句话表达了对电影演员的赞扬，也是对电影整体质量的肯定。   
    3. 剧情让我在整部影片中都很投入：这句话突出了作者对剧情的认可，同时也表达了在观影过程中的身临其境的感受，即投入感。  
    因此，可以得出这段文字的情感是积极的。
####实体识别：
　　大语言模型可以识别文本中的实体，如人、地方、组织和产品。这可用于各种领域的命名实体识别，如新闻文章或法律文件。

👁️ **[Prompt example]**:  

    分析以下段落，找出文中提到的所有人物、地点和组织，然后以Json格式输出结果。  
    文本：苹果公司的活动在加州库珀蒂诺的史蒂夫-乔布斯剧院举行。苹果公司首席执行官蒂姆-库克（Tim Cook）介绍了新的iPhone 13，该手机将从下周开始接受预购。这款手机有几种颜色，具有更快的处理器和更长的电池寿命。

**Output:**   

    {
    "人物": ["史蒂夫-乔布斯", "蒂姆-库克"],
    "地点": ["加州库珀蒂诺"],
    "组织": ["苹果公司"],
    "其他": ["iPhone 13"]
    }
####关系提取：
　　大语言模型也可以提取一段文本中实体之间的关系，例如确定一个人是一个公司的CEO或者一个产品是由某个品牌生产的。这对知识图谱构建等任务很有用，在这些任务中，实体之间的关系对理解该领域很重要。

👁️ **[Prompt example]**:  

    分析以下句子，提取两个实体之间的关系，然后以JSON格式输出结果。  
    文本： 埃隆-马斯克在2002年创立了SpaceX，目标是降低太空运输成本，实现火星殖民化。

**Output:**   

    {
      "实体1": "埃隆-马斯克",
      "实体2": "SpaceX",
      "关系": "创立"
    }
####文本总结：
　　大语言模型可以对文本内容进行总结，自动生成一篇较长文本的摘要，如一篇文章或报告。这对快速理解文件的关键点很有帮助，而不需要阅读整个文件。

👁️ **[Prompt example]**:  

    总结以下段落：   
    我们是否知道我们心中的风筝到底在什么地方，人生错过就不会再得到，也许我们会忏悔，会救赎，但这些似乎都已经晚了，每当天空放飞起风筝的那一刻，我们是不是应该问问自己我们是否真的珍惜我们所拥有的一切。
    我们每个人或多或少都在年幼的时候做过一些让自己今后感到羞愧的事，这些事可能如影子一般伴随自己一生，让你只能低着头去看它。可是时光不会掉头，自己尽力的弥补，何尝不是一种自我拯救呢？儿时的美好和友情，因为一个懦弱的疏忽而毁于一旦，如果再给你一次机会，你愿意不顾一切地去重新找回那个曾经的自己吗？
    可是人就是这样，总会活在某个时限内，那里的世界也许是几年之后连自己都无法理解的，但这又是我们无法突破的。为你，千千万万遍，遍体鳞伤还是会义无反顾，也许这就是人生，人生不是只做值得的事情！

**Output:**   

    这段文字探讨了人们在人生旅途中可能会面临的一些问题和挑战。  
    首先，它强调了人们应该珍惜所拥有的一切，因为生命中某些机会只会出现一次，错过了就不会再回来。  
    其次，文章提到了许多人在童年时犯下的错误，这些错误可能会伴随人们的一生，但通过努力弥补这些错误，也许可以实现自我拯救。  
    最后，这段文字表达了人们常常被困在某个时期的思维模式中，无法真正超越自己的限制。但是即使生命中充满了伤痛和不幸，人们仍然会义无反顾地前行，因为这就是生命的真谛，而不仅仅是做一些看似值得的事情。

####文本分类：
　　大语言模型可以将文本分为预定义的类别，例如将新闻文章分为不同的主题或将客户咨询分为不同类型。这对内容审核等任务很有用，因为在这些任务中，需要对传入的文本进行快速和准确的分类。

👁️ **[Prompt example]**:  

    将以下一组新闻文章根据其内容分为不同的组别：  
    "尽管有大流行病，但特斯拉的电动汽车销量仍在飙升"  
    "新的研究表明饮用咖啡可能会降低患心脏病的风险"  
    "最新的iPhone型号具有更大的屏幕和改进的摄像头"  
    "COVID-19病例在印度激增，使医疗系统不堪重负"   
    "亚马逊宣布计划在德克萨斯州建立一个新的履行中心"  
    "科学家在亚马逊雨林中发现新的鸟类物种"  
    "全球气候变化会议将于下个月在巴黎举行"  
    "星巴克在美国所有门店推出植物奶选择"  
**Output:**   

    根据文章内容，可以将新闻文章分为以下几个组别：  
    1. 商业和科技：  
    - "尽管有大流行病，但特斯拉的电动汽车销量仍在飙升"  
    - "最新的iPhone型号具有更大的屏幕和改进的摄像头"  
    - "亚马逊宣布计划在德克萨斯州建立一个新的履行中心"  
    2. 健康和医疗：  
    - "新的研究表明饮用咖啡可能会降低患心脏病的风险"  
    - "COVID-19病例在印度激增，使医疗系统不堪重负"  
    3. 环境和自然：  
    - "科学家在亚马逊雨林中发现新的鸟类物种"  
    - "全球气候变化会议将于下个月在巴黎举行"  
    4. 餐饮和食品：  
    - "星巴克在美国所有门店推出植物奶选择"  
    注意：这些分类是根据文章的主要内容和关键词进行的，可能存在一定的主观性，不同的人可能会进行不同的分类。

####机器翻译：
　　大语言模型可用于机器翻译，他们可以将文本从一种语言翻译成另一种语言。这对在全球范围内经营的企业以及需要与讲不同语言的人沟通的个人来说都很有用。

👁️ **[Prompt example]**:  

    将以下段落翻译成中文。  
    Tales from Shakespeare is an English children's book written by Charles Lamb and his sister Mary Lamb in 1807. The book is designed to make the stories of Shakespeare's plays familiar to the young. However, as noted in the author's Preface, "[Shakespeare's] words are used whenever it seemed possible to bring them in; and in whatever has been added to give them the regular。

**Output:**   

    《莎士比亚故事集》是一本英文儿童读物，由查尔斯·兰姆和他的姐姐玛丽·兰姆于1807年写成。这本书旨在使莎士比亚的剧作故事对年轻人更加熟悉。然而，正如作者的前言中所指出的那样，"莎士比亚的话语在任何可能引入的地方都被使用了；而且在添加的任何内容中都会使它们变得更加规范。"

####回答问题：
　　大语言模型可用于回答问题，它们可以阅读一段文字并回答有关问题。这对客户支持等应用很有用，客户可以提出问题并得到快速、准确的回答。

👁️ **[Prompt example]**:  

    大堡礁是世界上最大的珊瑚礁系统，由2,900多个独立的珊瑚礁和900个岛屿组成，绵延2,300多公里。它位于澳大利亚沿海的珊瑚海中。大堡礁是各种海洋生物的家园，包括1500多种鱼类，600多种珊瑚，以及众多其他物种。什么是大堡礁，它位于哪里？

**Output:**   

    大堡礁是世界上最大的珊瑚礁系统，位于澳大利亚东海岸的珊瑚海中，从昆士兰州北部的托雷斯海峡一直延伸到南部的伊纳拉沙漠。它由2,900多个独立的珊瑚礁和900个岛屿组成，绵延2,300多公里。大堡礁是各种海洋生物的家园，包括1500多种鱼类，600多种珊瑚，以及众多其他物种。

> 为了充分的发挥ChatGPT强大的生成能力，除了自然语言任务的生成之外，我们可以着眼于更多方面或者领域的生成任务。

### 3.2生成指定的编程语言
　　大语言模型可以根据自然语言描述编写相应任务的python（或者其他编程语言）代码。在这一类任务中，大语言模型所生成的代码有时也会出现错误，但我们可以将错误代码直接反馈给大语言模型，它会谦虚的承认错误并对代码进行调试与纠错。  
　　在下面的示例中，我们要求模型根据我们的提示实现大量EXCEL表格内容的汇总，将所有EXCEL成绩单汇总到总成绩单表格中，根据总成绩进行重新排序。

👁️ **[Prompt example]**:  

    假设你是一名熟练掌握python语言编写程序的程序员。  
    我需要将给定文件夹中的所有EXCEL表格数据，汇总到一个给定的EXCEL表格中，编写python要求如下：  
    1.分表中，各列分别是考生编号、考生姓名、培养方式、专业代码、专业名称、专业编号、专业课名称、英语分数、政治分数、数学分数、专业课分数、总分和备注。但是在第一行没有进行标注 。  
    2.总表格式要与分表相同，并且根据总分将分表中的数据由高到低进行排名。   
    3.做一个程序运行进度条，表示已经复制好的数据数量。  

**Output:**   

    import os    
    import openpyxl    
    from openpyxl.utils import get_column_letter    
    from openpyxl.styles import Font    
    from tqdm import tqdm    
    def merge_excel_files(folder_path, output_file):
    # 获取文件夹中所有的Excel文件路径
    excel_files = [file for file in os.listdir(folder_path) if file.endswith('.xlsx')]

    if not excel_files:
        print("文件夹中不存在Excel文件！")
        return

    # 创建输出Excel文件
    wb_output = openpyxl.Workbook()
    ws_output = wb_output.active

    # 复制第一张表格的表头到总表
    first_file = os.path.join(folder_path, excel_files[0])
    wb_first = openpyxl.load_workbook(first_file)
    ws_first = wb_first.active

    # 获取第一张表格的表头行
    header_row = ws_first[1]

    # 复制表头到总表
    for col_num, cell in enumerate(header_row, 1):
        col_letter = get_column_letter(col_num)
        ws_output[f'{col_letter}1'] = cell.value
        ws_output.column_dimensions[col_letter].width = ws_first.column_dimensions[col_letter].width
        ws_output[f'{col_letter}1'].font = Font(bold=True)

    # 复制所有表格数据到总表
    total_rows = 0
    progress_bar = tqdm(total=len(excel_files), desc='正在复制数据', unit='个')

    for file in excel_files:
        file_path = os.path.join(folder_path, file)
        workbook = openpyxl.load_workbook(file_path)
        worksheet = workbook.active

        # 复制每行数据到总表
        for row_num, row in enumerate(worksheet.iter_rows(min_row=2), start=2):
            total_rows += 1
            progress_bar.update(1)

            for col_num, cell in enumerate(row, 1):
                col_letter = get_column_letter(col_num)
                ws_output[f'{col_letter}{total_rows+1}'] = cell.value

        workbook.close()

    progress_bar.close()

    # 根据总分将数据进行排名
    ws_output.auto_filter.ref = ws_output.dimensions
    ws_output.auto_filter.add_sort_condition('M2:M' + str(total_rows+1))

    # 保存总表
    wb_output.save(output_file)
    wb_output.close()

    print(f"已将 {total_rows} 条数据复制到总表 {output_file} 中。")

    # 示例用法
    folder_path = '/path/to/excel/files'  # 替换为实际的文件夹路径
    output_file = '/path/to/output/excel.xlsx'  # 替换为实际的输出文件路径

    merge_excel_files(folder_path, output_file)



### 3.3办公软件宏命令生成
　　日常办公软件中相对复杂的工作内容，我们也可以利用准确的提示语，让模型为我们实现指定的操作内容。  
　　示例中，我们要求大语言模型编写EXCEL宏命令将表格中英语成绩在50-70之间的位置标红，并在同一行的备注栏写入“待处理”。

👁️ **[Prompt example]**:  

    假设你是一名熟练使用EXCEL宏命令编写的数据员。
    为我的EXCEL表格编写一个宏命令VBA。
    将所有H列在50到70之间的数据标红并加粗。同时在这些行的M列中，写入“待处理”，

**Output:**   

    Sub 标记待处理数据()
       Dim ws As Worksheet
       Dim lastRow As Long
       Dim rng As Range
       Dim cell As Range
    
       ' 设置要操作的工作表
       Set ws = ThisWorkbook.Sheets("Sheet1") ' 将 "Sheet1" 替换为你的工作表名称
    
       ' 获取H列的范围
       lastRow = ws.Cells(ws.Rows.Count, "H").End(xlUp).Row
       Set rng = ws.Range("H1:H" & lastRow)
    
       ' 循环遍历H列中的每个单元格
       For Each cell In rng
           ' 检查单元格的值是否在50到70之间
           If cell.Value >= 50 And cell.Value <= 70 Then
               ' 标记为红色并加粗
               cell.Font.Color = RGB(255, 0, 0) ' 将红色的RGB值替换为你想要的颜色
               cell.Font.Bold = True
               
               ' 在相应的M列写入"待处理"
               ws.Cells(cell.Row, "M").Value = "待处理"
           End If
       Next cell   
    End Sub
### 3.4SQL语句的生成
　　在数据库管理方面，我们也可以利用准确的提示语，要求大语言模型为我们编写相应功能的SQL语句。

**创建表格**

👁️ **[Prompt example]**:  

    假设你是一名熟练掌握MySQL语言的数据库管理员，根据我的要求编写MySQL语言。  
    创建两张基本表 ：  
    表1：名称为Student\_Information，表头包含Student\_number（8位） 、name、gender 、age 、Major 、 Contact\_information 。其中Student\_number和age为int型，其余均为char型。Student\_number为主键。   
    表2：名称Exam\_Results，表头包含Student\_number、 English 、 Mathematics 、Linear\_Algebra 、Software\_Engineering 、Deep\_Learning 、prompt\_Engineering和Total\_Results，数据类型均为int型。Student\_number为主键，除Total\_Results以外各科目成绩按照百分制记录。


**Output:**  

     -- 创建Student_Information表
        CREATE TABLE Student_Information (
          Student_number INT(8) NOT NULL,
          name CHAR(50) NOT NULL,
          gender CHAR(10) NOT NULL,
          age INT NOT NULL,
          Major CHAR(50) NOT NULL,
          Contact_information CHAR(100) NOT NULL,
          PRIMARY KEY (Student_number)
        );

        -- 创建Exam_Results表
        CREATE TABLE Exam_Results (
          Student_number INT(8) NOT NULL,
          English INT NOT NULL,
          Mathematics INT NOT NULL,
          Linear_Algebra INT NOT NULL,
          Software_Engineering INT NOT NULL,
          Deep_Learning INT NOT NULL,
          prompt_Engineering INT NOT NULL,
          Total_Results INT NOT NULL,
          PRIMARY KEY (Student_number)
        );
 
**生成模拟数据**

👁️ **[Prompt example]**:  

    为Student\_Information模拟生成20条数据

**Output:**   

    INSERT INTO Student_Information (Student_number, name, gender, age, Major, Contact_information) VALUES
    (10000001, '张三', '男', 20, '计算机科学', 'zhangsan@example.com'),
    (10000002, '李四', '男', 21, '数学', 'lisi@example.com'),
    (10000003, '王五', '女', 19, '物理学', 'wangwu@example.com'),
    (10000004, '赵六', '男', 22, '化学', 'zhaoliu@example.com'),
    (10000005, '陈七', '女', 20, '经济学', 'chenqi@example.com'),
    (10000006, '刘八', '男', 21, '历史学', 'liuba@example.com'),
    (10000007, '宋九', '女', 19, '英语', 'songjiu@example.com'),
    (10000008, '钱十', '男', 22, '地理学', 'qianshi@example.com'),
    (10000009, '周十一', '女', 20, '政治学', 'zhoushiyi@example.com'),
    (10000010, '吴十二', '男', 21, '文学', 'wushier@example.com'),
    (10000011, '郑十三', '女', 19, '哲学', 'zhengshisan@example.com'),
    (10000012, '孙十四', '男', 22, '法律', 'sunshisi@example.com'),
    (10000013, '杨十五', '女', 20, '社会学', 'yangshiwu@example.com'),
    (10000014, '徐十六', '男', 21, '心理学', 'xushiliu@example.com'),
    (10000015, '朱十七', '女', 19, '生物学', 'zhushiqi@example.com'),
    (10000016, '秦十八', '男', 22, '地球科学', 'qinshiba@example.com'),
    (10000017, '许十九', '女', 20, '统计学', 'xushijiu@example.com'),
    (10000018, '何二十', '男', 21, '人类学', 'heershi@example.com'),
    (10000019, '马廿一', '女', 19, '医学', 'mashiyi@example.com'),
    (10000020, '罗廿二', '男', 22, '工程学', 'luoshier@example.com');


👁️ **[Prompt example]**:  

    在模拟生成的Student\_Information中数据的基础上，为Exam\_Results生成20条模拟数据

**Output:**   

    INSERT INTO Exam_Results (Student_number, English, Mathematics, Linear_Algebra, 
    Software_Engineering, Deep_Learning, prompt_Engineering, Total_Results) VALUES
    (10000001, 85, 90, 92, 88, 87, 90, 532),
    (10000002, 78, 85, 90, 92, 89, 85, 519),
    (10000003, 92, 88, 87, 90, 92, 88, 537),
    (10000004, 85, 90, 92, 88, 87, 90, 532),
    (10000005, 78, 85, 90, 92, 89, 85, 519),
    (10000006, 92, 88, 87, 90, 92, 88, 537),
    (10000007, 85, 90, 92, 88, 87, 90, 532),
    (10000008, 78, 85, 90, 92, 89, 85, 519),
    (10000009, 92, 88, 87, 90, 92, 88, 537),
    (10000010, 85, 90, 92, 88, 87, 90, 532),
    (10000011, 78, 85, 90, 92, 89, 85, 519),
    (10000012, 92, 88, 87, 90, 92, 88, 537),
    (10000013, 85, 90, 92, 88, 87, 90, 532),
    (10000014, 78, 85, 90, 92, 89, 85, 519),
    (10000015, 92, 88, 87, 90, 92, 88, 537),
    (10000016, 85, 90, 92, 88, 87, 90, 532),
    (10000017, 78, 85, 90, 92, 89, 85, 519),
    (10000018, 92, 88, 87, 90, 92, 88, 537),
    (10000019, 85, 90, 92, 88, 87, 90, 532),
    (10000020, 78, 85, 90, 92, 89, 85, 519);


**编写查询命令**

👁️ **[Prompt example]**:  

    编写查询命令：查找Total\_Results小于530且English小于85的学生的 Contact\_information


**Output:**   

    要查找Total\_Results小于530且English小于85的学生的Contact\_information，可以使用SELECT语句结合WHERE子句进行筛选。以下是查询命令：

    SELECT Contact_information
    FROM Student_Information
    JOIN Exam_Results ON Student_Information.Student_number = Exam_Results.Student_number
    WHERE Total_Results < 530 AND English < 85;

    这条查询命令使用了JOIN语句来关联Student\_Information和Exam\_Results两张表，基于Student\_number字段进行连接。然后，在WHERE子句中设置条件，筛选出Total\_Results小于530且English小于85的学生。最后，SELECT语句选择了满足条件的学生的Contact\_information字段作为结果。

    执行以上查询命令后，将会返回满足条件的学生的联系信息(Contact\_information)。请注意，根据实际数据和需求，可能会有不同的查询结果。

**数据可视化**

👁️ **[Prompt example]**:  

    利用Python语言，生成Exam_Results表各科目成绩的柱状图

**Output:**   

    要使用Python语言生成Exam_Results表各科目成绩的柱状图，我们可以使用matplotlib库进行可视化。首先，需要从MySQL数据库中获取数据，并将其存储在Python的数据结构中，然后使用matplotlib绘制柱状图。以下是一个示例代码：

    import mysql.connector
    import matplotlib.pyplot as plt

    # 连接到MySQL数据库
    cnx = mysql.connector.connect(
        host='your_host',
        user='your_username',
        password='your_password',
        database='your_database'
        )

    # 获取数据
    cursor = cnx.cursor()
    query = "SELECT English, Mathematics, Linear_Algebra, Software_Engineering, Deep_Learning, prompt_Engineering FROM Exam_Results"
    cursor.execute(query)
    results = cursor.fetchall()

    # 关闭数据库连接
    cursor.close()
    cnx.close()

    # 提取各科目成绩数据
    english_scores = [result[0] for result in results]
    math_scores = [result[1] for result in results]
    linear_algebra_scores = [result[2] for result in results]
    software_engineering_scores = [result[3] for result in results]
    deep_learning_scores = [result[4] for result in results]
    prompt_engineering_scores = [result[5] for result in results]
    
    # 设置柱状图的数据和标签
    subjects = ['English', 'Mathematics', 'Linear Algebra', 'Software Engineering', 'Deep Learning', 'Prompt Engineering']
    scores = [english_scores, math_scores, linear_algebra_scores, software_engineering_scores, deep_learning_scores, prompt_engineering_scores]

    # 绘制柱状图
    plt.figure(figsize=(10, 6))
    plt.bar(subjects, [sum(score) / len(score) for score in scores])  # 计算每科成绩的平均值并绘制柱状图
    plt.xlabel('Subjects')
    plt.ylabel('Average Score')
    plt.title('Exam Results - Average Scores')
    plt.xticks(rotation=45)
    
    # 显示图形
    plt.tight_layout()
    plt.show()```
　　
  

<img width="200%" src="./figures/hr.gif" />



>**以上的内容，我们仅仅列举出了几种常见的使用方法和提示工程的基本思想。大语言模型的强大潜力赋予了我们无穷的可能，对于提示工程相关内容的不断探索和完善，也必将进一步展现大语言模型的无穷魅力。
我们也会不断更新和完善我们的内容，力争向您呈现更多的提示工程的思想与方法。如果您或者您的团队也对提示工程充满兴趣，无论是独特的理解、针对性的应用、亦或是进一步的思考，我们都期待与您的交流和共同探索。**
