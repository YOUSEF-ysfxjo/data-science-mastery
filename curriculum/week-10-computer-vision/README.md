<div dir="rtl">

# الأسبوع ١٠ — الرؤية الحاسوبية
## Week 10 — Computer Vision

---

## ماذا تتعلم

### CNNs (Convolutional Neural Networks)
- Convolution operation — وش يسوي
- Pooling (Max, Average)
- Architecture classics: LeNet, AlexNet, VGG, ResNet
- ليش CNNs أحسن من MLPs للصور

### Transfer Learning
- استخدم نماذج مدرّبة مسبقاً (ResNet50, EfficientNet)
- Freeze layers, fine-tune top
- ⭐ **هذا اللي يستخدمه الناس فعلاً في الشغل، مو تدريب من الصفر.**

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

## المكتبات

- **torchvision** — datasets + models جاهزة
- **timm** — ٧٠٠+ نموذج CV مدرّب مسبقاً
- **albumentations** — augmentations سريعة
- **OpenCV** — image processing الكلاسيكي

---

## المصادر

- ⭐ **[CS231n — Stanford (Andrej Karpathy original)](http://cs231n.stanford.edu/)** — معيار العالم
- ⭐ **[Practical Deep Learning for Coders — fast.ai](https://course.fast.ai/)** — top-down approach
- **[KAUST Academy CV Course](https://academy.kaust.edu.sa/)** — لو سعودي، هذا الخيار الأنسب
- [PyTorch Vision Tutorials](https://pytorch.org/vision/stable/index.html)

---

## التحدي

استخدم Transfer Learning مع ResNet50 لتصنيف dataset من اختيارك ([ChestX-ray, Cats vs Dogs, Custom](https://www.kaggle.com/datasets)). ارفع النموذج على Hugging Face Hub.

---

[**← الأسبوع ٩**](../week-09-neural-networks/) · [**الأسبوع ١١ →**](../week-11-nlp-llms/)

</div>
