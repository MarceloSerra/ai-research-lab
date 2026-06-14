# Deep Learning

## What is it?
Deep learning uses multi-layered neural networks to learn representations from data automatically. Unlike classical ML (where you engineer features manually), deep learning discovers features through layers of computation.

## How it differs from Classical ML

| Aspect | Classical ML | Deep Learning |
|--------|-------------|---------------|
| Feature engineering | Manual, domain expertise required | Automatic, learned from data |
| Data hunger | Works with small datasets | Needs large datasets for best results |
| Raw data handling | Requires preprocessing | Handles raw images, text, audio directly |
| Computational cost | CPU sufficient | GPU preferred/required |
| Interpretability | Often interpretable | Black box (generally)

## Why Neural Networks Matter
Neural networks inspired by biological neurons can approximate any function given enough layers and data. This universality makes them applicable to virtually any pattern-recognition problem.

## Sections

| Topic | Description | Difficulty |
|-------|-------------|------------|
| [Neural Network From Scratch](neural-network-from-scratch/README.md) | Building NN without frameworks | 🟡 Intermediate |
| [Backpropagation](backpropagation/README.md) | How networks learn — the core algorithm | 🔴 Advanced |
| [CNN](cnn/README.md) | Convolutional networks for images | 🟡 Intermediate |
| [RNN](rnn/README.md) | Recurrent networks for sequences | 🟡 Intermediate |
| [Transformer](transformer/README.md) | Attention-based architecture, powers LLMs | 🔴 Advanced |

## When should I use it?
- Large datasets available (10K+ samples)
- Complex patterns that classical ML can't capture
- Raw data: images, audio, text sequences
- Computational resources available (GPUs)
- Performance matters more than interpretability

## When should I NOT use it?
- Small datasets → [Classical ML](../classical_ml/README.md) performs better
- Need interpretability and explainability
- Limited computational resources
- Simple relationships between features and target

## Related Topics
- [Classical ML](../classical_ml/README.md) — Foundation before deep learning
- [Embeddings](../embeddings/README.md) — Learned by neural networks
- [NLP](../nlp/README.md) — Deep learning for language
- [Computer Vision](../computer_vision/README.md) — Deep learning for images

## Practical Project Ideas
1. Build a digit recognizer from scratch using basic neural network
2. Implement backpropagation by hand to understand the math
3. Train a CNN on CIFAR-10 image classification
4. Build a text generator with RNN/LSTM

---

Difficulty Level: 🟡 Intermediate → 🔴 Advanced
