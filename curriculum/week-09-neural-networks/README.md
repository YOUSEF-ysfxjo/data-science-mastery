<div dir="rtl">

# الأسبوع ٩ — الشبكات العصبية
## Week 9 — Neural Networks

> **الانتقال الكبير:** من scikit-learn إلى PyTorch. مرحباً بك في deep learning.

---

## ماذا تتعلم

### المفاهيم
- Perceptron → Multi-Layer Perceptron (MLP)
- Activation functions: ReLU, Sigmoid, Tanh, Softmax
- Forward pass + Backpropagation
- Loss functions: MSE, Cross-Entropy
- Optimizers: SGD, Adam
- Batch size, epochs, learning rate

### الكود
- بناء NN بـ PyTorch من الصفر
- Tensors, autograd, `nn.Module`
- Training loop يدوي (مهم تفهمه)
- GPU usage (`.to(device)`)

---

## ليش PyTorch مو TensorFlow؟

- PyTorch صار المعيار الأكاديمي والصناعي (٢٠٢٠+).
- API أبسط، debugging أسهل.
- Hugging Face مبني عليه.
- TensorFlow ما زال موجود لكن خصوصاً للـ production الكبير وKeras.

ابدأ بـ PyTorch. تعلّم TensorFlow لاحقاً لو احتجت.

---

## Template أساسي للـ Training Loop

```python
import torch
import torch.nn as nn

model = MyNet().to(device)
criterion = nn.CrossEntropyLoss()
optimizer = torch.optim.Adam(model.parameters(), lr=1e-3)

for epoch in range(epochs):
    for X_batch, y_batch in train_loader:
        X_batch, y_batch = X_batch.to(device), y_batch.to(device)
        
        optimizer.zero_grad()
        out = model(X_batch)
        loss = criterion(out, y_batch)
        loss.backward()
        optimizer.step()
```

---

## المصادر

- ⭐ **[PyTorch Official Tutorials](https://pytorch.org/tutorials/)** — ابدأ من "Learn the Basics"
- ⭐ **[Andrej Karpathy — Neural Networks: Zero to Hero](https://www.youtube.com/playlist?list=PLAqhIrjkxbuWI23v9cThsA9GvCAUhRvKZ)** — أحسن سلسلة فيديوهات في DL، فترة.
- **[Deep Learning Book — Goodfellow (Chapters 6, 7, 8)](https://www.deeplearningbook.org/)** — مرجع نظري.
- **[3Blue1Brown — Neural Networks](https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi)** — intuition بصري.

---

## التحدي

دربّ MLP بـ PyTorch على [MNIST dataset](http://yann.lecun.com/exdb/mnist/). الهدف: ٩٧٪+ accuracy. تعلّم Tensorboard لمتابعة التدريب.

---

[**← الأسبوع ٨**](../week-08-unsupervised/) · [**الأسبوع ١٠ →**](../week-10-computer-vision/)

</div>
