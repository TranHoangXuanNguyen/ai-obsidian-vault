---
url: "https://www.youtube.com/watch?v=_ZvnD73m40o"
channel: "freeCodeCamp.org"
tags:
  - "youtube"
  - "video"
---
![Thumbnail](https://www.youtube.com/img/desktop/yt_1200.png)

### Video description:
![](https://www.youtube.com/watch?v=_ZvnD73m40o)

Learn prompt engineering techniques to get better results from ChatGPT and other LLMs.  
  
✏️ Course developed by @aniakubow  
  
❤️ Support for this channel comes from our friends at Scrimba – the coding platform that's reinvented interactive learning: https://scrimba.com/freecodecamp  
  
⭐️ Contents ⭐️  
⌨️ (00:00) Introduction  
⌨️ (01:31) What is Prompt Engineering?  
⌨️ (02:17) Introduction to AI  
⌨️ (03:52) Why is Machine learning useful?  
⌨️ (06:36) Linguistics  
⌨️ (08:04) Language Models  
⌨️ (14:35) Prompt Engineering Mindset  
⌨️ (15:38) Using GPT-4  
⌨️ (20:41) Best practices  
⌨️ (31:20) Zero shot and few shot prompts  
⌨️ (35:06) AI hallucinations  
⌨️ (36:43) Vectors/text embeddings  
⌨️ (40:28) Recap  
  
🎉 Thanks to our Champion and Sponsor supporters:  
👾 davthecoder  
👾 jedi-or-sith  
👾 南宮千影  
👾 Agustín Kussrow  
👾 Nattira Maneerat  
👾 Heather Wcislo  
👾 Serhiy Kalinets  
👾 Justin Hual  
👾 Otis Morgan  
👾 Oscar Rahnama  
  
  
English  
This video has been dubbed using an artificial voice via https://aloud.area120.google.com to increase accessibility. You can change the audio track language in the Settings menu.  
  
Spanish  
Este video ha sido doblado al español con voz artificial con https://aloud.area120.google.com para aumentar la accesibilidad. Puede cambiar el idioma de la pista de audio en el menú Configuración.  
  
Portuguese  
Este vídeo foi dublado para o português usando uma voz artificial via https://aloud.area120.google.com para melhorar sua acessibilidade. Você pode alterar o idioma do áudio no menu Configurações.  
  
Hindi  
इस वीडियो को ज़्यादा लोगों तक पहुंचाने के लिए, इसे https://aloud.area120.google.com के ज़रिए एक आर्टिफ़िशियल वॉइस का इस्तेमाल करके डब किया गया है. सेटिंग्स मेनू में जाकर ऑडियो ट्रैक की भाषा बदली जा सकती है.  
  
(Hindi dubbed via Melt Labs - https://www.withmelt.com/)  
  
\--  
  
Learn to code for free and get a developer job: https://www.freecodecamp.org  
  
Read hundreds of articles on programming: https://freecodecamp.org/news

## Transcript

### Introduction

**0:00** · Learn how to get chat GPT and other LLMs to give you the perfect responses by mastering prompt engineering strategies.

**0:07** · Anu Kubo is one of our most popular instructors.

**0:10** · And in this course, she will teach you the latest techniques to maximize your productivity with large language models.

**0:17** · Hi everyone and welcome to this course on prompt engineering.

**0:21** · My name is Anu Kubo and I'm a software developer as well as course cruiser here on FreeCoCamp as well as on my own channel.

**0:28** · This is going to be a unique course for me as there is going to be a lot less coding going on but a lot more understanding about the topic of prompt engineering and why some companies are paying up to $335,000 a year according to Bloomberg for people in this profession.

**0:44** · And no, no coding background is necessarily required.

**0:48** · So what are we waiting for?

**0:50** · Let's do it.

**0:51** · In this course, we will learn what prompt engineering is exactly, get a brief introduction to AI, a look at large language models or LLMs such as chat GPT, a look at text to image models such as mid journey, a look at emerging models.

**1:07** · This would include text to speech, text to audio or speech to text as well as prompt engineering mindset, best practices, zero-shot prompting, few-shot prompting, chain of thought, AI hallucinations, vexes, text embeddings and also end with a quick intro to chat GPT.

**1:26** · So let's start off with looking at what exactly prompt engineering is in the first place.

### What is Prompt Engineering?

**1:31** · Prompt engineering in a nutshell is a career that came about of the back of the rise of artificial intelligence.

**1:38** · It involves human writing, refining and optimizing prompts in a structured way.

**1:43** · This is done with the intention of perfecting the interaction between humans and AI to the highest degree possible.

**1:49** · Not only that, however, a prompt engineer is then also required to continuously monitor those prompts ensure their effectiveness with time as AI progresses.

**1:59** · Maintaining an up-to-date prompt library will be a requirement that is placed onto the prompt engineer as well as reporting on findings and in general, being a thought leader in this space.

**2:09** · But why do we need it?

**2:11** · And how did it come about from AI?

**2:13** · Before moving on, let's actually make sure we are on the same page about what exactly AI is.

### Introduction to AI

**2:19** · Artificial intelligence is the simulation of human intelligence processes by machines.

**2:25** · I say simulation as artificial intelligence is not sentient, at least not yet anyways, meaning it cannot think for itself as much as it may seem it does.

**2:36** · Often, and this is certainly the case with tools such as chat GPT, for example, when we say AI, we are simply referring to a term called machine learning.

**2:46** · Machine learning works by using large amounts of training data that is then analyzed for correlations and patterns.

**2:53** · These patterns are then used to predict outcomes based on the training data provided.

**2:58** · So for example, here we are feeding data saying that if a paragraph looks like this with this type of title, then it should be categorized as international finance.

**3:09** · The second paragraph should be put in the category of earning reports and so on.

**3:14** · With some code, we should be able to train our AI model to correctly guess what future paragraphs are about.

**3:21** · And that's it.

**3:22** · Of course, that is a super basic example and we would need way more data than these five paragraphs right here, but you get the idea.

**3:30** · If you want to build your own AI model and understand the concept of machine learning better as a total beginner, please check out my video on it on my channel, Code with Anya Kubo.

**3:39** · As of now, rapidly improving general AI techniques can create realistic text responses and even images, music, and other media thanks to the huge amounts of training data and talented developers working on it today.

### Why is Machine learning useful?

**3:53** · Why is prompt engineering useful?

**3:56** · With the quick and exponential growing rise of AI, even the architects of it themselves struggle to control it and its outputs.

**4:04** · This might be a bit hard to understand, but think of it this way.

**4:07** · If you were to ask an AI chatbot what is four plus four, you would expect it to say eight, right?

**4:13** · The result of eight is pretty indisputable.

**4:16** · However, imagine you are a young student trying to learn the English language.

**4:21** · I'm going to show you just how different responses can be based on the prompts you feed and in turn your learning experience.

**4:29** · For this example, I'm going to be using Chat GPT's GPT-4 model.

**4:34** · So let's start with the basics.

**4:36** · If you were to type, correct my paragraph and then paste it a badly written paragraph.

**4:43** · So just like this, today was great in the world for me.

**4:45** · I went to a Disneyland with my mom.

**4:47** · It could have been better though if it wasn't raining.

**4:50** · Great, the young English learner has a better sentence, but it kind of stops there and the learner is just left to their own devices.

**4:57** · And honestly, the sentence really isn't that great anyway.

**5:02** · What if the learner could get the best sentences possible from a teacher who understands their interests to keep them engaged?

**5:10** · With the correct prompts, we can actually create that with AI.

**5:14** · So let's give it a go and let's write a prompt to do this.

**5:17** · So here's the prompt I'm going to give it.

**5:20** · I'm going to write, I want you to act as a spoken English teacher.

**5:24** · I will speak to you in English and you'll reply to me in English to practice my spoken English.

**5:30** · I want you to keep my reply neat, limiting the reply to 100 words.

**5:35** · I also want you to strictly correct my grammar mistakes and typos.

**5:39** · And I want you to ask me a question in your reply.

**5:43** · Now, let's start practicing.

**5:45** · You could ask me a question first.

**5:48** · Remember, I want you to strictly correct my grammar mistakes and typos.

**5:52** · So there's my prompt.

**5:54** · You can also go a step further and ask it to correct your factual errors too, which I think would be an excellent addition to the prompt that will benefit the young learner.

**6:03** · Okay, so let's go ahead and add that to the prompt.

**6:06** · Okay, and let us do its thing.

**6:09** · And great, so now this is way more interactive.

**6:13** · As you will see, it's asking you a question and telling you what to do and will provide you with corrections if needed.

**6:19** · So in a way, you're communicating with the AI.

**6:23** · It's giving you suggestions and you're learning along the way.

**6:26** · It's a completely different experience thanks to the prompt that we wrote.

**6:30** · Pretty cool, right?

**6:31** · We're gonna be diving into a bunch of these concepts soon, but first let's start with the basics.

### Linguistics

**6:37** · Linguistics.

**6:38** · Linguistics is the study of language.

**6:41** · It focuses on everything from phonetics, so the study of how speech sounds are produced and perceived.

**6:47** · Phonology, so the study of sound patterns and changes.

**6:51** · Morphology, the study of word structure.

**6:54** · Syntax, so the study of sentence structure.

**6:57** · Semantics, so the study of linguistic meaning.

**7:01** · Pragmatics, so in other words, the study of how language is used in context.

**7:05** · Historical linguistics, or the study of language change.

**7:09** · Sociolinguistics, or in other words, the study of the relation between language and society.

**7:16** · Computational linguistics, so the study of how computers can process human language.

**7:21** · And physiolinguistics, or the study of how humans acquire and use language.

**7:27** · So a lot.

**7:29** · Linguistics are the key to prompt engineering.

**7:32** · Why?

**7:33** · Understanding the nuances of language and how it is used in different contexts is crucial for crafting effective prompts.

**7:40** · Not only that, but knowing how to use a grammar or language structure that is universally used will result in the AI system returning back the most accurate results.

**7:50** · As you can imagine, the sheer amount of data that it is trained on is most likely to mostly use the standard grammar and language structure that is universally used.

**8:00** · So sticking to the standardization is key.

### Language Models

**8:04** · Language models.

**8:06** · Imagine a world where computers possess the power to understand and generate human language.

**8:11** · A world where machines can chat, write stories, and even compose poetry.

**8:16** · In this magical realm, language models can come into play.

**8:21** · They are like the wizards of the digital realm capable of understanding and creating human-like text.

**8:27** · A language model is a clever computer program that learns from a vast collection of written text.

**8:34** · It takes in books, articles, websites, and all sorts of written resources, allowing it to gather knowledge about how humans use language.

**8:42** · Just like a master linguist, it becomes an expert in the art of conversation, grammar, and style.

**8:48** · But how does this all work?

**8:50** · Well, imagine you feed a sentence.

**8:53** · The language model will then analyze the sentence, examine the order of words, their meanings, and the way they fit together.

**8:59** · Then the language model would generate a prediction or a continuation of the sentence that makes sense based on its understanding of the language.

**9:08** · It will weave words together one by one, creating a response that seems like it was crafted by a human being.

**9:15** · Imagine having a conversation with the language model as if you were exchanging ideas with a digital friend.

**9:20** · You ask a question, and it responds with a well-crafted answer.

**9:24** · You tell a joke, and it counters with a witty remark.

**9:27** · It's like having a language expert by your side always ready to assist and engage in conversation.

**9:33** · Now, you may wonder where these language models are used.

**9:36** · They can be found in various places, from your smartphone's virtual assistants to customer service chatbots, and even in the creative realm of writing.

**9:46** · They help us find information, offer suggestions, and create content.

**9:50** · But remember, while language models possess incredible abilities, they still rely on the human to create and train them.

**9:58** · They are, in fact, a fusion of human ingenuity and the power of algorithms, blending the best of both worlds.

**10:05** · Let's start off by looking at the history of language models, starting with the first AI, Eliza, back in the 60s.

**10:12** · Eliza is an early natural language processing computer program created from 1964 to 1966 at MIT by Joseph Wiesenbaum.

**10:22** · Eliza was designed to simulate a conversation with a human being.

**10:26** · Eliza had a special knack for mimicking a Rogerian psychotherapist, someone who essentially listens attentively and asks probing questions to help people explore their thoughts and feelings.

**10:37** · Eliza's secret weapon was its mastery of pattern matching.

**10:42** · It had a treasure trove of predefined patterns, each associated with specific responses.

**10:47** · These patterns were like magical spells that allowed Eliza to understand and respond to human language.

**10:54** · When you engage in a conversation with Eliza, it would carefully analyze your input, seeking patterns and keywords.

**11:00** · It would then transform your words into a series of symbols, searching for patterns that match those symbols in its repertoire.

**11:07** · Once a pattern was detected, Eliza would work its magic by transforming your words into a question or statement that aimed to explore your thoughts and emotions.

**11:17** · It was as if Eliza was holding up a metaphorical mirror, encouraging you to delve deeper into your own thinking.

**11:24** · For example, if you said something like, I feel sad, Eliza would detect the pattern and respond with a question like, why do you think you feel sad?

**11:33** · It encouraged reflection and introspection, just like a caring therapist would.

**11:39** · But here's the delightful twist.

**11:41** · Eliza didn't truly understand what you were saying.

**11:44** · It was just a clever illusion.

**11:46** · It used pattern matching and some creative programming tricks to create the illusion of understanding while in reality, it was just following a set of predefined rules.

**11:57** · Yet, even though Eliza was a simple program, people were often captivated by its conversational abilities.

**12:04** · They felt heard and understood, even if they knew they were talking to a machine.

**12:09** · It was like having a digital confident who was always ready to listen and offer gentle guidance.

**12:15** · Eliza's creator, Weisenbaum, intended the program as a method to explore communication between humans and machines.

**12:22** · He was surprised and shocked that individuals, including his secretary, attributed human-like feelings to the computer program.

**12:29** · But that is a whole other topic of conversation in itself.

**12:34** · Eliza's impact was profound, sparking interest and research in the field of natural language processing.

**12:39** · It paved the way for more advanced systems that could truly understand and generate human language.

**12:45** · It was the humble beginning of a grand adventure in the world of conversational AI.

**12:51** · Fast forward to the 1970s, when a program named Shudlu appeared.

**12:56** · It could understand simple commands and interact with a virtual world of blocks.

**13:00** · Although Shudlu wasn't a language model per se, it laid the foundation for the idea of machines comprehending human language.

**13:08** · But the true language models began around 2010, when the power of deep learning and neural networks came into play.

**13:16** · Enter the mighty GPT, short for generative pre-trained transformer, ready to conquer the world of language.

**13:24** · In the year 2018, the fast iteration of GPT emerged, created by the company OpenAI.

**13:31** · It was trained on a large amount of text data, absorbing knowledge from books, articles, and a large chunk of the internet.

**13:38** · GPT-1 was a taste of things to come, an impressive language model, but small compared to its descendants that we use today.

**13:46** · As time went on, the saga continued with the arrival of GPT-2 in 2019, followed by GPT-3 in 2020.

**13:54** · This was a titan among language models equipped with a large number of parameters, over 175 billion to be precise.

**14:02** · GPT-3 dazzled the world with its unparalleled ability to understand, respond, and even generate creative pieces of writing.

**14:09** · The arrival of GPT-3 marked a real turning point in terms of language models and AI.

**14:15** · At the time of writing, we now also have GPT-4, trained on pretty much the whole internet, rather than outdated large data sets, as well as BERT from Google and so much more.

**14:25** · It would seem we are only just at the start when it comes to language models and AI.

**14:30** · So learning how to harness this data with prompt engineering is a smart move for anyone today.

### Prompt Engineering Mindset

**14:36** · The prompt engineering mindset.

**14:38** · When thinking of good prompts, it is always best to get in the correct mindset.

**14:42** · Essentially, you want to just write one prompt, right?

**14:45** · And not have to waste time and tokens, writing lots of different prompts until you get the result you desire.

**14:52** · So essentially, kind of the same as when you Google stuff, right?

**14:56** · How good are your Googling skills now, as opposed to five years ago?

**15:00** · I'm assuming a lot better.

**15:02** · We have grown to intuitively know what to type into Google the first time round as to not waste time.

**15:09** · Having the same mindset for prompt engineering can also be applied.

**15:13** · Mahail Eric of the Infinite Machine Learning Podcast says it well when he says, I personally like the analogy of prompting to designing effective Google searches.

**15:23** · There are clearly better and worse ways to write queries against the Google search engine that solve your task.

**15:29** · This variance exists because of the opaqueness of what Google is doing under the hood.

**15:35** · We are gonna keep this in mind for the remainder of the course.

### Using GPT-4

**15:39** · A quick intro to using chat GPT by OpenAI.

**15:43** · So as I said in this course for the examples, I will be using chat GPT's GPT for model.

**15:51** · In order to follow along or just to understand how we are going to be using the platform, please head over to openai.com and just go ahead and sign up.

**16:03** · I've already signed up, so I'm just gonna go ahead and log in and that will take me to the platform in which I can choose what I want to interact with.

**16:13** · For this tutorial, we are going to be interacting with chat GPT for.

**16:19** · So please go ahead and click on here and that will take you to the platform.

**16:24** · And then I'm just gonna go ahead and switch to the GPT for model, which is the latest one.

**16:31** · Okay, so great.

**16:33** · You will see here all the previous chats that I've had.

**16:37** · I'm just going to minimize this.

**16:39** · And if we want to create a new chat, all we'd have to do is click the new chat button.

**16:44** · Okay, so here, for example, what I can do is just go ahead and ask any questions.

**16:51** · So what is four plus four?

**16:54** · And then hit send.

**16:55** · And that will essentially give me a response.

**16:58** · So I'm now interacting with chat GPT for.

**17:02** · On this occasion, I can actually build on the previous conversation.

**17:07** · So what I can do is say, great.

**17:11** · Now, can you add another five to that?

**17:19** · What is the answer?

**17:21** · And it will take into account everything that I have previously.

**17:25** · Okay, I am building on top of the knowledge that it already has.

**17:30** · Great.

**17:31** · So again, this is just a very quick introduction to how to use this, we will be doing a deeper dive into this throughout this course.

**17:41** · So once again, to create a new chat, all you'd have to do is create new chat.

**17:45** · And if you want to delete the old one, just go ahead and click that delete button.

**17:48** · And that will delete it.

**17:50** · And then a new chat is brought up automatically.

**17:53** · Wonderful.

**17:55** · Now you might have seen my course on open AI in which we can also use the API.

**18:02** · And to use the API, just go over to the API references.

**18:06** · And all you would have to do is get an API key.

**18:10** · And the API key can be viewed here.

**18:13** · And then you just go ahead and create an API key.

**18:16** · And that will allow you to interact with the open AI API in order for you to build out your own platforms just as the one we saw before.

**18:26** · So if you're interested in that, please do head over to my tutorial on this, again, on the free COCAM channel.

**18:33** · Otherwise, let's continue using chat GPT.

**18:38** · So once again, I'm just going to log in and head back to the platform here.

**18:43** · And that is it, we are ready to go.

**18:47** · Another thing I want to discuss is tokens.

**18:51** · As you might find that you have run out of the free tokens that you have in order to interact with chat GPT.

**18:58** · So in order to do that, I'm just going to show you this, I'm going to head over to the documentation and talk to you a little bit about tokens.

**19:09** · So GPT-4 essentially processes all texts in chunks called tokens.

**19:16** · And this token is approximately four characters or 0.75 words for English text.

**19:24** · And we essentially get charged by token.

**19:27** · If you want to know exactly how many tokens you are using, you can check it out here, you can check out the tokenizer tool, and it will give you a rough example.

**19:37** · So for example, I can say, what is four plus four.

**19:44** · And with that piece of text, the total count of tokens is going to be six.

**19:51** · Okay, so there we go.

**19:54** · That is exactly how many tokens will be used in order to produce a answer for this request.

**20:02** · Great, so here is a URL for that.

**20:04** · You can play around with it.

**20:06** · I hope you have fun.

**20:08** · If you want to see your usage, you can head over to account and then you can manage your account.

**20:14** · And this should be able to show you your usage.

**20:17** · So it will show you your usage right here per month.

**20:21** · And then you can, of course, also add billing in order to carry on using chat GPT in case you've used up all your tokens and you can't use it anymore.

**20:32** · So once again, this is under account billing overview.

**20:36** · So just go check it out.

**20:38** · Okay, and now back to the platform.

### Best practices

**20:42** · Best practices.

**20:44** · The biggest misconception when it comes to prompt engineering is that it's an easy job with no science to it.

**20:51** · I imagine a lot of people think it's just about constructing a one-off sentence such as correct my paragraph that we saw in the previous example.

**21:00** · When you start to look at it, creating effective prompts relies on a bunch of different factors.

**21:06** · Here are some things to consider when writing a good prompt.

**21:10** · Consider writing clear instructions with details in your query.

**21:14** · Consider adopting a persona as well as specifying the format using iterative prompting, meaning if you have a multi-part question or if the first response wasn't sufficient, you can continue by asking follow-up questions or asking the model to elaborate and avoid leading the answer.

**21:33** · Try not to make your prompts so leading that it inadvertently tells the model what answer you're expecting.

**21:39** · This might bias the response unduly.

**21:42** · And finally, limit the scope for long topics.

**21:45** · If you're asking about a broad topic, it's helpful to break it down or limit the scope to get a more focused answer.

**21:51** · Let's look at some of these now.

**21:53** · In order to write clearer instructions, we can adopt writing more details in our queries.

**21:59** · And to get the best results, don't assume the AI knows what you are talking about.

**22:04** · Writing something like, when is the election, implies that you are expecting the AI to know what election you are talking about and what country you mean.

**22:14** · This may result in you asking a few follow-up questions to finally get the result you want, resulting in time loss and frankly, perhaps some frustration.

**22:23** · Consider taking the time to write a prompt with clear instructions.

**22:27** · So, for example, instead of writing, when is the election, you could write, when is the next presidential election for Poland?

**22:36** · So let's go ahead and run this.

**22:39** · And this will be much more precise and knows exactly what we are asking about.

**22:44** · It's not gonna go guessing and waste our time as well as waste our resources.

**22:50** · So in other words, tokens that we are using, so in other words, money, in order to get the right answer the first time.

**22:57** · Here are some other examples of how you could write clearer prompts.

**23:01** · So for example, we have this prompt here, which says write code to filter out the ages from data.

**23:07** · And if you run it, you don't really know what language it's gonna come back with, let's see.

**23:12** · So for example, here it's using Python.

**23:15** · I actually didn't wanna use Python, okay?

**23:18** · So now we've lost some tokens asking this.

**23:21** · We've also lost some time and we just haven't got the right response.

**23:25** · This could have been so easily avoided.

**23:28** · So I'm gonna stop this from generating and let's try again.

**23:32** · So this time, let's be more specific by writing, write a JavaScript function that will take an array of objects and filter out the value of age property and put them in a new array.

**23:44** · Please explain what each code snippet does.

**23:47** · In this example, I am not assuming the AI knows what computer language I like to use and I am being more specific about what my data actually looks like.

**23:56** · On this occasion, it's an array of objects.

**23:59** · Not only that, I'm also asking the AI to explain why it's doing each step so that I in turn can understand and not just copy paste the code without gaining any knowledge from it.

**24:11** · Okay, so here you can see a live example of what's coming back to us from GPT-4.

**24:17** · It's given us the correct code.

**24:20** · So I have checked that and I was also giving us an example of how you would use the function, which is something I didn't ask, which is super useful.

**24:28** · It's kind of gone above and beyond for helping me out in understanding what is going on.

**24:35** · Let's look at another example.

**24:37** · We can write, tell me what this essay is about.

**24:41** · So I'm going to just type this and then just paste in an essay and hit go.

**24:46** · And then chat GPT will do its thing.

**24:49** · It's going to give me a summarization as it thinks best.

**24:53** · So on this occasion, it is essentially giving me numbered points about what this essay is about.

**25:00** · They're really long.

**25:01** · I really didn't want to read this much.

**25:03** · It's pretty much looking to be the same as the original essay.

**25:08** · So this is not something I wanted.

**25:11** · I should have been way more specific in telling it what I need.

**25:16** · So what I'm going to do is just add to this conversation.

**25:19** · So it's going to learn on what I wrote previously.

**25:22** · And I'm just going to specify to use bullet points to explain what this essay is about, making sure each point is no longer the 10 words long.

**25:30** · So I am being super specific in providing the instructions of what I want and let's hit go.

**25:39** · So now this is a lot shorter.

**25:40** · Okay, as you can see, each point is no longer than 10 words long.

**25:44** · And then I'm going to get a summary that is a bit longer and will give me a summary of the essay that I pasted in above.

**25:54** · So great, of course you can do this on any essay or piece of text that you wish and you can set your own clear and specific instructions as well.

**26:07** · Okay, so I hope you can see why the second one is better.

**26:11** · It's because I am not assuming the AI knows what kind of format I want the summarization of the essay to be in.

**26:17** · I am being specific that I want very short notes on the essay in bullet point format with a short conclusion at the end.

**26:25** · If I did not put this, the summary could have been just as long as the essay itself and the prompt could be considered useless in my eyes.

**26:34** · Next up, we can also adopt a persona.

**26:37** · When writing prompts, it is sometimes helpful to create a persona.

**26:40** · This means you're asking the AI to respond to you and a certain character.

**26:45** · So exactly like the English language teacher example we saw earlier, using a persona in prompt engineering can help ensure that the language model's output is relevant, useful and consistent with the needs and preferences of the target audience, making it a powerful tool for developing effective language models that meet the needs of users.

**27:05** · Let's look at some examples of adopting a persona.

**27:08** · So for example, you're gonna have this prompt right here.

**27:12** · Write a poem for a sister's high school graduation that will be read out to a family and close friends.

**27:19** · So let's go ahead and run this and let's see what comes back.

**27:24** · So there we go.

**27:25** · It is quite good in a room filled with kin and close ties.

**27:29** · We gathered to honor the mist in our eyes for a journey has ended another begun as our dear sister steps into the sun.

**27:36** · Okay, so it's coming out with a poem I can see here.

**27:41** · It is quite a good one, I guess, probably better than anything that I would have written.

**27:46** · And it is maybe a little bit generic.

**27:50** · Maybe that's what you wanted.

**27:52** · I think we can do better than this.

**27:54** · So let's try this.

**27:56** · This time I'm gonna write a prompt with a persona.

**28:00** · So this time I'm gonna specify who I'm writing as.

**28:03** · I'm gonna do write a poem as Helena.

**28:09** · Helena is 25 years old and an amazing writer.

**28:18** · Her writing style is similar to famous 21st century poet Rupi Kaur.

**28:29** · Writing as Helena, write a poem for her 18 year old sister to celebrate her sister's high school graduation.

**28:49** · High school graduation, this will be read out to friends and family at the gathering.

**29:06** · Okay, so let's check it out now.

**29:08** · We're writing as Helena, she's 25, she's an amazing writer and we've also assigned a writing style.

**29:17** · So let's check it out.

**29:19** · Now Chat GPT should be using anything it knows about Rupi Kaur, hopefully from the internet, in order to apply that style to this poem.

**29:29** · Okay, and as you can see, this is maybe a little bit more affectionate.

**29:34** · We've said sister, it's obviously a younger sister, so the words little sister are being used.

**29:39** · And in general, I think this is a much higher quality poem and if Helena truly does have the style of Rupi Kaur in writing, it will be almost indistinguishable who wrote this poem, Chat GPT or Helena.

**29:56** · So here we go, here's the full thing.

**29:58** · It starts off, in the garden of our youth, I watch you bloom from bud to blossom, from child to woman, 18 summers passed.

**30:06** · Again, utilizing the fact that we fed it, she was 18 and every winter's chill only made you stronger, a force of nature still.

**30:14** · So yes, in my eyes, this poem is a lot more better it's much more refined, it's much more personal, thanks to the prompts that we wrote.

**30:24** · We've already had a brief look at specifying format when we limited the word count of our bullet points in a previous example.

**30:33** · So that was a great example, limiting words is one that I use often.

**30:37** · However, we can do a bunch of other things, including specifying if something is a summary, a list or a detailed explanation.

**30:47** · Heck, you can even create checklists.

**30:49** · So I'm going to go ahead and show you how to do this.

**30:52** · Here is an example prompt and I'm just going to run it.

**30:56** · And there we go, we have created a checklist.

**31:00** · So many things you can do in Chat GPT.

**31:05** · Just make sure to specify the type of format you want and it should be able to do it.

**31:13** · Okay, great.

**31:14** · Now that we looked at some best practices, let's move on to some more advanced topics in the prompt engineering.

### Zero shot and few shot prompts

**31:21** · In this section, I'm going to talk about two types of prompting we can do, zero-shot prompting and few-shot prompting.

**31:28** · Zero-shot prompting leverages a pre-trained model's understanding of words and concept relationships without further training.

**31:36** · And few-shot prompting enhances the model with training examples via the prompt avoiding retraining.

**31:42** · So essentially in the context of the GPT-4 model, we don't really need to do much.

**31:48** · We are already using all of the data that it has in order to ask when is Christmas in America?

**31:53** · So let's go ahead and do some zero-shot prompting.

**31:57** · When is Christmas in America?

**32:03** · And here, go.

**32:05** · Okay, so it clearly already has the data for this.

**32:10** · We don't need to add any examples or anything like that.

**32:13** · So as you can see, zero-shot prompting refers to a way of querying models like GPT without any explicit training examples for the task at hand.

**32:25** · In the context of machine learning and not just GPT, zero-shot typically means that a model performs a task without having seen any examples of that task during its training.

**32:38** · Okay, great.

**32:40** · So now let's look at few-shot prompting.

**32:43** · So once again, with zero-shot prompting, we gave our language model a prompt and got a response.

**32:49** · But sometimes that's just not enough and we need a bit more training.

**32:54** · So let's use few-shot prompting and level up our language model by showing a few examples of the tasks we want it to perform.

**33:02** · So instead of zero examples, we give it a tiny bit of data.

**33:07** · So let's think, what would GPT for not know?

**33:12** · I guess it would not know my favorite types of food.

**33:16** · So for example, let's check, what is Ania's favorite type of food?

**33:26** · Plural, okay.

**33:28** · And I mean, it can guess, but no, it's just telling me that it doesn't know.

**33:34** · So that is absolutely fine, let's stop generating.

**33:38** · So now let's feed it in some example data.

**33:40** · I'm gonna feed it in a tiny bit of data.

**33:43** · Ania's favorite type of food includes, sorry about my English.

**33:54** · Let's go with burgers, fries, I love fries, pizza, and hit enter, okay?

**34:03** · So we are essentially giving chat GPT some information.

**34:09** · So now if I type what restaurant should I take Ania to in Dubai this weekend and hit here, it should hopefully understand that my favorite types of foods are burgers, fries, and pizza, and given that find me some restaurants in Dubai that I would like to go to.

**34:38** · So here are some, this has been updated as of September, 2021, but you know, these are pretty good ones.

**34:45** · So I would totally go to these.

**34:48** · This is a great example of few shop prompting in which it wouldn't have been able to answer this question if I hadn't had given it some example data or just trained the model a little bit more in order to get the response that I want.

**35:05** · Great, AI hallucinations.

### AI hallucinations

**35:09** · Now we're delving into something you probably never thought you'd hear in an AI context and that's hallucinations.

**35:16** · So what exactly are AI hallucinations?

**35:19** · And no, they're not when your AI assistants start seeing unicorns and rainbows.

**35:24** · It's actually a time that refers to the unusual outputs that AI models can produce when they misinterpret data.

**35:32** · A prime example of this is Google's Deep Dream.

**35:36** · You know, that project that turns pictures of your dog into a nightmarish blend of dog faces and well, more dog faces.

**35:44** · Deep Dream is an experiment that visualizes the patterns learned by a neural network.

**35:49** · It is built to over interpret and enhance the patterns it sees in an image, or in other words, fill in the gaps with images.

**35:58** · But some of the time those gaps can be filled with the wrong thing.

**36:02** · This is an example of an unusual output that AI models can produce when they misinterpret data.

**36:10** · Now, why do these hallucinations happen, you ask?

**36:13** · They're trained on a huge amount of data and they make sense of new data based on what they've seen before.

**36:20** · Sometimes, however, they make connections that are, let's call it creative.

**36:26** · And voila, an AI hallucination occurs.

**36:29** · Despite their funny results, AI hallucinations aren't just entertaining.

**36:34** · They're also quite enlightening.

**36:36** · They show us how our AI models interpret and understand data.

**36:40** · It's like a sneak peek into their thought processes.

### Vectors/text embeddings

**36:43** · This example is actually an AI image hallucination, as I thought it would be a fun one to show.

**36:49** · AI hallucinations can also happen with text models.

**36:52** · An example of this is us asking a text model about a historical figure and the text model not having an answer and hallucinating one instead, resulting in an inaccurate response.

**37:04** · Vectors and text embeddings.

**37:06** · To finish off, I'm going to leave you with a slightly more complex subject.

**37:11** · We're going to take a quick look at the topic of text embedding and vectors.

**37:15** · In computer science, particularly in the realm of machine learning and natural language processing or NLP, text embedding is a popular technique to represent textual information in a format that can be easily processed by algorithms, especially deep learning models.

**37:31** · In the context of prompt engineering, LLM embedding refers to representing prompts in a form that the model can understand and process.

**37:39** · This involves converting the text prompt into a high dimensional vector that captures its semantic information.

**37:46** · So essentially the word food is represented by this.

**37:49** · If using the create embedding API from open AI.

**37:53** · Okay, so you will see it's represented, the word was represented by an array of lots and lots of numbers.

**38:00** · But why do this?

**38:02** · Well, think about it this way.

**38:04** · If you ask a computer to come back with a similar word to food, you wouldn't really expect it to come back with burger or pizza, right?

**38:12** · That's what a human might do when thinking of similar words to food.

**38:16** · A computer would more likely look at the word lexicographically, kind of like when you scroll through a dictionary and come back with foot, for example.

**38:26** · This is kind of useless to us.

**38:28** · We wanna capture a word's semantic meaning.

**38:31** · So the meaning behind the word.

**38:34** · Text embeddings do essentially that, thanks to the data captured in this super long array.

**38:40** · Now, I can find words that are similar to food in a large corpus of text by comparing text embedding to text embedding and returning the most similar ones.

**38:51** · So words such as burger instead of foot will be more similar.

**38:56** · To create a text embedding of a word or even a whole sentence, check out the create embedding API here from OpenAI.

**39:05** · So here's the URL that you should visit and to create your own text embedding, you're gonna have to create a post request to this endpoint.

**39:15** · Okay, so that's what you can do.

**39:17** · You can also take the code from here.

**39:20** · So this is an example request written in Node.js and you would have to install the OpenAI package, take these two methods from it in order to pass through your OpenAI API key that I showed you how to get earlier.

**39:39** · As a refresher, you should go here and view API keys to create your own API key.

**39:45** · And once you pass that through, you can then use the configuration and pass it through here in order to use OpenAI and all of its wonderfulness, including the create embedding method in which you pass through an object.

**40:02** · That object has to include the model and it also is gonna include the input.

**40:07** · So in this case, it is the text that you want to turn into an embedding.

**40:13** · So this is the code for doing that.

**40:16** · And here is the response, which comes back as an object.

**40:21** · And then you would use dot notation to get the data, go into the array in order to get the embedding.

### Recap

**40:28** · So this is gonna be the embedding that we saw earlier.

**40:31** · It's an array made up of numbers and a lot of these numbers, okay?

**40:37** · So not just these three, this does spill out and this will be a very, very long array of numbers that will give you this semantic meaning of whatever text you pass through, okay?

**40:50** · So please have a go at playing around with this API in order to create your own text embeddings and compare them against other texts embeddings in order to find similar text.

**41:02** · And that's it.

**41:04** · Thank you so much for watching this course on prompt engineering in which we covered what it is.

**41:10** · We covered an introduction to AI as well as looked at linguistics, language models, prompt engineering mindset, using GPT-4, how to look at best practices as well as zero shot and few shot prompting, as well as AI hallucinations, vectors or texts embeddings and this recap right here.

**41:29** · So I hope you've enjoyed it and I'll see you again on the FreeCocam channel.