# Object Detection

## What is it?
Object detection finds and localizes multiple objects within an image. Unlike classification (one label per image), detection answers: "What objects are present AND where are they?"

## Why does it exist?
Many applications need object locations, not just categories:
- Autonomous driving — detect pedestrians, cars, signs
- Retail — count items on shelves
- Security — locate people in surveillance footage
- Medical imaging — find tumors with precise boundaries

## Output Format
Each detected object returns:
- **Class**: What it is (person, car, dog)
- **Bounding Box**: [x_min, y_min, x_max, y_max] location
- **Confidence Score**: How certain the model is

## Common Architectures

| Architecture | Type | Speed | Accuracy |
|-------------|------|-------|----------|
| YOLO (You Only Look Once) | Single-shot | Very fast | Good |
| Faster R-CNN | Two-stage | Moderate | High |
| SSD (Single Shot Detector) | Single-shot | Fast | Good |
| DETR | Transformer-based | Moderate | Very high |

## When should I use it?
- Locating objects within images
- Counting instances of object types
- Real-time visual monitoring
- Multi-object scene understanding

## When should I NOT use it?
- Single image categorization → Use [Image Classification](../image-classification/README.md)
- Pixel-level precision needed → Use [Image Segmentation](../image-segmentation/README.md)
- Object relationships matter more than locations → Consider scene graph models

## Related Topics
- [CNN](../../deep_learning/cnn/README.md) — Feature extraction backbone
- [Image Classification](../image-classification/README.md) — Simpler alternative
- [Image Segmentation](../image-segmentation/README.md) — More precise localization

## Practical Project Ideas
1. Detect objects in real-time webcam feed using YOLO
2. Count products on retail shelf images
3. Build a pedestrian detection system for safety applications

---

Difficulty Level: 🟡 Intermediate
