# RNN (Recurrent Neural Networks)

## What is it?
RNNs are neural networks designed for sequential data. Unlike standard networks that process independent inputs, RNNs maintain a hidden state that carries information from previous time steps.

## Why does it exist?
Sequential data has temporal dependencies:
- Text: each word depends on previous words
- Time series: current value depends on past values
- Speech: sounds form meaningful sequences

RNNs capture these dependencies through their recurrent connection.

## Core Concepts

| Concept | Purpose | Challenge |
|---------|----------|-----------|
| Hidden State | Carry information across time steps | Can degrade over long sequences |
| LSTM (Long Short-Term Memory) | Solve vanishing gradients | More complex architecture |
| GRU (Gated Recurrent Unit) | Simplified LSTM alternative | Slightly less expressive than LSTM |
| Bidirectional RNN | Process sequence both directions | Requires full sequence available |

## The Vanishing Gradient Problem
Standard RNNs struggle with long sequences because gradients vanish during backpropagation through time. Solutions:
- **LSTM** — Gated cells preserve information selectively
- **GRU** — Simplified gating mechanism
- **Transformer** — Bypass recurrence entirely with attention (see below)

## When should I use it?
- Short to medium sequences where order matters
- Time series prediction
- Text generation tasks
- Sequential decision making

## When should I NOT use it?
- Long sequences → [Transformer](../transformer/README.md) handles better
- Parallel processing needed — RNNs are inherently sequential
- Very long-range dependencies → Transformer attention is superior

## Related Topics
- [Backpropagation](../backpropagation/README.md) — Extended to BPTT (Backprop Through Time)
- [Transformer](../transformer/README.md) — Modern replacement for most RNN use cases
- [NLP](../../nlp/README.md) — Primary application domain

## Practical Project Ideas
1. Build a character-level text generator with LSTM
2. Predict stock prices from time series data
3. Compare RNN vs Transformer on the same sequence task

---

Difficulty Level: 🟡 Intermediate
