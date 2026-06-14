# Classical Machine Learning

## What is it?
Classical machine learning refers to algorithms that learn patterns from data without deep neural networks. It includes regression, classification, clustering, and dimensionality reduction techniques using libraries like scikit-learn.

## Why does it exist?
Before deep learning dominated headlines, classical ML solved real problems effectively. Many production systems still rely on these methods because they are:
- **Fast to train** — Minutes vs hours/days
- **Interpretable** — You can explain decisions
- **Data-efficient** — Work well with small datasets
- **Low-cost** — No GPU required

## Sections

| Topic | Description | Difficulty |
|-------|-------------|------------|
| [Regression](regression/README.md) | Predicting continuous values | 🟢 Beginner |
| [Classification](classification/README.md) | Categorizing data into groups | 🟢 Beginner |
| [Clustering](clustering-unsupervised/README.md) | Finding groups without labels | 🟢 Beginner |
| [Feature Engineering](feature-engineering/README.md) | Creating better input features | 🟡 Intermediate |
| [Model Selection](model-selection/README.md) | Choosing the right model | 🟡 Intermediate |

## When should I use it?
- Small to medium datasets (< 100K samples)
- Tabular data (spreadsheets, databases)
- Need interpretability and explainability
- Limited computational resources
- Quick prototyping and baseline models

## When should I NOT use it?
- Raw images, audio, or text sequences → Use [Deep Learning](../deep_learning/README.md)
- Very large datasets with complex patterns → Consider neural networks
- State-of-the-art performance requirements → Modern DL often wins

## Related Topics
- [Deep Learning](../deep_learning/README.md) — The natural evolution beyond classical ML
- [Embeddings](../embeddings/README.md) — Feature representation techniques
- [NLP](../nlp/README.md) — Language-specific applications

## Practical Project Ideas
1. Predict house prices using regression on a housing dataset
2. Classify iris flowers using different classifiers
3. Segment customers using clustering for marketing
4. Build a spam classifier from scratch

---

Difficulty Level: 🟢 Beginner → 🟡 Intermediate
