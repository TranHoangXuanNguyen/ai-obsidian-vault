---
source: https://www.promptingguide.ai/techniques/dsp
author:
published:
tags:
  - clipping
  - article
  - prompt-engineering
  - prompt-technique
---
# Prompt Engineering Guide

[Prompting Techniques](https://www.promptingguide.ai/techniques)

Directional Stimulus Prompting

## Directional Stimulus Prompting

[Li et al., (2023) (opens in a new tab)](https://arxiv.org/abs/2302.11520) proposes a new prompting technique to better guide the LLM in generating the desired summary.

A tuneable policy LM is trained to generate the stimulus/hint. Seeing more use of RL to optimize LLMs.

The figure below shows how Directional Stimulus Prompting compares with standard prompting. The policy LM can be small and optimized to generate the hints that guide a black-box frozen LLM.

![DSP](https://www.promptingguide.ai/_next/image?url=%2F_next%2Fstatic%2Fmedia%2Fdsp.27a0005f.jpeg&w=3840&q=75)

Image Source: [Li et al., (2023) (opens in a new tab)](https://arxiv.org/abs/2302.11520)

Full example coming soon!

## Related Learning

Course

### [Prompt Engineering for LLMs](https://academy.dair.ai/courses/introduction-prompt-engineering)

Master directional stimulus prompting and advanced techniques for guiding LLM outputs.

Beginner

2 hours

Course

### [Building Effective AI Agents](https://academy.dair.ai/courses/building-effective-ai-agents)

Learn to build effective AI agents. Covers function calling, tool integration, and debugging agentic systems.

Intermediate

5 hours

### Explore All Courses

Discover our full catalog of AI and prompt engineering courses. From beginners to advanced practitioners.

Use code `PROMPTING20` for 20% off!

[Browse Academy](https://academy.dair.ai/)

Last updated on Mon Feb 02 2026

Sponsored by

[Active-Prompt](https://www.promptingguide.ai/techniques/activeprompt "Active-Prompt") [Program-Aided Language Models](https://www.promptingguide.ai/techniques/pal "Program-Aided Language Models")