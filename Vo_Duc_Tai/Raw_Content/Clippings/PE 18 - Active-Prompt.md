---
source: https://www.promptingguide.ai/techniques/activeprompt
author:
published:
tags:
  - clipping
  - article
  - prompt-engineering
  - prompt-technique
---
# Prompt Engineering Guide

Active-Prompt

## Active-Prompt

Chain-of-thought (CoT) methods rely on a fixed set of human-annotated exemplars. The problem with this is that the exemplars might not be the most effective examples for the different tasks. To address this, [Diao et al., (2023) (opens in a new tab)](https://arxiv.org/pdf/2302.12246.pdf) recently proposed a new prompting approach called Active-Prompt to adapt LLMs to different task-specific example prompts (annotated with human-designed CoT reasoning).

Below is an illustration of the approach. The first step is to query the LLM with or without a few CoT examples. *k* possible answers are generated for a set of training questions. An uncertainty metric is calculated based on the *k* answers (disagreement used). The most uncertain questions are selected for annotation by humans. The new annotated exemplars are then used to infer each question.

![ACTIVE](https://www.promptingguide.ai/_next/image?url=%2F_next%2Fstatic%2Fmedia%2Factive-prompt.f739657b.png&w=3840&q=75)

Image Source: [Diao et al., (2023) (opens in a new tab)](https://arxiv.org/pdf/2302.12246.pdf)

### Explore All Courses

Discover our full catalog of AI and prompt engineering courses. From beginners to advanced practitioners.

Use code `PROMPTING20` for 20% off!

[Browse Academy](https://academy.dair.ai/)

Last updated on Mon Feb 02 2026

Sponsored by