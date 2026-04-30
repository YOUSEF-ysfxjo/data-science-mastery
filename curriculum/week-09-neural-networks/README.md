# Week 9 — Neural Networks

> **The big transition:** from scikit-learn to PyTorch. Welcome to deep learning.

---

## What You Learn

### Concepts
- Perceptron → Multi-Layer Perceptron (MLP)
- Activation functions: ReLU, Sigmoid, Tanh, Softmax
- Forward pass + Backpropagation
- Loss functions: MSE, Cross-Entropy
- Optimizers: SGD, Adam
- Batch size, epochs, learning rate

### Code
- Building a neural network with PyTorch from scratch
- Tensors, autograd, `nn.Module`
- Manual training loop (important to understand)
- GPU usage (`.to(device)`)

---

## Why PyTorch and Not TensorFlow?

- PyTorch has become the academic and industry standard (2020+).
- Simpler API, easier debugging.
- Hugging Face is built on it.
- TensorFlow still exists, mainly for large-scale production and Keras.

Start with PyTorch. Learn TensorFlow later if you need it.

---

## Basic Training Loop Template

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

## Resources

- ⭐ **[PyTorch Official Tutorials](https://pytorch.org/tutorials/)** — start from "Learn the Basics"
- ⭐ **[Andrej Karpathy — Neural Networks: Zero to Hero](https://www.youtube.com/playlist?list=PLAqhIrjkxbuWI23v9cThsA9GvCAUhRvKZ)** — the best DL video series, period.
- **[Deep Learning Book — Goodfellow (Chapters 6, 7, 8)](https://www.deeplearningbook.org/)** — theoretical reference.
- **[3Blue1Brown — Neural Networks](https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi)** — visual intuition.

---

## Challenge

Train an MLP with PyTorch on the [MNIST dataset via `torchvision.datasets.MNIST`](https://pytorch.org/vision/stable/generated/torchvision.datasets.MNIST.html). Goal: 97%+ accuracy. Learn TensorBoard to monitor training.

---

[**← Week 8**](../week-08-unsupervised/) · [**Week 10 →**](../week-10-computer-vision/)

