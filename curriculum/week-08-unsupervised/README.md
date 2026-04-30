<div dir="rtl">

# الأسبوع ٨ — التعلم غير الموجَّه
## Week 8 — Unsupervised Learning

> **متى تستخدمه:** ما عندك labels. تبي تكتشف بنية مخفية في البيانات.

---

## Clustering

- **K-Means** — الأشهر. اختر K بـ Elbow method أو Silhouette.
- **DBSCAN** — للأشكال غير الكروية + يكتشف outliers.
- **Hierarchical Clustering** — يعطيك dendrogram. مفيد لما ما تعرف K.
- **Gaussian Mixture Models (GMM)** — soft clustering (احتمالات).

## Dimensionality Reduction

- **PCA (Principal Component Analysis)** — الأساس. linear projection.
- **t-SNE** — للـ visualization فقط (لا تستخدمه قبل ML model).
- **UMAP** — أحسن من t-SNE في أكثر الحالات.

## Anomaly Detection

- Isolation Forest
- One-Class SVM
- Autoencoders (موّجل لـ Deep Learning)

---

## متى تستخدم وش

| السيناريو | الحل |
|---|---|
| تجزئة عملاء (segmentation) | K-Means |
| كشف احتيال (fraud) | Isolation Forest |
| تقليل أبعاد قبل classification | PCA |
| visualizing high-dim data | UMAP |

---

## المصادر

- ⭐ [Scikit-learn — Clustering](https://scikit-learn.org/stable/modules/clustering.html)
- [StatQuest — PCA Step by Step](https://www.youtube.com/watch?v=FgakZw6K1QQ)
- [UMAP Documentation](https://umap-learn.readthedocs.io/)

---

## التحدي

استخدم [Mall Customer Segmentation Dataset](https://www.kaggle.com/vjchoudhary7/customer-segmentation-tutorial-in-python). جرّب K-Means و DBSCAN. ارسم clusters بـ PCA.

---

[**← الأسبوع ٧**](../week-07-feature-engineering/) · [**الأسبوع ٩ →**](../week-09-neural-networks/)

</div>
