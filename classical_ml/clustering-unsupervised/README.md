# Clustering (Unsupervised)

## What is it?
Clustering groups similar data points together WITHOUT predefined labels. Unlike classification (which knows the categories), clustering discovers structure in unlabeled data.

## Why does it exist?
Many problems have no labeled training data:
- Customer segmentation for marketing
- Anomaly detection — outliers stand out from clusters
- Exploratory data analysis — discover hidden patterns
- Document organization — group similar content

## Common Algorithms

| Algorithm | Best For | Complexity |
|-----------|----------|------------|
| K-Means | Simple spherical clusters, fast | 🟢 Beginner |
| DBSCAN | Arbitrary shapes, noise detection | 🟡 Intermediate |
| Hierarchical Clustering | Nested group structures | 🟡 Intermediate |
| Gaussian Mixture Models | Probabilistic cluster assignment | 🟡 Intermediate |

## When should I use it?
- No labeled data available
- Exploring dataset structure before supervised learning
- Finding natural groupings in data
- Detecting anomalies (points that don't fit any cluster)

## When should I NOT use it?
- You have clear labels → Use [Classification](../classification/README.md)
- Need specific predictions, not exploration
- Data has no inherent grouping structure

## Evaluation Challenges
Clustering is harder to evaluate because there's no ground truth. Common approaches:
- **Silhouette Score** — How well-separated clusters are
- **Elbow Method** — Finding optimal number of clusters
- Visual inspection with dimensionality reduction (PCA, t-SNE)

## Related Topics
- [Classification](../classification/README.md) — Supervised counterpart
- [Embedding Clustering](../../embeddings/clustering/README.md) — Clustering vector representations
- [Feature Engineering](../feature-engineering/README.md) — Better features = better clusters

## Practical Project Ideas
1. Segment customers by purchasing behavior
2. Group news articles by topic without labels
3. Detect fraudulent transactions as outliers
4. Cluster genes by expression patterns

---

Difficulty Level: 🟢 Beginner → 🟡 Intermediate
