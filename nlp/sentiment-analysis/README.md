# Sentiment Analysis

## What is it?
Sentiment analysis determines the emotional tone of text: positive, negative, or neutral. It measures opinion, attitude, and emotion expressed in language.

## Why does it exist?
Understanding sentiment drives business decisions:
- Monitor brand reputation from customer reviews
- Analyze public reaction to products or events
- Detect customer dissatisfaction early
- Measure engagement quality on social media

## Approaches

| Approach | Methods | Strengths |
|----------|---------|-----------|
| Lexicon-based | Word lists with sentiment scores | Fast, interpretable, no training needed |
| Classical ML | SVM/Naive Bayes + features | Works well with labeled data |
| Deep Learning | LSTM/CNN on text | Captures context better |
| Transformer-based | Fine-tuned BERT/RoBERTa | State-of-the-art accuracy |

## Challenges
- **Sarcasm**: "Great, another meeting" — positive word, negative sentiment
- **Context dependence**: "This movie is sick" — can be positive or negative
- **Mixed sentiment**: "Good camera, terrible battery" — different sentiments per aspect
- **Domain specificity**: "Hot" in restaurant reviews vs tech reviews

## When should I use it?
- Analyzing customer feedback and reviews
- Monitoring social media brand perception
- Measuring public opinion on topics
- Quality assurance for customer interactions

## When should I NOT use it?
- Extracting specific entities → Use [Named Entity Recognition](../named-entity-recognition/README.md)
- Categorizing by topic → Use [Text Classification](../text-classification/README.md)
- Understanding complex reasoning → Use LLM analysis

## Related Topics
- [Text Classification](../text-classification/README.md) — Sentiment is a form of classification
- [Embeddings](../../embeddings/README.md) — Sentiment-aware embeddings exist
- [LLM Evaluation](../../llm/evaluation/README.md) — Evaluating model sentiment understanding

## Practical Project Ideas
1. Analyze Twitter sentiment about a product launch
2. Classify movie reviews as positive/negative/neutral
3. Track sentiment changes over time for a brand
4. Build aspect-based sentiment analysis (sentiment per feature)

---

Difficulty Level: 🟢 Beginner
