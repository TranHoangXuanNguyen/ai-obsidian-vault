---
title: "What is LLM? - Large Language Models Explained"
source: "https://aws.amazon.com/what-is/large-language-model/#how-do-large-language-models-work--1u0mds"
author:
published:
created: 2026-05-27
description: "Learn what Large Language Models are and why LLMs are essential. Discover its benefits and how you can use it to create new content and ideas including text, conversations, images, video, and audio."
tags:
  - "clippings"
---
## What is LLM (Large Language Model)?

[Create an AWS Account](https://portal.aws.amazon.com/gp/aws/developer/registration/index.html?pg=what_is_header)

## Page topics

## What are Large Language Models?

Large language models, also known as LLMs, are very large [deep learning](https://aws.amazon.com/what-is/deep-learning/) models that are pre-trained on vast amounts of data. The underlying transformer is a set of [neural networks](https://aws.amazon.com/what-is/neural-network/) that consist of an encoder and a decoder with self-attention capabilities. The encoder and decoder extract meanings from a sequence of text and understand the relationships between words and phrases in it.

Transformer LLMs are capable of unsupervised training, although a more precise explanation is that transformers perform self-learning. It is through this process that transformers learn to understand basic grammar, languages, and knowledge.

Unlike earlier recurrent neural networks (RNN) that sequentially process inputs, transformers process entire sequences in parallel. This allows the data scientists to use GPUs for training transformer-based LLMs, significantly reducing the training time.

Transformer neural network architecture allows the use of very large models, often with hundreds of billions of parameters. Such large-scale models can ingest massive amounts of data, often from the internet, but also from sources such as the [Common Crawl](https://registry.opendata.aws/commoncrawl/), which comprises more than 50 billion web pages, and Wikipedia, which has approximately 57 million pages.

[Read more about neural networks »](https://aws.amazon.com/what-is/neural-network/)

[Read more about deep learning »](https://aws.amazon.com/what-is/deep-learning/)

## Why are large language models important?

Large language models are incredibly flexible. One model can perform completely different tasks such as answering questions, summarizing documents, translating languages and completing sentences. LLMs have the potential to disrupt content creation and the way people use search engines and virtual assistants.

While not perfect, LLMs are demonstrating a remarkable ability to make predictions based on a relatively small number of prompts or inputs. LLMs can be used for [generative AI](https://aws.amazon.com/ai/generative-ai/) (artificial intelligence) to produce content based on input prompts in human language.

LLMs are big, very big. They can consider billions of parameters and have many possible uses. Here are some examples:

- Open AI's GPT-3 model has 175 billion parameters. Its cousin, ChatGPT, can identify patterns from data and generate natural and readable output. While we don’t know the size of Claude 2, it can take inputs up to 100K tokens in each prompt, which means it can work over hundreds of pages of technical documentation or even an entire book.
- AI21 Labs’ Jurassic-1 model has 178 billion parameters and a token vocabulary of 250,000-word parts and similar conversational capabilities.
- Cohere’s Command model has similar capabilities and can work in more than 100 different languages.
- LightOn's Paradigm offers foundation models with claimed capabilities that exceed those of GPT-3. All these LLMs come with APIs that allow developers to create unique generative AI applications.

[Read more about generative AI](https://aws.amazon.com/what-is/generative-ai/) [»](https://aws.amazon.com/what-is/generative-ai/)

[Read more about foundation models »](https://aws.amazon.com/what-is/foundation-models/)

## How do large language models work?

A key factor in how LLMs work is the way they represent words. Earlier forms of [machine learning](https://aws.amazon.com/what-is/machine-learning/) used a numerical table to represent each word. But, this form of representation could not recognize relationships between words such as words with similar meanings. This limitation was overcome by using multi-dimensional vectors, commonly referred to as word embeddings, to represent words so that words with similar contextual meanings or other relationships are close to each other in the vector space.

Using word embeddings, transformers can pre-process text as numerical representations through the encoder and understand the context of words and phrases with similar meanings as well as other relationships between words such as parts of speech. It is then possible for LLMs to apply this knowledge of the language through the decoder to produce a unique output.

## What are applications of large language models?

There are many practical applications for LLMs.

### Copywriting

Apart from GPT-3 and ChatGPT, Claude, Llama 2, Cohere Command, and Jurassiccan write original copy. AI21 Wordspice suggests changes to original sentences to improve style and voice.

### Knowledge base answering

Often referred to as knowledge-intensive natural language processing (KI-NLP), the technique refers to LLMs that can answer specific questions from information help in digital archives. An example is the ability of AI21 Studio playground to answer general knowledge questions.

### Text classification

Using clustering, LLMs can classify text with similar meanings or sentiments. Uses include measuring customer sentiment, determining the relationship between texts, and document search.

### Code generation

LLM are proficient in code generation from natural language prompts. Examples include [Amazon CodeWhisperer](https://aws.amazon.com/q/developer/) and Open AI's codex used in GitHub Copilot, which can code in Python, JavaScript, Ruby and several other programming languages. Other coding applications include creating SQL queries, writing shell commands and website design. [Learn more about AI code generation](https://aws.amazon.com/what-is/ai-coding/).

### Text generation

Similar to code generation, text generation can complete incomplete sentences, write product documentation or, like Alexa Create, write a short children's story.

## How are large language models trained?

Transformer-based neural networks are very large. These networks contain multiple nodes and layers. Each node in a layer has connections to all nodes in the subsequent layer, each of which has a weight and a bias. Weights and biases along with embeddings are known as model parameters. Large transformer-based neural networks can have billions and billions of parameters. The size of the model is generally determined by an empirical relationship between the model size, the number of parameters, and the size of the training data.

Training is performed using a large corpus of high-quality data. During training, the model iteratively adjusts parameter values until the model correctly predicts the next token from an the previous squence of input tokens. It does this through self-learning techniques which teach the model to adjust parameters to maximize the likelihood of the next tokens in the training examples.

Once trained, LLMs can be readily adapted to perform multiple tasks using relatively small sets of supervised data, a process known as fine tuning.

Three common learning models exist:

- Zero-shot learning; Base LLMs can respond to a broad range of requests without explicit training, often through prompts, although answer accuracy varies.
- Few-shot learning: By providing a few relevant training examples, base model performance significantly improves in that specific area.
- Fine-tuning: This is an extension of few-shot learning in that data scientists train a base model to adjust its parameters with additional data relevant to the specific application.

## What is the future of LLMs?

The introduction of large language models like ChatGPT, Claude 2, and Llama 2 that can answer questions and generate text points to exciting possibilities in the future. Slowly, but surely, LLMs are moving closer to human-like performance. The immediate success of these LLMs demonstrates a keen interest in robotic-type LLMs that emulate and, in some contexts, outperform the human brain. Here are some thoughts on the future of LLMs,

### Increased capabilities

As impressive as they are, the current level of technology is not perfect and LLMs are not infallible. However, newer releases will have improved accuracy and enhanced capabilities as developers learn how to improve their performance while reducing bias and eliminating incorrect answers.

### Audiovisual training

While developers train most LLMs using text, some have started training models using video and audio input. This form of training should lead to faster model development and open up new possibilities in terms of using LLMs for autonomous vehicles.

### Workplace transformation

LLMs are a disruptive factor that will change the workplace. LLMs will likely reduce monotonous and repetitive tasks in the same way that robots did for repetitive manufacturing tasks. Possibilities include repetitive clerical tasks, customer service [chatbots](https://aws.amazon.com/what-is/chatbot/), and simple automated copywriting.

### Conversational AI

LLMs will undoubtedly improve the performance of automated virtual assistants like Alexa, Google Assistant, and Siri. They will be better able to interpret user intent and respond to sophisticated commands.

[Read more about conversational AI](https://aws.amazon.com/what-is/conversational-ai/)

## How can AWS help with LLMs?

AWS offers several possibilities for large language model developers. [Amazon Bedrock](https://aws.amazon.com/bedrock/) is the easiest way to build and scale [generative AI](https://aws.amazon.com/ai/generative-ai/) applications with LLMs. Amazon Bedrock is a fully managed service that makes LLMs from Amazon and leading AI startups available through an API, so you can choose from various LLMs to find the model that's best suited for your use case.

Amazon SageMaker JumpStart is a machine learning hub with foundation models, built-in algorithms, and prebuilt ML solutions that you can deploy with just a few clicks With SageMaker JumpStart, you can access pretrained models, including foundation models, to perform tasks like article summarization and image generation. Pretrained models are fully customizable for your use case with your data, and you can easily deploy them into production with the user interface or SDK.

Get started with LLMs and AI on AWS by [creating a free account today](https://portal.aws.amazon.com/gp/aws/developer/registration/index.html).

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