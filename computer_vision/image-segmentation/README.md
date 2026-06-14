# Image Segmentation

## What is it?
Image segmentation assigns a class label to every pixel in an image. Unlike detection (bounding boxes), segmentation provides pixel-level precision about what belongs to each object.

## Why does it exist?
Some applications need precise boundaries:
- Medical imaging — tumor boundaries for surgery planning
- Autonomous driving — road vs sidewalk vs building distinction
- Photo editing — isolating subjects from backgrounds
- Satellite imagery — land use classification at pixel level

## Types

| Type | Output | Use Case |
|------|--------|----------|
| Semantic Segmentation | Pixel class labels | What type is each pixel? |
| Instance Segmentation | Individual object masks | Separate instances of same class |
| Panoptic Segmentation | Both combined | Complete scene understanding |

## Common Architectures

| Architecture | Key Feature | Application |
|-------------|-------------|-------------|
| U-Net | Encoder-decoder with skip connections | Medical imaging standard |
| DeepLab | Atrous convolution for multi-scale | General purpose |
| Mask R-CNN | R-CNN + mask branch | Instance segmentation |

## When should I use it?
- Pixel-level precision required
- Object boundaries matter critically
- Dense prediction needed across entire image
- Medical or scientific analysis requiring accuracy

## When should I NOT use it?
- Coarse localization sufficient → Use [Object Detection](../object-detection/README.md)
- Single category per image → Use [Image Classification](../image-classification/README.md)
- Limited labeled data — pixel annotation is expensive

## Related Topics
- [CNN](../../deep_learning/cnn/README.md) — Feature extraction foundation
- [Object Detection](../object-detection/README.md) — Less precise but easier to label
- [Computer Vision Overview](../README.md) — Segmentation as advanced CV task

## Practical Project Ideas
1. Segment cells in microscopy images using U-Net
2. Build a road segmentation system for autonomous driving
3. Create background removal tool for product photos

---

Difficulty Level: 🔴 Advanced
