# Instruction Tuning

## What is it?
Instruction tuning teaches models to follow human instructions effectively. Instead of continuing pre-training on raw text, instruction tuning uses (instruction, output) pairs to teach task-specific behavior.

## Why does it exist?
Base language models are not instruction-followers:
- They continue text patterns, not execute commands
- They don't understand formats like "classify this:" or "summarize in 3 bullets"
- They lack consistent behavior across different task types

Instruction tuning transforms a base model into an assistant that understands and executes diverse instructions.

## Data Format

Standard instruction tuning data:
```json
{
  "instruction": "Classify the sentiment of this review",
  "input": "The movie was amazing, best I've seen all year!",
  "output": "Positive"
}
```

Key characteristics:
- **Diverse instructions** — Many task types prevent overfitting to one pattern
- **Clear input/output separation** — Model learns to map inputs to outputs given instructions
- **Quality matters more than quantity** — Accurate outputs teach correct behavior

## When should I use it?
- Building domain-specific assistants
- Customizing model behavior for particular workflows
- Teaching models specialized formats or styles
- Improving instruction-following on specific task types

## When should I NOT use it?
- General capability needed → Use pre-trained instruction models directly
- Simple prompting achieves the goal → No fine-tuning needed
- Insufficient quality data → Garbage in, garbage out

## Related Topics
- [LoRA](../lora/README.md) — Efficient method for instruction tuning
- [QLoRA](../qlora/README.md) — Instruction tuning on consumer hardware
- [Synthetic Datasets](../synthetic-datasets/README.md) — Generating instruction data

## Practical Project Ideas
1. Instruction-tune a model for your domain's specific tasks
2. Compare instruction-following quality before and after fine-tuning
3. Create a multilingual instruction dataset for local language support
4. Build specialized assistant for code review or documentation generation

---

Difficulty Level: 🟡 Intermediate
