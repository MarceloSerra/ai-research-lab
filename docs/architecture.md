# Architecture

## System Overview

AI Research Lab is structured as a learning-first repository where every directory teaches concepts before showing code. The architecture separates concerns into three layers: knowledge, practice, and infrastructure.

## Layers

### Knowledge Layer
- **Discipline READMEs**: Each major field (Classical ML, DL, NLP, etc.) has an educational README
- **Sub-topic READMEs**: Specific techniques explained with decision guidance
- [Learning Roadmap](learning-roadmap.md): Progressive path through all topics

### Practice Layer
- **Notebooks**: Interactive exploration and experimentation
- **Experiments**: Structured, reproducible experiment runs
- **Datasets**: Curated data collections for each domain

### Infrastructure Layer
- **Tools**: Shared utilities across experiments
- **Reports**: Results documentation and analysis
- **Research Templates**: Standardized project methodology

## Key Architectural Decisions

| Decision | Rationale | Reference |
|----------|-----------|-----------|
| README-first structure | Knowledge before code — learn why before how | Learning philosophy |
| Relative links between topics | Web of knowledge, not isolated docs | Internal linking |
| Mermaid diagrams | Visual learners benefit from flowcharts | Main README |
| Decision tree format | Problem → Technique mapping | Main README |
| Conventional Commits | Consistent commit history across contributors | Git conventions |

## Topic Relationships

```
Classical ML ──→ Deep Learning ──→ Embeddings ──→ LLM Engineering
     ↑                    ↑                  ↑              ↓
     │                    │                  │              ↓
Feature Eng ←──────────── Clustering ←──── Semantic Search  ↓
                                                              ↓
                                              Fine-Tuning ←── RAG
```
