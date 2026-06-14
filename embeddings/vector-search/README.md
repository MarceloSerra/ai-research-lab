# Vector Search

## What is it?
Vector search finds the nearest vectors in a high-dimensional space. Given a query embedding, it returns the most similar items by measuring distance or angle between vectors.

## Why does it exist?
Traditional keyword search fails when:
- Users don't know exact terminology
- Synonyms express the same concept
- Context matters more than word matching

Vector search solves this by comparing meaning, not words.

## Core Concepts

| Concept | Description |
|---------|-------------|
| Cosine Similarity | Measures angle between vectors (0 to 1) |
| Euclidean Distance | Straight-line distance in vector space |
| ANN (Approximate Nearest Neighbor) | Fast search with slight accuracy tradeoff |
| Index Types | HNSW, IVF, Flat — different speed/accuracy tradeoffs |

## When should I use it?
- Finding similar items in a collection
- Building recommendation systems
- Document retrieval by similarity
- Duplicate detection

## When should I NOT use it?
- Exact matching needed → Use database equality queries
- Very small datasets (< 100 items) where linear scan is fast enough
- Real-time latency requirements under milliseconds

## Related Topics
- [Semantic Search](../semantic-search/README.md) — Vector search with meaning-focused embeddings
- [Clustering](../clustering/README.md) — Grouping vectors into clusters
- [RAG Experiments](../rag-experiments/README.md) — Using vector search for knowledge retrieval

## Practical Project Ideas
1. Build a movie recommendation system from embedding similarity
2. Find duplicate documents in a corpus
3. Implement nearest-neighbor image search

---

Difficulty Level: 🟢 Beginner
