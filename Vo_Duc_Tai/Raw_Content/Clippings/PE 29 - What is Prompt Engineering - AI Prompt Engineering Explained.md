---
source: "https://aws.amazon.com/what-is/prompt-engineering/"
author:
published:
tags:
  - "clipping"
  - "article"
  - "aws"
  - "prompt-engineering"
---
# What is Prompt Engineering? - AI Prompt Engineering Explained

## What is Prompt Engineering?

[Create an AWS Account](https://portal.aws.amazon.com/gp/aws/developer/registration/index.html?pg=what_is_header)

## Page topics

## What is prompt engineering?

Prompt engineering is the process where you guide [generative artificial intelligence (generative AI](https://aws.amazon.com/what-is/generative-ai/)) solutions to generate desired outputs. Even though generative AI attempts to mimic humans, it requires detailed instructions to create high-quality and relevant output. In prompt engineering, you choose the most appropriate formats, phrases, words, and symbols that guide the AI to interact with your users more meaningfully. Prompt engineers use creativity plus trial and error to create a collection of input texts, so an application's generative AI works as expected.

## What is a prompt?

A prompt is a natural language text that requests the [generative AI](https://aws.amazon.com/ai/generative-ai/) to perform a specific task. Generative AI is an artificial intelligence solution that creates new content like stories, conversations, videos, images, and music. It's powered by very large machine learning (ML) models that use deep neural networks that have been pretrained on vast amounts of data.

The large language models (LLMs) are very flexible and can perform various tasks. For example, they can summarize documents, complete sentences, answer questions, and translate languages. For specific user input, the models work by predicting the best output that they determine from past training.

However, because they're so open-ended, your users can interact with generative AI solutions through countless input data combinations. The AI language models are very powerful and don't require much to start creating content. Even a single word is sufficient for the system to create a detailed response.

That being said, not every type of input generates helpful output. Generative AI systems require context and detailed information to produce accurate and relevant responses. When you systematically design prompts, you get more meaningful and usable creations. In prompt engineering, you continuously refine prompts until you get the desired outcomes from the AI system.

[Read about generative AI »](https://aws.amazon.com/what-is/generative-ai/)

[Read about large language models (LLMs) »](https://aws.amazon.com/what-is/large-language-model/)

## Why is prompt engineering important?

Prompt engineering jobs have increased significantly since the launch of generative AI. Prompt engineers bridge the gap between your end users and the large language model. They identify scripts and templates that your users can customize and complete to get the best result from the language models. These engineers experiment with different types of inputs to build a prompt library that application developers can reuse in different scenarios.

Prompt engineering makes AI applications more efficient and effective. Application developers typically encapsulate open-ended user input inside a prompt before passing it to the AI model.

For example, consider AI [chatbots](https://aws.amazon.com/what-is/chatbot/). A user may enter an incomplete problem statement like, *"Where to purchase a shirt."* Internally, the application's code uses an engineered prompt that says, *"You are a sales assistant for a clothing company. A user, based in Alabama, United States, is asking you where to purchase a shirt. Respond with the three nearest store locations that currently stock a shirt."* The chatbot then generates more relevant and accurate information.

Next, we discuss some benefits of prompt engineering.

### Greater developer control

Prompt engineering gives developers more control over users' interactions with the AI. Effective prompts provide intent and establish context to the large language models. They help the AI refine the output and present it concisely in the required format.

They also prevent your users from misusing the AI or requesting something the AI does not know or cannot handle accurately. For instance, you may want to limit your users from generating inappropriate content in a business AI application.

### Improved user experience

Users avoid trial and error and still receive coherent, accurate, and relevant responses from AI tools. Prompt engineering makes it easy for users to obtain relevant results in the first prompt. It helps mitigate bias that may be present from existing human bias in the large language models’ training data.

Further, it enhances the user-AI interaction so the AI understands the user's intention even with minimal input. For example, requests to summarize a legal document and a news article get different results adjusted for style and tone. This is true even if both users just tell the application, *"Summarize this document."*

### Increased flexibility

Higher levels of abstraction improve AI models and allow organizations to create more flexible tools at scale. A prompt engineer can create prompts with domain-neutral instructions highlighting logical links and broad patterns. Organizations can rapidly reuse the prompts across the enterprise to expand their AI investments.

For example, to find opportunities for process optimization, the prompt engineer can create different prompts that train the AI model to find inefficiencies using broad signals rather than context-specific data. The prompts can then be used for diverse processes and business units.

## What are some prompt engineering use cases?

Prompt engineering techniques are used in sophisticated AI systems to improve user experience with the learning language model. Here are some examples.

### Subject matter expertise

Prompt engineering plays a key role in applications that require the AI to respond with subject matter expertise. A prompt engineer with experience in the field can guide the AI to reference the correct sources and frame the answer appropriately based on the question asked.

For example, in the medical field, a physician could use a prompt-engineered language model to generate differential diagnoses for a complex case. The medical professional only needs to enter the symptoms and patient details. The application uses engineered prompts to guide the AI first to list possible diseases associated with the entered symptoms. Then it narrows down the list based on additional patient information.

### Critical thinking

Critical thinking applications require the language model to solve complex problems. To do so, the model analyzes information from different angles, evaluates its credibility, and makes reasoned decisions. Prompt engineering enhances a model's data analysis capabilities.

For instance, in decision-making scenarios, you could prompt a model to list all possible options, evaluate each option, and recommend the best solution.

### Creativity

Creativity involves generating new ideas, concepts, or solutions. Prompt engineering can be used to enhance a model's creative abilities in various scenarios.

For instance, in writing scenarios, a writer could use a prompt-engineered model to help generate ideas for a story. The writer may prompt the model to list possible characters, settings, and plot points then develop a story with those elements. Or a graphic designer could prompt the model to generate a list of color palettes that evoke a certain emotion then create a design using that palette.

## What are prompt engineering techniques?

Prompt engineering is a dynamic and evolving field. It requires both linguistic skills and creative expression to fine-tune prompts and obtain the desired response from the generative AI tools.

[Read the guide to prompt engineering by AWS PartyRock »](https://partyrock.aws/u/js2222/zEj353AmT/Prompt-Engineering-Guide-Introduction)

Here are some more examples of techniques that prompt engineers use to improve their AI models' natural language processing (NLP) tasks.

### Chain-of-thought prompting

Chain-of-thought prompting is a technique that breaks down a complex question into smaller, logical parts that mimic a train of thought. This helps the model solve problems in a series of intermediate steps rather than directly answering the question. This enhances its reasoning ability.

You can perform several chain-of-though rollouts for complex tasks and choose the most commonly reached conclusion. If the rollouts disagree significantly, a person can be consulted to correct the chain of thought.

For example, if the question is *"What is the capital of France?"* the model might perform several rollouts leading to answers like *"Paris,"* **"The capital of France is Paris,"** and *"Paris is the capital of France."* Since all rollouts lead to the same conclusion, *"Paris"* would be selected as the final answer.

### Tree-of-thought prompting

The tree-of-thought technique generalizes chain-of-thought prompting. It prompts the model to generate one or more possible next steps. Then it runs the model on each possible next step using a tree search method.

For example, if the question is *"What are the effects of climate change?"* the model might first generate possible next steps like *"List the environmental effects* *"* and *"List the social effects."* It would then elaborate on each of these in subsequent steps.

### Maieutic prompting

Maieutic prompting is similar to tree-of-thought prompting. The model is prompted to answer a question with an explanation. The model is then prompted to explain parts of the explanation,. Inconsistent explanation trees are pruned or discarded. This improves performance on complex commonsense reasoning.

For example, if the question is *"Why is the sky blue?"* the model might first answer, *"The sky appears blue to the human eye because the short waves of blue light are scattered in all directions by the gases and particles in the Earth's atmosphere."* It might then expand on parts of this explanation, such as why blue light is scattered more than other colors and what the Earth's atmosphere is composed of.

### Complexity-based prompting

This prompt-engineering technique involves performing several chain-of-thought rollouts. It chooses the rollouts with the longest chains of thought then chooses the most commonly reached conclusion.

For example, if the question is a complex math problem, the model might perform several rollouts, each involving multiple steps of calculations. It would consider the rollouts with the longest chain of thought, which for this example would be the most steps of calculations. The rollouts that reach a common conclusion with other rollouts would be selected as the final answer.

### Generated knowledge prompting

This technique involves prompting the model to first generate relevant facts needed to complete the prompt. Then it proceeds to complete the prompt. This often results in higher completion quality as the model is conditioned on relevant facts.

For example, imagine a user prompts the model to write an essay on the effects of deforestation. The model might first generate facts like **"deforestation contributes to climate change"** and **"deforestation leads to loss of biodiversity."** Then it would elaborate on the points in the essay.

### Least-to-most prompting

In this prompt engineering technique, the model is prompted first to list the subproblems of a problem, and then solve them in sequence. This approach ensures that later subproblems can be solved with the help of answers to previous subproblems.

For example, imagine that a user prompts the model with a math problem like *"Solve for x in equation 2x + 3 = 11*." The model might first list the subproblems as *"Subtract 3 from both sides"* and *"Divide by 2"*. It would then solve them in sequence to get the final answer.

### Self-refine prompting

In this technique, the model is prompted to solve the problem, critique its solution, and then resolve the problem considering the problem, solution, and critique. The problem-solving process repeats until a it reaches a predetermined reason to stop. For example, it could run out of tokens or time, or the model could output a stop token.

For example, imagine a user prompts a model, *"Write a short essay on literature."* The model might draft an essay, critique it for lack of specific examples, and rewrite the essay to include specific examples. This process would repeat until the essay is deemed satisfactory or a stop criterion is met.

### Directional-stimulus prompting

This prompt engineering technique includes a hint or cue, such as desired keywords, to guide the language model toward the desired output.

For example, if the prompt is to write a poem about love, the prompt engineer may craft prompts that include *"heart,"* *"passion,"* and *"eternal."* The model might be prompted, *"Write a poem about love that includes the words 'heart,' 'passion,' and 'eternal'."* This would guide the model to craft a poem with these keywords.

## What are some prompt engineering best practices?

Good prompt engineering requires you to communicate instructions with context, scope, and expected response. Next, we share some best practices.

### Unambiguous prompts

Clearly define the desired response in your prompt to avoid misinterpretation by the AI. For instance, if you are asking for a novel summary, clearly state that you are looking for a summary, not a detailed analysis. This helps the AI to focus only on your request and provide a response that aligns with your objective.

### Adequate context within the prompt

Provide adequate context within the prompt and include output requirements in your prompt input, confining it to a specific format. For instance, say you want a list of the most popular movies of the 1990s in a table. To get the exact result, you should explicitly state how many movies you want to be listed and ask for table formatting.

### Balance between targeted information and desired output

Balance simplicity and complexity in your prompt to avoid vague, unrelated, or unexpected answers. A prompt that is too simple may lack context, while a prompt that is too complex may confuse the AI. This is especially important for complex topics or domain-specific language, which may be less familiar to the AI. Instead, use simple language and reduce the prompt size to make your question more understandable.

### Experiment and refine the prompt

Prompt engineering is an iterative process. It's essential to experiment with different ideas and test the AI prompts to see the results. You may need multiple tries to optimize for accuracy and relevance. Continuous testing and iteration reduce the prompt size and help the model generate better output. There are no fixed rules for how the AI outputs information, so flexibility and adaptability are essential.

## How can AWS support your generative AI requirements?

Amazon Web Services (AWS) offers the breadth and depth of tools to build and use generative AI. For example, you can use these services:

- [Amazon CodeWhisperer](https://aws.amazon.com/q/developer/) to [generate code suggestions](https://aws.amazon.com/what-is/ai-coding/) ranging from snippets to full functions in real time based on your comments and existing code.
- [Amazon Bedrock](https://aws.amazon.com/bedrock/) to accelerate development of generative AI applications using language models through an API, without managing infrastructure.
- [Amazon SageMaker JumpStart](https://aws.amazon.com/sagemaker/jumpstart/) to discover, explore, and deploy open source language models. For example, you can work with models like OpenLLaMA, RedPajama, MosaicML's MPT-7B, FLAN-T5, GPT-NeoX-20B, and BLOOM.

If you prefer to create your own models, use [Amazon SageMaker](https://aws.amazon.com/sagemaker/). It provides managed infrastructure and tools to accelerate scalable, reliable, and secure model building, training, and deployment.

Get started with prompt engineering on AWS by [creating an account](https://portal.aws.amazon.com/billing/signup/) today.

## Browse all cloud computing concepts

Browse all cloud computing concepts content here:

Displaying 1-8 (293)[2022-08-08](https://aws.amazon.com/what-is/iaas/?trk=faq_card)

#### What is IaaS (Infrastructure as a Service)?

Infrastructure as a Service (IaaS) is a business model that delivers IT infrastructure like compute, storage, and network resources on a pay-as-you-go basis over the internet. You can use IaaS to request and configure the resources you require to run your applications and IT systems. You are responsible for deploying, maintaining, and supporting your applications, and the IaaS provider is responsible for maintaining the physical infrastructure. Infrastructure as a Service gives you flexibility and control over your IT resources in a cost-effective manner.

Learn more

[View original](https://aws.amazon.com/what-is/iaas/?trk=faq_card)[2022-05-25](https://aws.amazon.com/what-is/machine-translation/?trk=faq_card)

#### What is Machine Translation?

Machine translation is the process of using artificial intelligence to automatically translate text from one language to another without human involvement. Modern machine translation goes beyond simple word-to-word translation to communicate the full meaning of the original language text in the target language. It analyzes all text elements and recognizes how the words influence one another.

Learn more

[View original](https://aws.amazon.com/what-is/machine-translation/?trk=faq_card)[2022-08-12](https://aws.amazon.com/what-is/block-storage/?trk=faq_card)

#### What is Block Storage?

Block storage is technology that controls data storage and storage devices. It takes any data, like a file or database entry, and divides it into blocks of equal sizes. The block storage system then stores the data block on underlying physical storage in a manner that is optimized for fast access and retrieval. Developers prefer block storage for applications that require efficient, fast, and reliable data access. Think of block storage as a more direct pipeline to the data as opposed to file storage which has an extra layer consisting of a file system (NFS, SMB) to process before accessing the data.

Learn more

[View original](https://aws.amazon.com/what-is/block-storage/?trk=faq_card)[2021-09-29](https://aws.amazon.com/relational-database/?trk=faq_card)

#### What is a Relational Database?

A relational database is a collection of data items with pre-defined relationships between them. These items are organized as a set of tables with columns and rows. Tables are used to hold information about the objects to be represented in the database. Each column in a table holds a certain kind of data and a field stores the actual value of an attribute. The rows in the table represent a collection of related values of one object or entity. Each row in a table could be marked with a unique identifier called a primary key, and rows among multiple tables can be made related using foreign keys. This data can be accessed in many different ways without reorganizing the database tables themselves.

Learn more

[View original](https://aws.amazon.com/relational-database/?trk=faq_card)[2023-10-02](https://aws.amazon.com/what-is/advanced-analytics/?trk=faq_card)

#### What is Advanced Analytics?

Advanced analytics is the process of using complex machine learning (ML) and visualization techniques to derive data insights beyond traditional business intelligence. Modern organizations collect vast volumes of data and analyze it to discover hidden patterns and trends. They use the information to improve business process efficiency and customer satisfaction. With advanced analytics, you can take this one step further and use data for future and real-time decision-making. Advanced analytics techniques also derive meaning from unstructured data like social media comments or images. They can help your organization solve complex problems more efficiently. Advancements in cloud computing and data storage have made advanced analytics more affordable and accessible to all organizations.

Learn more

[View original](https://aws.amazon.com/what-is/advanced-analytics/?trk=faq_card)[2023-10-04](https://aws.amazon.com/what-is/gpu/?trk=faq_card)

#### What is a GPU?

A graphics processing unit (GPU) is an electronic circuit that can perform mathematical calculations at high speed. Computing tasks like graphics rendering, machine learning (ML), and video editing require the application of similar mathematical operations on a large dataset. A GPU’s design allows it to perform the same operation on multiple data values in parallel. This increases its processing efficiency for many compute-intensive tasks.

Learn more

[View original](https://aws.amazon.com/what-is/gpu/?trk=faq_card)[2024-08-01](https://aws.amazon.com/what-is/enterprise-ai/?trk=faq_card)

#### What Is Enterprise AI?

Enterprise artificial intelligence (AI) is the adoption of advanced AI technologies within large organizations. Taking AI systems from prototype to production introduces several challenges around scale, performance, data governance, ethics, and regulatory compliance. Enterprise AI includes policies, strategies, infrastructure, and technologies for widespread AI use within a large organization. Even though it requires significant investment and effort, enterprise AI is important for large organizations as AI systems become more mainstream.

Learn more

[View original](https://aws.amazon.com/what-is/enterprise-ai/?trk=faq_card)[2022-05-25](https://aws.amazon.com/what-is/web-hosting/?trk=faq_card)

#### What is Web Hosting?

Web hosting is a service that stores your website or web application and makes it easily accessible across different devices such as desktop, mobile, and tablets. Any web application or website is typically made of many files, such as images, videos, text, and code, that you need to store on special computers called servers. The web hosting service provider maintains, configures, and runs physical servers that you can rent for your files. Website and web application hosting services also provide additional support, such as security, website backup, and website performance, which free up your time so that you can focus on the core functions of your website.

Learn more

[View original](https://aws.amazon.com/what-is/web-hosting/?trk=faq_card)

## Did you find what you were looking for today?

Let us know so we can improve the quality of the content on our pages