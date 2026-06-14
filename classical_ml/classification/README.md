# Classification

## What is it?
Classification assigns data points to discrete categories. Unlike regression (which predicts numbers), classification answers: "Which group does this belong to?"

## Why does it exist?
Categorization is fundamental to decision-making:
- Spam vs not spam
- Disease diagnosis: present vs absent
- Customer churn: will leave vs will stay
- Sentiment: positive, neutral, negative

## Common Algorithms

| Algorithm | Best For | Complexity |
|-----------|----------|------------|
| Logistic Regression | Binary classification, baseline | 🟢 Beginner |
| k-Nearest Neighbors | Small datasets, simple patterns | 🟢 Beginner |
| Decision Trees | Interpretable rules | 🟢 Beginner |
| Random Forest | Robust, handles many features | 🟡 Intermediate |
| SVM (Support Vector Machines) | High-dimensional data | 🟡 Intermediate |
| Naive Bayes | Text classification, fast training | 🟢 Beginner |

## When should I use it?
- Target variable is categorical (discrete classes)
- Clear boundaries between groups exist in the data
- You need to make decisions based on categories

## When should I NOT use it?
- Predicting continuous values → Use [Regression](../regression/README.md)
- No clear category structure → Consider [Clustering](../clustering-unsupervised/README.md)
- Complex patterns in images/text → Use [Deep Learning](../../deep_learning/README.md)

## Evaluation Metrics
- **Accuracy** — Overall correctness (can be misleading with imbalanced data)
- **Precision** — Of predicted positives, how many are correct?
- **Recall** — Of actual positives, how many did we find?
- **F1 Score** — Harmonic mean of precision and recall
- **Confusion Matrix** — Full breakdown of predictions

## Related Topics
- [Regression](../regression/README.md) — The continuous-value counterpart
- [NLP Text Classification](../../nlp/text-classification/README.md) — Classification for text data
- [Model Selection](../model-selection/README.md) — Choosing the right classifier

## Practical Project Ideas
1. Build a spam email classifier
2. Predict customer churn from subscription data
3. Classify wine quality from chemical properties
4. Detect fraudulent transactions

---

Difficulty Level: 🟢 Beginner
