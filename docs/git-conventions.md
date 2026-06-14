# Git Conventions

## Commit Format

Conventional Commits with ML-specific scoping:

```
<type>(<scope>): <description>
```

### Types

| Type | Use For |
|------|---------|
| `feat` | New features or functionality |
| `fix` | Bug fixes |
| `refactor` | Code restructuring without behavior change |
| `docs` | Documentation only changes |
| `chore` | Build processes, dependencies, tooling |
| `perf` | Performance improvements |
| `test` | Adding or modifying tests |
| `data` | Dataset additions or modifications |

### Scopes

- `classical-ml` — Classical ML modules
- `dl` — Deep Learning components
- `nlp` — Natural Language Processing
- `llm` — LLM engineering, prompts, agents
- `embeddings` — Embedding and vector search
- `cv` — Computer Vision
- `fine-tuning` — LoRA, QLoRA, instruction tuning
- `datasets` — Data collection and preparation
- `experiments` — Experiment configurations
- `reports` — Results documentation
- `tools` — Utility scripts

### Examples

```
feat(classical-ml): add logistic regression classifier
docs(dl): explain backpropagation fundamentals
data(datasets): add IMDB sentiment dataset
fix(embeddings): normalize vector similarity scores
perf(cv): optimize image preprocessing pipeline
refactor(llm): extract prompt templates to shared module
```

## Branch Naming

| Type | Pattern | Example |
|------|---------|---------|
| Feature | `feat/<short-description>` | `feat/lora-finetuning` |
| Bug fix | `fix/<short-description>` | `fix/embedding-normalization` |
| Documentation | `docs/<short-description>` | `docs/backprop-readme` |

## Versioning

Semantic Versioning: `MAJOR.MINOR.PATCH`

- Incompatible architecture change → MAJOR
- New feature / backward compatible → MINOR
- Bug fix, docs, chore → PATCH
