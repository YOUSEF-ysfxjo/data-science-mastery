# Week 8 — Unsupervised Learning

> **When to use it:** You have no labels. You want to discover hidden structure in your data.

---

## Clustering

- **K-Means** — the most popular. Choose K with the Elbow method or Silhouette score.
- **DBSCAN** — for non-spherical shapes + detects outliers.
- **Hierarchical Clustering** — gives you a dendrogram. Useful when you don't know K.
- **Gaussian Mixture Models (GMM)** — soft clustering (probabilities).

## Dimensionality Reduction

- **PCA (Principal Component Analysis)** — the foundation. Linear projection.
- **t-SNE** — for visualization only (don't use before an ML model).
- **UMAP** — better than t-SNE in most cases.

## Anomaly Detection

- Isolation Forest
- One-Class SVM
- Autoencoders (deferred to Deep Learning)

---

## When to Use What

| Scenario | Solution |
|---|---|
| Customer segmentation | K-Means |
| Fraud detection | Isolation Forest |
| Dimensionality reduction before classification | PCA |
| Visualizing high-dimensional data | UMAP |

---

## Resources

- ⭐ [Scikit-learn — Clustering](https://scikit-learn.org/stable/modules/clustering.html)
- [StatQuest — PCA Step by Step](https://www.youtube.com/watch?v=FgakZw6K1QQ)
- [UMAP Documentation](https://umap-learn.readthedocs.io/)

---

## Challenge

Use the [Mall Customer Segmentation Dataset](https://www.kaggle.com/vjchoudhary7/customer-segmentation-tutorial-in-python). Try K-Means and DBSCAN. Plot clusters using PCA.

---

[**← Week 7**](../week-07-feature-engineering/) · [**Week 9 →**](../week-09-neural-networks/)

