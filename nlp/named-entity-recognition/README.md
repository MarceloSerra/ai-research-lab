# Named Entity Recognition (NER)

## What is it?
NER identifies and classifies named entities in text into predefined categories: persons, organizations, locations, dates, monetary values, and domain-specific terms.

## Why does it exist?
Raw text contains structured information that needs extraction:
- "Apple announced $100B in investments on Monday in Cupertino"
  → Organization: Apple, Money: $100B, Date: Monday, Location: Cupertino
- Legal documents require extracting parties, dates, clauses
- Research papers need author names, institutions, citations

## Common Entity Types

| Type | Examples |
|------|----------|
| PERSON | Names of people |
| ORGANIZATION | Companies, institutions, agencies |
| LOCATION | Cities, countries, addresses |
| DATE | Specific dates, time periods |
| MONEY | Currency amounts |
| PRODUCT | Products, technologies, brands |

## When should I use it?
- Extracting structured data from unstructured text
- Information retrieval and knowledge base population
- Document analysis and summarization
- Building search indexes from extracted entities

## When should I NOT use it?
- Classifying entire documents → Use [Text Classification](../text-classification/README.md)
- Understanding overall sentiment → Use [Sentiment Analysis](../sentiment-analysis/README.md)
- Generating new text → Use LLMs

## Related Topics
- [Text Classification](../text-classification/README.md) — Document-level categorization
- [Embeddings](../../embeddings/README.md) — Entity representations for matching
- [LLM Tool Calling](../../llm/tool-calling/README.md) — Entities as function arguments

## Practical Project Ideas
1. Extract company names from financial news articles
2. Identify locations in travel blog posts
3. Build a timeline from dates extracted from historical documents

---

Difficulty Level: 🟡 Intermediate
