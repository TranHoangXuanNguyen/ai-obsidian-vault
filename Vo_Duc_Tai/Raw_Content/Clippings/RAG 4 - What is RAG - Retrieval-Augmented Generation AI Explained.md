---
source: "https://aws.amazon.com/what-is/retrieval-augmented-generation/"
author:
published:
tags:
  - "clipping"
  - "article"
  - "news"
---
# What is RAG? - Retrieval-Augmented Generation AI Explained

## What is RAG (Retrieval-Augmented Generation)?

[Create an AWS Account](https://portal.aws.amazon.com/gp/aws/developer/registration/index.html?pg=what_is_header)

## Page topics

## What is Retrieval-Augmented Generation?

Retrieval-Augmented Generation (RAG) is the process of optimizing the output of a large language model, so it references an authoritative knowledge base outside of its training data sources before generating a response. Large Language Models (LLMs) are trained on vast volumes of data and use billions of parameters to generate original output for tasks like answering questions, translating languages, and completing sentences. RAG extends the already powerful capabilities of LLMs to specific domains or an organization's internal knowledge base, all without the need to retrain the model. It is a cost-effective approach to improving LLM output so it remains relevant, accurate, and useful in various contexts.

## Why is Retrieval-Augmented Generation important?

LLMs are a key [artificial intelligence (AI)](https://aws.amazon.com/what-is/artificial-intelligence/) technology powering intelligent [chatbots](https://aws.amazon.com/what-is/chatbot/) and other [natural language processing (NLP)](https://aws.amazon.com/what-is/nlp/) applications. The goal is to create bots that can answer user questions in various contexts by cross-referencing authoritative knowledge sources. Unfortunately, the nature of LLM technology introduces unpredictability in LLM responses. Additionally, LLM training data is static and introduces a cut-off date on the knowledge it has.

Known challenges of LLMs include:

- Presenting false information when it does not have the answer.
- Presenting out-of-date or generic information when the user expects a specific, current response.
- Creating a response from non-authoritative sources.
- Creating inaccurate responses due to terminology confusion, wherein different training sources use the same terminology to talk about different things.

You can think of the [Large Language Model](https://aws.amazon.com/what-is/large-language-model/) as an over-enthusiastic new employee who refuses to stay informed with current events but will always answer every question with absolute confidence. Unfortunately, such an attitude can negatively impact user trust and is not something you want your chatbots to emulate!

RAG is one approach to solving some of these challenges. It redirects the LLM to retrieve relevant information from authoritative, pre-determined knowledge sources. Organizations have greater control over the generated text output, and users gain insights into how the LLM generates the response.

## What are the benefits of Retrieval-Augmented Generation?

RAG technology brings several benefits to an organization's [generative AI](https://aws.amazon.com/what-is/generative-ai/) efforts.

### Cost-effective implementation

Chatbot development typically begins using a [foundation model](https://aws.amazon.com/what-is/foundation-models/). Foundation models (FMs) are API-accessible LLMs trained on a broad spectrum of generalized and unlabeled data. The computational and financial costs of retraining FMs for organization or domain-specific information are high. RAG is a more cost-effective approach to introducing new data to the LLM. It makes generative artificial intelligence (generative AI) technology more broadly accessible and usable.

### Current information

Even if the original training data sources for an LLM are suitable for your needs, it is challenging to maintain relevancy. RAG allows developers to provide the latest research, statistics, or news to the generative models. They can use RAG to connect the LLM directly to live social media feeds, news sites, or other frequently-updated information sources. The LLM can then provide the latest information to the users.

### Enhanced user trust

RAG allows the LLM to present accurate information with source attribution. The output can include citations or references to sources. Users can also look up source documents themselves if they require further clarification or more detail. This can increase trust and confidence in your generative AI solution.

### More developer control

With RAG, developers can test and improve their chat applications more efficiently. They can control and change the LLM's information sources to adapt to changing requirements or cross-functional usage. Developers can also restrict sensitive information retrieval to different authorization levels and ensure the LLM generates appropriate responses. In addition, they can also troubleshoot and make fixes if the LLM references incorrect information sources for specific questions. Organizations can implement generative AI technology more confidently for a broader range of applications.

## How does Retrieval-Augmented Generation work?

Without RAG, the LLM takes the user input and creates a response based on information it was trained on—or what it already knows. With RAG, an information retrieval component is introduced that utilizes the user input to first pull information from a new data source. The user query and the relevant information are both given to the LLM. The LLM uses the new knowledge and its training data to create better responses. The following sections provide an overview of the process.

### Create external data

The new data outside of the LLM's original training data set is called *external data*. It can come from multiple data sources, such as a APIs, databases, or document repositories. The data may exist in various formats like files, database records, or long-form text. Another AI technique, called *embedding language models*, converts data into numerical representations and stores it in a vector database. This process creates a knowledge library that the generative AI models can understand.

### Retrieve relevant information

The next step is to perform a relevancy search. The user query is converted to a vector representation and matched with the vector databases. For example, consider a smart chatbot that can answer human resource questions for an organization. If an employee searches, *"How much annual leave do I have?"* the system will retrieve annual leave policy documents alongside the individual employee's past leave record. These specific documents will be returned because they are highly-relevant to what the employee has input. The relevancy was calculated and established using mathematical vector calculations and representations.

### Augment the LLM prompt

Next, the RAG model augments the user input (or prompts) by adding the relevant retrieved data in context. This step uses prompt engineering techniques to communicate effectively with the LLM. The augmented prompt allows the large language models to generate an accurate answer to user queries.

### Update external data

The next question may be—what if the external data becomes stale? To maintain current information for retrieval, asynchronously update the documents and update embedding representation of the documents. You can do this through automated real-time processes or periodic batch processing. This is a common challenge in data analytics—different data-science approaches to change management can be used.

The following diagram shows the conceptual flow of using RAG with LLMs.

![](https://docs.aws.amazon.com/images/sagemaker/latest/dg/images/jumpstart/jumpstart-fm-rag.jpg)

## How can AWS support your Retrieval-Augmented Generation requirements?

[Amazon Bedrock](https://aws.amazon.com/bedrock/) is a fully-managed service that offers a choice of high-performing foundation models—along with a broad set of capabilities—to build generative AI applications while simplifying development and maintaining privacy and security. With knowledge bases for Amazon Bedrock, you can connect FMs to your data sources for RAG in just a few clicks. Vector conversions, retrievals, and improved output generation are all handled automatically.

For organizations managing their own RAG, [Amazon Kendra](https://aws.amazon.com/kendra/) is a highly-accurate enterprise search service powered by machine learning. It provides an optimized Kendra [Retrieve API](https://docs.aws.amazon.com/kendra/latest/APIReference/API_Retrieve.html) that you can use with Amazon Kendra’s high-accuracy semantic ranker as an enterprise retriever for your RAG workflows. For example, with the Retrieve API, you can:

- Retrieve up to 100 semantically-relevant passages of up to 200 token words each, ordered by relevance.
- Use pre-built connectors to popular data technologies like [Amazon Simple Storage Service](https://aws.amazon.com/s3/), SharePoint, Confluence, and other websites.
- Support a wide range of document formats such as HTML, Word, PowerPoint, PDF, Excel, and text files.
- Filter responses based on those documents that the end-user permissions allow.

Amazon also offers options for organizations who want to build more custom generative AI solutions. [Amazon SageMaker JumpStart](https://aws.amazon.com/sagemaker/jumpstart/) is a ML hub with FMs, built-in algorithms, and prebuilt ML solutions that you can deploy with just a few clicks. You can speed up RAG implementation by referring to existing SageMaker notebooks and code examples.

Get started with Retrieval-Augmented Generation on AWS by [creating a free account today](https://portal.aws.amazon.com/billing/signup)

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