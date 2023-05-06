# NaLLM: _Not a Large Language Model_

## Small is the new big

In recent years, Large Language Models such as [ChatGPT](https://chat.openai.com) or [Open Assistant](https://open-assistant.io) played a very large role in the world of AI and they literally changed the world for better but they also brought new problems to the scene as well! The main problem with ChatGPT is that _it's not open source_ and the main problem with the open source ones is that they need huge amount of money and resources in order to be self-hosted. So what is our possible solution?

The solution is to get back to the old ways of making a question-answering chatbot, but instead of making them on a limited knowledge base, use ChatGPT and other sources in order to make the answers more _humanized_. For this particular purpose we can use _Tensorflow_ and even better we can use [neuralintents](https://github.com/neuralnine/neuralintents) library which is written on top of tensorflow for making intelligent chatbots.

## It's _almost_ limitless

### No GPU is needed.

The main _bottleneck_ of most of modern AI models is the GPU. Specially since most of these models are tuned to work on GPU's with CUDA support, if you don't own an NVIDIA system, you basically have no chance to test most of the brand new models. On the other hand, GPU's are quiet expensive. So using _NaLLM_ requires no GPU's and it can even be running on a Raspberry Pi with only 2 GB of RAM.

### No big data is needed.

In order to train LLM's you usually need tons of tokens. For example _Large Language Model Meta AI_ or _LLaMa_ has been trained on one trillion tokens. Even crawling this amount of data from the internet is impossible for individuals and requires hundreds (if not thousands) of servers. It may also need a lot of data cleanup, duplication removal, etc. 

For using NaLLM, you only need to _make variations_ on your own knowledge base which is not a hard thing to do. The main task is to answer the questions in a way you think you're not faced by a machine and NaLLM does it well!

### No languages left behind!

That's it. You can train _NaLLM_ on every language supported by today's computers. It doesn't matter if it's English, German, Persian, Kurdish or Swahili! You just need to follow instructions in order to create a dataset and work with the architectures and models.

![NLLB](./nallm.png)

## Using ChatGPT to create a _large enough_ dataset.

As told you earlier, we still can utilize LLM's in our way. For this particular project we have this scenario:

1. Explain the procedure to ChatGPT (depending on the circumstances, it can be different AI like OpenAssistant or GPT-3)
2. Give our desired topics to the LLM and ask for _a question-answer pair_
3. Ask the LLM to add variations. For example we can tell it _ask the question in 10 or 20 other ways_ and _re-write the answer in 15 other ways_. 
4. We can ask it to JSON format the data for us.

### Procedure explanation

_NOTE: it may be changed in the future_