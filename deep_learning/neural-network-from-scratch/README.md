# Neural Network From Scratch

## What is it?
Building a neural network from scratch means implementing the core components — layers, activation functions, forward pass, and backward pass — without using frameworks like PyTorch or TensorFlow.

## Why does it exist?
Understanding what happens inside deep learning frameworks is crucial:
- Frameworks abstract away critical details
- Debugging requires understanding internals
- Custom architectures need low-level control
- True mastery comes from building fundamentals yourself

## Core Components

| Component | Purpose | Math Behind It |
|-----------|----------|----------------|
| Layer (Perceptron) | Basic computation unit | y = Wx + b |
| Activation Function | Introduce non-linearity | ReLU, Sigmoid, Tanh |
| Forward Pass | Compute predictions | Matrix multiplication chain |
| Loss Function | Measure error | MSE, Cross-entropy |
| Backward Pass | Compute gradients | Chain rule, backpropagation |

## When should I use it?
- Learning how neural networks actually work
- Building custom architectures frameworks don't support
- Educational purposes and research exploration
- Understanding what frameworks abstract away

## When should I NOT use it?
- Production systems → Use established frameworks
- Complex models needing optimized computation
- Time-constrained projects where framework speed matters

## Related Topics
- [Backpropagation](../backpropagation/README.md) — The learning algorithm this network uses
- [CNN](../cnn/README.md) — Specialized neural networks for images
- [Transformer](../transformer/README.md) — Modern architecture powering LLMs

## Practical Project Ideas
1. Implement a 2-layer network that classifies XOR
2. Build a network that fits polynomial curves
3. Compare your implementation against PyTorch on the same task

---

Difficulty Level: 🟡 Intermediate
