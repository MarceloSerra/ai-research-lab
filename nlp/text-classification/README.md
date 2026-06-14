# Text Classification

## What is it?
Text classification assigns categories to text documents: spam/ham, topic labels, language identification, intent detection.

## Why does it exist?
Unstructured text needs organization:
- Route customer inquiries to appropriate departments
- Filter unwanted content automatically
- Organize documents by topic
- Detect harmful or policy-violating content

## Approaches

| Approach | Methods | When to Use |
|----------|---------|-------------|
| Classical ML | Naive Bayes, SVM + TF-IDF | Small datasets, interpretability needed |
| Deep Learning | CNN/RNN on text | Medium datasets, better performance |
| Transformer-based | BERT, RoBERTa fine-tuning | Large datasets, state-of-the-art accuracy |

## When should I use it?
- Categorizing documents, emails, messages
- Content filtering and moderation
- Intent detection in conversational AI
- Topic labeling for organization

## When should I NOT use it?
- Extracting specific entities → Use [Named Entity Recognition](../named-entity-recognition/README.md)
- Understanding opinions → Use [Sentiment Analysis](../sentiment-analysis/README.md)
- Open-ended text generation → Use LLMs

## Related Topics
- [Classification](../../classical_ml/classification/README.md) — Foundational classification concepts
- [Embeddings](../../embeddings/README.md) — Text representations for classification
- [Sentiment Analysis](../sentiment-analysis/README.md) — Specialized text classification

## Practical Project Ideas
1. Classify news articles by topic (sports, politics, entertainment)
2. Build intent classifier for chatbot routing
3. Detect fake news from article text

---

Difficulty Level: 🟢 Beginner
