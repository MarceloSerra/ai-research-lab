# QLoRA (Quantized Low-Rank Adaptation)

## What is it?
QLoRA combines LoRA efficiency with 4-bit quantization, enabling fine-tuning of large models on consumer GPUs (even a single 16GB card). It makes LLM customization accessible without enterprise infrastructure.

## Why does it exist?
Even LoRA requires significant GPU memory for very large models:
- 70B parameter model with LoRA still needs ~80GB+ VRAM
- Most developers don't have access to A100/H100 GPUs
- Cloud GPU time is expensive for experimentation

QLoRA solves this by quantizing the base model to 4-bit precision while maintaining quality through techniques like page-wise activation memory scaling.

## How It Works
1. **Quantize base model** to 4-bit (NF4 — Normal Float 4)
2. **Apply LoRA adapters** on top of quantized weights
3. **Train only adapters** with standard gradient descent
4. **Use advanced techniques**: paged optimizers, offloading to CPU when needed

## Resource Requirements

| Parameter | LoRA | QLoRA | Savings |
|-----------|------|-------|---------|
| Model precision | 16-bit (FP16) | 4-bit (NF4) | 75% less memory |
| Min GPU for 70B model | ~80GB VRAM | ~16-24GB VRAM | Consumer GPUs viable |
| Training quality | High | Nearly identical to LoRA | No meaningful loss |
| Inference speed | Standard | Slightly slower decode | Negligible in practice |

## When should I use it?
- Limited GPU resources (consumer hardware)
- Experimenting with large models without cloud costs
- Rapid prototyping of fine-tuned applications
- Educational/research purposes on accessible hardware

## When should I NOT use it?
- Maximum inference performance needed — quantization adds slight overhead
- Models where 4-bit precision degrades quality significantly (rare)
- Full precision required for downstream integration

## Related Topics
- [LoRA](../lora/README.md) — QLoRA builds on LoRA foundations
- [Instruction Tuning](../instruction-tuning/README.md) — Common QLoRA use case
- [Synthetic Datasets](../synthetic-datasets/README.md) — Training data for QLoRA

## Practical Project Ideas
1. Fine-tune a 34B parameter model on a single consumer GPU
2. Compare QLoRA vs full LoRA quality on benchmark tasks
3. Create domain-specific assistant using QLoRA on available hardware

---

Difficulty Level: 🔴 Advanced
