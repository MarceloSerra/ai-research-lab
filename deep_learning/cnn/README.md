# CNN (Convolutional Neural Networks)

## What is it?
CNNs are neural networks designed for processing grid-like data — primarily images. They use convolution operations that detect local patterns (edges, textures, shapes) and compose them hierarchically.

## Why does it exist?
Standard neural networks fail on images because:
- Images have spatial structure — nearby pixels are related
- Objects appear at different locations — need translation invariance
- Raw pixel input is too large for dense layers

CNNs solve this with convolutions that share weights across spatial positions.

## Core Concepts

| Concept | Purpose | Description |
|---------|----------|-------------|
| Convolution Filter | Detect local patterns | Sliding window that extracts features |
| Pooling | Reduce dimensionality | Downsample while preserving important features |
| Feature Maps | Layer outputs | Each filter produces one feature map |
| Depth | Multiple filters per layer | Learn multiple pattern types simultaneously |

## When should I use it?
- Image classification, detection, segmentation
- Any 2D/3D grid data (medical images, satellite imagery)
- Video processing (3D convolutions)
- Pattern recognition in spatial data

## When should I NOT use it?
- Sequential data → Use [RNN](../rnn/README.md) or [Transformer](../transformer/README.md)
- Tabular data → Classical ML often performs better
- Very small image datasets where transfer learning isn't viable

## Related Topics
- [Backpropagation](../backpropagation/README.md) — How CNNs are trained
- [Image Classification](../../computer_vision/image-classification/README.md) — Primary CNN application
- [Object Detection](../../computer_vision/object-detection/README.md) — Advanced CV with CNNs

## Practical Project Ideas
1. Build a CNN for MNIST digit classification from scratch
2. Implement transfer learning with pre-trained ResNet
3. Compare CNN vs classical ML on image tasks

---

Difficulty Level: 🟡 Intermediate
