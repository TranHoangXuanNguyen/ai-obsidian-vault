---
source: "https://www.promptingguide.ai/research/rag_hallucinations"
author:
published:
tags:
  - "clipping"
  - "article"
  - "news"
---
# Prompt Engineering Guide

## Reducing Hallucination in Structured Outputs via RAG

![](https://www.youtube.com/watch?v=TUL5guqZejw)

Researchers at ServiceNow shared a [new paper](https://arxiv.org/abs/2404.08189) where they discuss how to deploy an efficient RAG system for structured output tasks.

!["RAG Hallucination"](https://www.promptingguide.ai/_next/image?url=%2F_next%2Fstatic%2Fmedia%2Fstructured_outputs.d719e97d.png&w=1920&q=75)

The RAG system combines a small language model with a very small retriever. It shows that RAG can enable deploying powerful LLM-powered systems in limited-resource settings while mitigating issues like hallucination and increasing the reliability of outputs.

The paper covers the very useful enterprise application of translating natural language requirements to workflows (formatted in JSON). So much productivity can come from this task but there is a lot of optimization that can be further achieved (eg., using speculative decoding or using YAML instead of JSON).

The paper provides some great insights and practical tips on how to effectively develop RAG systems for the real world.

Last updated on Mon Dec 29 2025

Sponsored by