# LoRA (Low-Rank Adaptation)

## What is it?
LoRA adapts large models by training small rank decomposition matrices instead of updating all parameters. It achieves comparable performance to full fine-tuning while using far fewer resources.

## Why does it exist?
Full fine-tuning a 70B parameter model requires:
- Massive GPU memory (hundreds of GB)
- Expensive compute infrastructure
- Long training times
- High storage costs for checkpoints

LoRA reduces this by freezing the base model and training only small adapter matrices — typically <1% of total parameters.

## How It Works
Instead of updating weight matrix W directly:
- Freeze W completely
- Add low-rank decomposition: ΔW = BA (where B is m×r, A is r×n, r << min(m,n))
- Train only B and A matrices
- At inference, merge adapters: W' = W + BA

## Resource Requirements

| Parameter | Full Fine-Tuning | LoRA | Savings |
|-----------|-----------------|------|---------|
| Trainable params | 100% | ~0.1-1% | 99%+ fewer |
| GPU memory | Massive (full model gradients) | Small (adapter gradients only) | ~80-90% less |
| Storage per checkpoint | GBs | MBs | ~95% less |
| Training time | Hours/days | Minutes/hours | Similar or faster |

## When should I use it?
- Adapting large models to specific tasks
- Limited GPU resources available
- Multiple task variants needed (swap adapters, not full models)
- Rapid experimentation with different adaptations

## When should I NOT use it?
- Very small models where full fine-tuning is cheap anyway
- Tasks requiring fundamental model architecture changes
- Extreme performance requirements where full tuning marginally helps

## Related Topics
- [QLoRA](../qlora/README.md) — LoRA + quantization for even smaller GPUs
- [Instruction Tuning](../instruction-tuning/README.md) — Common use case for LoRA
- [Fine Tuning Overview](../README.md) — LoRA as efficient fine-tuning method

## Practical Project Ideas
1. Fine-tune a language model for code generation using LoRA
2. Compare LoRA adapter quality vs full fine-tuning on small models
3. Create multiple LoRA adapters for different tasks on one base model

---

Difficulty Level: 🟡 Intermediate
