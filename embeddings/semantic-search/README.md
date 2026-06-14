# Semantic Search

## What is it?
Semantic search retrieves documents based on meaning, not keywords. It understands that "car" and "automobile" are related, or that "how do I fix" matches "repair guide."

## Why does it exist?
Keyword search has fundamental limitations:
- **Synonym problem**: Searching "happy" misses "joyful", "elated", "content"
- **Polysemy problem**: "Apple" could mean fruit or company
- **Context problem**: "Python" could mean snake or programming language

Semantic search uses embeddings to capture meaning and context, solving these problems.

## How It Works
1. Embed query text into a vector
2. Compare against document vectors using similarity metrics
3. Rank results by semantic closeness, not keyword overlap
4. Return top-k most relevant documents

## When should I use it?
- Enterprise search where users don't know exact terminology
- Document retrieval across diverse vocabulary
- Cross-language search (embeddings bridge languages)
- Finding conceptually related content

## When should I NOT use it?
- Exact phrase matching needed → Use keyword search
- Very specific technical queries with known terminology
- Legal/regulatory searches requiring precise matches
- Small datasets where manual curation is faster

## Related Topics
- [Vector Search](../vector-search/README.md) — The underlying mechanism
- [RAG Experiments](../rag-experiments/README.md) — Semantic search powers RAG retrieval
- [LLM RAG](../../llm/rag/README.md) — Full RAG systems use semantic search

## Practical Project Ideas
1. Build a FAQ search that understands natural language questions
2. Create a code snippet finder from descriptions
3. Implement cross-language document retrieval

---

Difficulty Level: 🟡 Intermediate
