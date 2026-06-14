# Model Selection

## What is it?
Model selection is the process of choosing the best algorithm and configuration for your specific problem. It's not about using the most complex model — it's about finding the right fit.

## Why does it exist?
No single algorithm wins all competitions. Different problems require different approaches:
- Data size affects which models work well
- Feature types matter (numeric, categorical, text)
- Performance requirements vary (speed vs accuracy tradeoff)

## Selection Framework

```mermaid
flowchart TD
    A[What is your target?] --> B{Continuous or Categorical?}
    B -->|Continuous| C[Regression]
    B -->|Categorical| D[Classification]
    B -->|Unknown groups| E[Clustering]
    
    C --> F{Data size?}
    D --> F
    F -->|Small < 1K| G[Simple models: Linear, k-NN]
    F -->|Medium 1K-100K| H[Ensembles: Random Forest, Gradient Boosting]
    F -->|Large > 100K| I[XGBoost, LightGBM, Neural Networks]
    
    G --> J{Need interpretability?}
    H --> J
    J -->|Yes| K[Linear models, Decision Trees]
    J -->|No| L[Any high-performance model]
```

## Validation Methods

| Method | Use When | Tradeoff |
|--------|----------|----------|
| Train/Test Split | Quick baseline | Single split may be unlucky |
| k-Fold Cross-Validation | Standard evaluation | k times slower training |
| Stratified k-Fold | Imbalanced classes | Preserves class distribution |
| Time Series Split | Temporal data | Prevents future leakage |

## Common Pitfalls
1. **Overfitting** — Model memorizes training data, fails on new data
2. **Data Leakage** — Future information accidentally in training data
3. **Ignoring baseline** — Not comparing against simple approaches first
4. **Chasing metrics** — Optimizing for numbers that don't matter to the business

## Related Topics
- [Regression](../regression/README.md) — Regression model selection
- [Classification](../classification/README.md) — Classifier comparison
- [Feature Engineering](../feature-engineering/README.md) — Prerequisite step

## Practical Project Ideas
1. Compare 5 classifiers on the same dataset, rank by F1 score
2. Use cross-validation to find optimal k for k-NN
3. Build a pipeline: preprocessing → model selection → evaluation
4. Implement early stopping to prevent overfitting

---

Difficulty Level: 🟡 Intermediate
