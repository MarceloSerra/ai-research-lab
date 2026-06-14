# Regression

## What is it?
Regression predicts continuous numerical values. Given input features, a regression model outputs a number — like house price, temperature, or sales revenue.

## Why does it exist?
Many real-world problems involve predicting quantities:
- Sales forecasting
- Price prediction
- Demand estimation
- Risk scoring

## Common Algorithms

| Algorithm | Best For | Complexity |
|-----------|----------|------------|
| Linear Regression | Simple relationships, baseline | 🟢 Beginner |
| Ridge/Lasso | Feature selection, preventing overfitting | 🟡 Intermediate |
| Polynomial Regression | Non-linear patterns | 🟡 Intermediate |
| Decision Tree Regression | Interpretable non-linear models | 🟢 Beginner |
| Random Forest Regression | Robust performance | 🟡 Intermediate |

## When should I use it?
- Target variable is continuous (numbers)
- Relationship between features and target is learnable
- Historical data shows patterns that repeat

## When should I NOT use it?
- Predicting categories → Use [Classification](../classification/README.md)
- No clear relationship between inputs and output
- Time series with strong temporal dependencies → Consider specialized methods

## Evaluation Metrics
- **MAE** (Mean Absolute Error) — Average error magnitude
- **RMSE** (Root Mean Square Error) — Penalizes large errors more
- **R²** (R-squared) — Proportion of variance explained

## Related Topics
- [Classification](../classification/README.md) — The sibling technique for categories
- [Model Selection](../model-selection/README.md) — Choosing between regression models
- [Feature Engineering](../feature-engineering/README.md) — Better features = better predictions

## Practical Project Ideas
1. Predict housing prices from square footage, location, and amenities
2. Forecast monthly sales from historical data
3. Estimate energy consumption based on building characteristics

---

Difficulty Level: 🟢 Beginner
