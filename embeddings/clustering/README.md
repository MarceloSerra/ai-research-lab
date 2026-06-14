# Clustering (Embeddings)

## What is it?
Clustering groups similar embeddings together without predefined labels. It discovers hidden patterns and natural groupings in your data's vector representation.

## Why does it exist?
When you have thousands of embedded documents, products, or items:
- You can't manually categorize everything
- Hidden patterns may not be obvious from raw features
- Grouping reveals structure for downstream tasks

Clustering turns a flat collection into organized groups.

## Common Approaches

| Method | Best For | Tradeoff |
|--------|----------|----------|
| K-Means on embeddings | Simple, fast clustering | Requires specifying k |
| DBSCAN | Finding natural cluster boundaries | Sensitive to density parameters |
| HDBSCAN | Robust clustering with noise detection | More complex tuning |
| Agglomerative | Hierarchical nested clusters | Slower for large datasets |

## When should I use it?
- Discovering topics in document collections
- Segmenting customers from behavioral embeddings
- Quality control — outliers indicate anomalies
- Pre-processing before supervised learning

## When should I NOT use it?
- Clear labels already exist → Use [Classification](../../classical_ml/classification/README.md)
- Need specific predictions, not exploration
- Embeddings don't capture relevant similarity dimensions

## Related Topics
- [Vector Search](../vector-search/README.md) — Clusters improve search organization
- [Semantic Search](../semantic-search/README.md) — Cluster-based routing for queries
- [Classical Clustering](../../classical_ml/clustering-unsupervised/README.md) — Foundational clustering concepts

## Practical Project Ideas
1. Discover topics in news article embeddings
2. Segment customers from purchase history embeddings
3. Find anomalous samples in product review embeddings

---

Difficulty Level: 🟡 Intermediate
