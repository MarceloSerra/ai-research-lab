# Image Classification

## What is it?
Image classification assigns a single category label to an entire image: cat/dog, healthy/diseased, spam image/legitimate.

## Why does it exist?
Categorizing visual content automates decisions:
- Medical diagnosis from X-rays and scans
- Content filtering for inappropriate images
- Product categorization in e-commerce
- Species identification in biology

## Common Architectures

| Architecture | Era | Key Feature |
|-------------|-----|-------------|
| LeNet | 1990s | First successful CNN |
| AlexNet | 2012 | Deep learning revolution |
| VGG | 2015 | Simple, deep architecture |
| ResNet | 2015 | Skip connections solve vanishing gradients |
| EfficientNet | 2019 | Optimal accuracy-compute tradeoff |

## When should I use it?
- Single label per image needed
- Clear category boundaries exist
- Sufficient labeled training data available

## When should I NOT use it?
- Multiple objects to locate → Use [Object Detection](../object-detection/README.md)
- Pixel-level precision needed → Use [Image Segmentation](../image-segmentation/README.md)
- No labeled data available → Consider self-supervised learning

## Related Topics
- [CNN](../../deep_learning/cnn/README.md) — Core architecture for classification
- [Object Detection](../object-detection/README.md) — More detailed localization
- [Transfer Learning](../../fine_tuning/instruction-tuning/README.md) — Reusing pre-trained models

## Practical Project Ideas
1. Classify CIFAR-10 images with a CNN from scratch
2. Build a medical image classifier (pneumonia detection from X-rays)
3. Create a plant disease detector for agriculture

---

Difficulty Level: 🟢 Beginner
