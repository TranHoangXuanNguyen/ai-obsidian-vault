---
url: "https://www.youtube.com/watch?v=T-D1OfcDW1M"
channel: "IBM Technology"
tags:
  - "youtube"
  - "video"
---
![Thumbnail](https://www.youtube.com/img/desktop/yt_1200.png)

### Video description:
![](https://www.youtube.com/watch?v=T-D1OfcDW1M)

Ready to become a certified GenAI engineer? Register now and use code IBMTechYT20 for 20% off of your exam → https://ibm.biz/BdGhCF  
Learn about the technology → https://ibm.biz/BdMsRT  
  
Large language models usually give great answers, but because they're limited to the training data used to create the model. Over time they can become incomplete--or worse, generate answers that are just plain wrong. One way of improving the LLM results is called "retrieval-augmented generation" or RAG. In this video, IBM Senior Research Scientist Marina Danilevsky explains the LLM/RAG framework and how this combination delivers two big advantages, namely: the model gets the most up-to-date and trustworthy facts, and you can see where the model got its info, lending more credibility to what it generates.  
  
Get weekly AI, cloud, security and sustainability industry news, events and insights. → https://ibm.biz/BdK6UY

## Transcript

### Introduction

**0:00** · Large language models. They are everywhere.

**0:02** · They get some things amazingly right and other things very interestingly wrong.

**0:07** · My name is Marina Danilevsky.

**0:09** · I am a Senior Research Scientist here at IBM Research.

**0:12** · And I want to tell you about a framework to help large language models be more accurate and more up to date: Retrieval-Augmented Generation, or RAG.

### What is RAG

**0:22** · Let's just talk about the "Generation" part for a minute.

**0:24** · So forget the "Retrieval-Augmented".

**0:26** · So the generation, this refers to large language models, or LLMs, that generate text in response to a user query, referred to as a prompt.

**0:36** · These models can have some undesirable behavior.

**0:38** · I want to tell you an anecdote to illustrate this.

**0:41** · So my kids, they recently asked me this question: "In our solar system, what planet has the most moons?"

### An anecdote

**0:48** · And my response was, “Oh, that's really great that you're asking this question. I loved space when I was your age.”

**0:55** · Of course, that was like 30 years ago.

**0:58** · But I know this! I read an article and the article said that it was Jupiter and 88 moons. So that's the answer.

**1:06** · Now, actually, there's a couple of things wrong with my answer.

**1:10** · First of all, I have no source to support what I'm saying.

**1:14** · So even though I confidently said “I read an article, I know the answer!”, I'm not sourcing it.

**1:18** · I'm giving the answer off the top of my head.

**1:20** · And also, I actually haven't kept up with this for awhile, and my answer is out of date.

### Two problems

**1:26** · So we have two problems here. One is no source. And the second problem is that I am out of date.

**1:35** · And these, in fact, are two behaviors that are often observed as problematic when interacting with large language models. They’re LLM challenges.

**1:46** · Now, what would have happened if I'd taken a beat and first gone and looked up the answer on a reputable source like NASA?

**1:55** · Well, then I would have been able to say, “Ah, okay! So the answer is Saturn with 146 moons.”

**2:03** · And in fact, this keeps changing because scientists keep on discovering more and more moons.

**2:08** · So I have now grounded my answer in something more believable.

**2:11** · I have not hallucinated or made up an answer.

**2:13** · Oh, by the way, I didn't leak personal information about how long ago it's been since I was obsessed with space.

### Large language models

**2:18** · All right, so what does this have to do with large language models?

**2:22** · Well, how would a large language model have answered this question?

**2:26** · So let's say that I have a user asking this question about moons.

**2:31** · A large language model would confidently say, OK, I have been trained and from what I know in my parameters during my training, the answer is Jupiter.

**2:46** · The answer is wrong. But, you know, we don't know.

**2:50** · The large language model is very confident in what it answered.

**2:52** · Now, what happens when you add this retrieval augmented part here?

**2:57** · What does that mean?

**2:59** · That means that now, instead of just relying on what the LLM knows, we are adding a content store.

**3:05** · This could be open like the internet.

**3:07** · This can be closed like some collection of documents, collection of policies, whatever.

**3:14** · The point, though, now is that the LLM first goes and talks to the content store and says, “Hey, can you retrieve for me information that is relevant to what the user's query was?”

**3:25** · And now, with this retrieval-augmented answer, it's not Jupiter anymore.

**3:31** · We know that it is Saturn. What does this look like?

**3:35** · Well, first user prompts the LLM with their question.

**3:46** · They say, this is what my question was.

**3:48** · And originally, if we're just talking to a generative model, the generative model says, “Oh, okay, I know the response. Here it is. Here's my response.”

**3:57** · But now in the RAG framework, the generative model actually has an instruction that says, "No, no, no."

**4:04** · "First, go and retrieve relevant content."

**4:08** · "Combine that with the user's question and only then generate the answer."

**4:13** · So the prompt now has three parts: the instruction to pay attention to, the retrieved content, together with the user's question.

### How does RAG help

**4:23** · Now give a response. And in fact, now you can give evidence for why your response was what it was.

**4:30** · So now hopefully you can see, how does RAG help the two LLM challenges that I had mentioned before?

**4:35** · So first of all, I'll start with the out of date part.

**4:38** · Now, instead of having to retrain your model, if new information comes up, like, hey, we found some more moons-- now to Jupiter again, maybe it'll be Saturn again in the future.

**4:48** · All you have to do is you augment your data store with new information, update information.

**4:53** · So now the next time that a user comes and asks the question, we're ready.

**4:57** · We just go ahead and retrieve the most up to date information.

**5:00** · The second problem, source.

**5:02** · Well, the large language model is now being instructed to pay attention to primary source data before giving its response.

**5:10** · And in fact, now being able to give evidence.

**5:13** · This makes it less likely to hallucinate or to leak data because it is less likely to rely only on information that it learned during training.

**5:21** · It also allows us to get the model to have a behavior that can be very positive, which is knowing when to say, “I don't know.”

**5:29** · If the user's question cannot be reliably answered based on your data store, the model should say, "I don't know," instead of making up something that is believable and may mislead the user.

**5:41** · This can have a negative effect as well though, because if the retriever is not sufficiently good to give the large language model the best, most high-quality grounding information, then maybe the user's query that is answerable doesn't get an answer.

**5:57** · So this is actually why lots of folks, including many of us here at IBM, are working the problem on both sides.

**6:03** · We are both working to improve the retriever to give the large language model the best quality data on which to ground its response, and also the generative part so that the LLM can give the richest, best response finally to the user when it generates the answer.

**6:21** · Thank you for learning more about RAG and like and subscribe to the channel.

**6:25** · Thank you.