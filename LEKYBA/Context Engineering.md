# Definition
Context engineering is the practice of deliberating designing, structuring and optimizing the context provided to LLMs to produce more accurate, relevant and reliable output.
It encompasses two techniques: Prompt Engineering and RAG.

----
# What is context in ML?
In modern ML systems, context is everything the model sees at inference time.
It might include: The system prompt, the user's query, any other provided data.

----
# Why it is important?
Context engineering can lead to better reasoning, tool calls and answers.
As a result, the quality and structure of [[Context window]] directly influence the model reasoning, tool use and outputs.

From studies on needle-in-a-haystack style benchmarking of Anthropic, they uncovered the concept of **context rot**: as the number of tokens in the context window increase, the ability of the model in accurate recalling information from that context decreases. 

[Reference](https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents)

----
# What are the key steps?
1. **Context selection:** choose what information to include in the context.
2. **Context structuring**
3. **Prompt design and Engineering:** frame instruction, include the constraint and rules and any requirements for the output formatting.
4. **Context compression:** fit more useful information into limited token space.
5. **Context sequencing:** Ordering matter for LLM. Should include instruction and rule first. The order should be the most relevant from top to bottom.
6. **Tool and memory integration:** 