# Feature Engineering

## What is it?
Feature engineering is the process of creating, transforming, and selecting input features to improve model performance. It's often said: "Data and features beat algorithms."

## Why does it exist?
Raw data rarely works well directly. Models need:
- Clean, consistent inputs
- Relevant signals extracted from noise
- Features that capture domain knowledge
- Properly scaled values for algorithm compatibility

## Key Techniques

| Technique | Description | Example |
|-----------|-------------|---------|
| Encoding Categoricals | Convert categories to numbers | One-hot encoding, label encoding |
| Scaling/Normalization | Put features on same scale | Min-max scaling, standardization |
| Feature Creation | Combine existing features | Age from birth date, aspect ratio from dimensions |
| Dimensionality Reduction | Reduce feature count | PCA, feature selection |
| Handling Missing Data | Fill or remove gaps | Mean imputation, KNN imputation |

## When should I use it?
- Before any model training — always prepare data first
- Model performance is poor despite good algorithms
- Features have different scales (some 0-1, others 0-10000)
- Categorical data needs numeric representation

## When should I NOT use it?
- Over-engineering features can cause overfitting
- Deep learning sometimes learns features automatically → [Deep Learning](../../deep_learning/README.md)
- Too many features relative to samples → Use dimensionality reduction

## The Golden Rule
Spend 60-80% of your ML project time on feature engineering. A simple model with great features often beats a complex model with poor features.

## Related Topics
- [Regression](../regression/README.md) — Benefits from good features
- [Classification](../classification/README.md) — Same principle applies
- [Embeddings](../../embeddings/README.md) — Automated feature learning

## Practical Project Ideas
1. Engineer features from raw dates (day of week, month, season)
2. Create interaction terms between numerical features
3. Compare model performance with and without feature scaling
4. Use PCA to reduce 50 features to 10 while preserving information

---

Difficulty Level: 🟡 Intermediate
