# Synthetic Datasets

## What is it?
Synthetic datasets are training data generated programmatically — by LLMs, rules, templates, or data augmentation techniques — rather than collected from human annotators. They enable fine-tuning when labeled data is scarce, expensive, or impossible to collect.

## Why does it exist?
Human-labeled data has fundamental constraints:
- **Cost**: Quality annotation requires experts (medical, legal, technical)
- **Scale**: Large models need large datasets — human labeling doesn't scale linearly
- **Rarity**: Edge cases and rare scenarios are hard to find in real data
- **Speed**: Waiting for annotation delays development cycles

Synthetic data solves these by generating training examples programmatically.

## Generation Methods

| Method | Description | Quality | Cost |
|--------|-------------|---------|------|
| LLM-generated | Use stronger models to create data for smaller ones | High | Moderate |
| Template-based | Fill structured templates with variations | Medium | Low |
| Rule-based | Apply transformation rules to existing data | Varies | Low |
| Data augmentation | Modify existing examples (paraphrase, noise) | Medium | Low |
| Human-in-the-loop | Generate then validate key samples | Highest | Moderate |

## Quality Principles

1. **Diversity**: Synthetic data must cover the same distribution as real data
2. **Accuracy**: Generated labels must be correct — wrong labels teach wrong behavior
3. **Validation**: Always test synthetic models on real held-out data
4. **Iterative refinement**: Use model failures to improve synthetic data generation

## When should I use it?
- Labeled data is too expensive or time-consuming to collect
- Edge cases need representation that's rare in real data
- Rapid prototyping before collecting human-labeled data
- Augmenting small labeled datasets with generated variations

## When should I NOT use it?
- Domain requires expert judgment that LLMs can't replicate reliably
- Safety-critical applications where synthetic errors are unacceptable
- Sufficient high-quality labeled data already exists
- Synthetic generation process introduces systematic biases

## Related Topics
- [Instruction Tuning](../instruction-tuning/README.md) — Synthetic instruction data
- [LoRA](../lora/README.md) — Train with synthetic datasets efficiently
- [Evaluation](../../llm/evaluation/README.md) — Validate synthetic model performance on real data

## Practical Project Ideas
1. Generate synthetic QA pairs from documentation for RAG fine-tuning
2. Create synthetic edge cases to improve model robustness
3. Compare models trained on synthetic vs human-labeled data
4. Build a pipeline that generates and validates synthetic training data automatically

---

Difficulty Level: 🔴 Advanced
