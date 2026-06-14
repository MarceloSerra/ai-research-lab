# Prompt Engineering

## What is it?
Prompt engineering is the practice of designing effective inputs (prompts) for Large Language Models to get desired outputs. It's the primary way to control LLM behavior without modifying the model itself.

## Why does it exist?
LLMs are sensitive to how questions are asked:
- Same model, different prompt → dramatically different results
- Poor prompts produce generic, inaccurate responses
- Good prompts unlock reasoning, creativity, and precision
- Prompt design is often faster than model fine-tuning for new tasks

## Core Techniques

| Technique | Description | Example |
|-----------|-------------|---------|
| Zero-shot | Direct instruction without examples | "Classify this text as positive or negative" |
| Few-shot | Provide examples in prompt | "Happy → positive. Sad → negative. Great day → ?" |
| Chain-of-Thought | Ask model to reason step-by-step | "Think through this problem step by step" |
| Role Prompting | Assign a role/persona | "You are an expert physicist explaining concepts simply" |
| Structured Output | Specify output format | "Return JSON with fields: answer, confidence, reasoning" |

## When should I use it?
- First approach for any LLM task — before fine-tuning
- Rapid prototyping of language applications
- Tasks where prompt flexibility matters more than consistency
- Exploring whether an LLM can solve a problem at all

## When should I NOT use it?
- Consistent behavior across many calls → Use [Fine Tuning](../../fine_tuning/README.md)
- Complex reasoning requiring structured training data
- Performance-critical applications needing optimized models
- Domain-specific terminology the model doesn't know

## Related Topics
- [RAG](../rag/README.md) — Combining prompts with retrieved knowledge
- [Agents](../agents/README.md) — Prompts as agent instructions
- [Fine Tuning](../../fine_tuning/README.md) — When prompting isn't enough

## Practical Project Ideas
1. Compare zero-shot vs few-shot performance on classification task
2. Design prompts that extract structured data from unstructured text
3. Build a prompt library for common tasks in your domain
4. Experiment with chain-of-thought prompting for complex reasoning

---

Difficulty Level: 🟢 Beginner
