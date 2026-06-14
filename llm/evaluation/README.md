# Evaluation

## What is it?
LLM evaluation measures how well language models perform on specific tasks. Unlike classical ML metrics (accuracy, F1), LLM evaluation handles open-ended generation, reasoning quality, and subjective outputs.

## Why does it exist?
Evaluating LLMs is fundamentally harder than classical ML:
- Multiple valid answers may exist for a single question
- Output quality includes fluency, coherence, factuality, and relevance
- Human judgment often differs from automated metrics
- Different tasks require different evaluation criteria

Without proper evaluation, you can't compare models or measure improvement.

## Evaluation Methods

| Method | Description | When to Use |
|--------|-------------|-------------|
| Automated Metrics | BLEU, ROUGE, perplexity | Quick baseline comparison |
| Human Evaluation | Rating outputs by humans | Gold standard for quality |
| LLM-as-Judge | Using another LLM to evaluate | Scalable quality assessment |
| Task-Specific Metrics | Exact match, F1 for QA | When ground truth exists |
| Benchmark Suites | MMLU, GSM8K, HumanEval | Standardized comparison across models |

## Key Dimensions

| Dimension | Question | Metric Example |
|-----------|----------|----------------|
| Accuracy | Is the answer correct? | Exact match, factuality score |
| Completeness | Does it cover all aspects? | Coverage ratio |
| Relevance | Is it on-topic? | Off-topic rate |
| Safety | Is it harmful or biased? | Toxicity score |
| Efficiency | How many tokens/steps? | Token count, latency |

## When should I use it?
- Comparing different models for a task
- Measuring improvement after fine-tuning
- Validating RAG system quality
- Establishing baselines before optimization

## When should I NOT use it?
- Early prototyping where rough comparison suffices
- Very constrained tasks with clear success criteria → simple testing works
- Evaluation cost exceeds the value of insights gained

## Related Topics
- [Prompt Engineering](../prompt-engineering/README.md) — Evaluating prompt effectiveness
- [RAG](../rag/README.md) — Evaluating retrieval quality and generation accuracy
- [Fine Tuning](../../fine_tuning/README.md) — Measuring fine-tuned model improvement

## Practical Project Ideas
1. Build an evaluation pipeline for your QA system using LLM-as-judge
2. Compare multiple models on your specific task with consistent metrics
3. Create a human evaluation interface for rating model outputs
4. Implement automated regression testing for prompt changes

---

Difficulty Level: 🟡 Intermediate
