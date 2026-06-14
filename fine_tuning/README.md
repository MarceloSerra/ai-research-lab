# Fine Tuning

## What is it?
Fine tuning adapts a pre-trained model to specific tasks by continuing training on domain-specific data. Instead of using a general-purpose model, you customize it for your particular use case.

## Why does it exist?
General models have limitations:
- **Domain specificity** — General models lack specialized knowledge
- **Style consistency** — Need consistent tone, format, or behavior
- **Performance** — Fine-tuned models often outperform prompting on narrow tasks
- **Efficiency** — Smaller fine-tuned models can match larger general models on specific tasks

## Sections

| Topic | Description | Difficulty |
|-------|-------------|------------|
| [LoRA](lora/README.md) | Low-Rank Adaptation — efficient parameter tuning | 🟡 Intermediate |
| [QLoRA](qlora/README.md) | Quantized LoRA — train on consumer GPUs | 🔴 Advanced |
| [Instruction Tuning](instruction-tuning/README.md) | Teaching models to follow instructions | 🟡 Intermediate |
| [Synthetic Datasets](synthetic-datasets/README.md) | Generating training data programmatically | 🔴 Advanced |

## When should I use it?
- Domain-specific performance matters more than general capability
- Consistent behavior/style across many calls is critical
- You have quality labeled data for your specific task
- Prompting alone doesn't achieve required performance level

## When should I NOT use it?
- Task is simple enough that prompting works well
- Insufficient training data for quality fine-tuning
- Rapidly changing requirements make retraining costly
- General model capability suffices for the application

## Related Topics
- [LLM Engineering](../llm/README.md) — Fine tuning as LLM customization
- [Prompt Engineering](../llm/prompt-engineering/README.md) — Try prompting first before fine-tuning
- [Evaluation](../llm/evaluation/README.md) — Measuring fine-tuned model improvement

## Practical Project Ideas
1. Fine-tune a small model for your specific classification task
2. Compare LoRA vs full fine-tuning on resource usage and quality
3. Create instruction-tuned dataset from existing Q&A pairs
4. Generate synthetic training data for rare edge cases

---

Difficulty Level: 🟡 Intermediate → 🔴 Advanced
