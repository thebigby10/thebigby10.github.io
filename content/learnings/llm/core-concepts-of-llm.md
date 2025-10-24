+++
date = '2025-10-19T19:56:48+06:00'
draft = true
title = 'Core Concepts of LLM'
+++

# Core Concepts of LLM

## What is LLM?

LLM is a language model that is trained on a large corpus of text data. It is a type of **artificial neural network** that can generate human-like text. LLMs are trained using machine learning algorithms to **predict the next word in a sequence of text based on the previous words**.

#### TLDR;

Basically llm just predicts what should be the next work based on the previous words(or contexts).

## Main concepts of LLMs

1. Neural network
2. Embeddings
3. Transformers & Attention Mechanism
4. Pre-training & Fine-tuning
5. Tokens
6. Qunantization

Let's explore each of these concepts one by one.

## Transformers

## Qunantization

## Neural Network



### Refrences

- [Neural Networks Explained in 5 minutes - IBM Technology](https://www.youtube.com/watch?v=jmmW0F0biz0)
- [I Built a Neural Network from Scratch - Green Code](https://www.youtube.com/watch?v=cAkMcPfY_Ns)

rough notes:

refernce to : neural-network-overview.md

how llm use neural network?

At their heart, LLMs are just extremely large and specialized neural networks.

The biggest difference is the architecture. Instead of the simple layered network above, LLMs use a more advanced architecture called a Transformer. The key innovation of the Transformer is a mechanism called self-attention.

Think of self-attention as the ability to understand context. When processing a sentence, the attention mechanism allows the model to look at all the other words in the sentence and figure out which ones are most important for understanding the current word.

For example, in the sentence:

    "The cat chased the mouse until it got tired."

The self-attention mechanism helps the LLM figure out that "it" refers to the "cat," not the "mouse." This ability to track relationships and context across long sequences of text is what makes Transformers so powerful.

LLMs are trained on a simple but massive task: predicting the next word. They are fed trillions of words from the internet, and after every word, they try to predict the next one. They then use the same loss calculation -> backpropagation -> weight update cycle we discussed, but on a colossal scale with billions of weights.

By doing nothing but learning to predict the next word, these massive Transformer networks develop an emergent and sophisticated understanding of grammar, facts, reasoning, and style.
