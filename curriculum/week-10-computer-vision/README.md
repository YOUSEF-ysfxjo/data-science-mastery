# Week 10 — Computer Vision

---

## What You Learn

### CNNs (Convolutional Neural Networks)
- Convolution operation — what does it do?
- Pooling (Max, Average)
- Architecture classics: LeNet, AlexNet, VGG, ResNet
- Why CNNs are better than MLPs for images

### Transfer Learning
- Use pre-trained models (ResNet50, EfficientNet)
- Freeze layers, fine-tune top
- ⭐ **This is what people actually use at work — not training from scratch.**

### Modern Approaches
- Vision Transformers (ViT)
- CLIP (text + image)
- Segment Anything Model (SAM)

### Tasks
- Image Classification
- Object Detection (YOLO)
- Semantic Segmentation (U-Net)
- Face Recognition (InsightFace, FaceNet)

---

## Libraries

- **torchvision** — ready-to-use datasets + models
- **timm** — 700+ pre-trained CV models
- **albumentations** — fast augmentations
- **OpenCV** — classic image processing

---

## Resources

- ⭐ **[CS231n — Stanford (Andrej Karpathy original)](http://cs231n.stanford.edu/)** — the world standard
- ⭐ **[Practical Deep Learning for Coders — fast.ai](https://course.fast.ai/)** — top-down approach
- **[KAUST Academy CV Course](https://academy.kaust.edu.sa/)** — if you're in Saudi Arabia, this is the best local option
- [PyTorch Vision Tutorials](https://pytorch.org/vision/stable/index.html)

---

## Challenge

Use Transfer Learning with ResNet50 to classify a dataset of your choice from [Kaggle Datasets](https://www.kaggle.com/datasets) (Chest X-ray, Cats vs Dogs, or a custom dataset). Upload the trained model to [Hugging Face Hub](https://huggingface.co/docs/hub/models-uploading).

---

[**← Week 9**](../week-09-neural-networks/) · [**Week 11 →**](../week-11-nlp-llms/)

