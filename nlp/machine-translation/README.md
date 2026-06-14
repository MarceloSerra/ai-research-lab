# Machine Translation

## What is it?
Machine translation automatically converts text from one language to another. Modern systems use neural networks (NMT) rather than rule-based approaches.

## Why does it exist?
Language barriers limit global communication:
- Business operates across languages
- Research needs cross-language access
- Content reaches multilingual audiences
- Real-time communication requires instant translation

## Evolution of Translation

| Era | Method | Quality |
|-----|--------|---------|
| 1950s-1990s | Rule-based | Poor, limited vocabulary |
| 2000s | Statistical MT | Better, data-driven but fragmented |
| 2016+ | Neural MT (NMT) | Fluent, context-aware |
| Present | Transformer-based | Near-human for major language pairs |

## Core Architecture
Modern translation uses **encoder-decoder Transformers**:
1. Encoder reads source language fully
2. Attention connects source to target positions
3. Decoder generates target language token by token

## When should I use it?
- Cross-language communication needs
- Content localization
- Multilingual document processing
- Building translation services

## When should I NOT use it?
- Legal/medical documents requiring certified human translation
- Creative writing where nuance matters critically
- Low-resource language pairs with poor model quality
- Context-dependent terminology needing domain expertise

## Related Topics
- [Transformer](../../deep_learning/transformer/README.md) — Architecture powering modern translation
- [NLP Overview](../README.md) — Translation as NLP task
- [LLM Engineering](../../llm/README.md) — LLMs excel at translation

## Practical Project Ideas
1. Build a simple translator between two languages using seq2seq model
2. Compare machine translation quality across different systems
3. Implement domain-specific translation (medical, legal terminology)

---

Difficulty Level: 🔴 Advanced
