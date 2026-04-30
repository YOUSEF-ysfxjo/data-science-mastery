<div dir="rtl">

# الأسبوع ٧ — هندسة الميزات
## Week 7 — Feature Engineering

> **القاعدة الذهبية:** Features قوية + نموذج بسيط > Features ضعيفة + نموذج معقد.

---

## ماذا تتعلم

### Encoding
- One-Hot Encoding — للـ categorical غير مرتب
- Label Encoding — للـ ordinal
- Target Encoding — قوي لكن يحتاج cross-validation عشان ما يحصل leakage
- Binary Encoding — لما عندك categories كثيرة

### Scaling
- StandardScaler (mean=0, std=1) — للنماذج اللي تعتمد على المسافة
- MinMaxScaler [0, 1] — للـ neural networks
- RobustScaler — لما عندك outliers

### Feature Creation
- Interaction features (x1 × x2)
- Polynomial features
- Date features (day of week, month, is_weekend)
- Text features (length, word count, sentiment)
- Aggregations (mean salary per city, count of orders per user)

### Feature Selection
- Correlation analysis
- Recursive Feature Elimination (RFE)
- Feature importance من Random Forest / XGBoost
- SHAP values

---

## Gradient Boosting — النجوم

- **XGBoost** — كان ملك Kaggle لسنوات
- **LightGBM** — أسرع، أحسن للـ datasets الكبيرة
- **CatBoost** — يتعامل مع categorical تلقائياً

نصيحة: ابدأ بـ LightGBM في أكثر المشاريع.

---

## Pipelines

```python
from sklearn.pipeline import Pipeline
from sklearn.compose import ColumnTransformer
from sklearn.preprocessing import StandardScaler, OneHotEncoder

preprocessor = ColumnTransformer([
    ("num", StandardScaler(), numeric_cols),
    ("cat", OneHotEncoder(), categorical_cols),
])

pipeline = Pipeline([
    ("preprocess", preprocessor),
    ("model", LGBMClassifier()),
])

pipeline.fit(X_train, y_train)
```

استخدم Pipelines دايماً. تمنع leakage وتسهّل deployment.

---

## المصادر

- ⭐ [Feature Engineering A–Z (Kaggle Course)](https://www.kaggle.com/learn/feature-engineering)
- [Feature Engineering for ML — Alice Zheng (Book)](https://www.oreilly.com/library/view/feature-engineering-for/9781491953235/)
- [SHAP Documentation](https://shap.readthedocs.io/)

---

## التحدي

ارجع للـ Titanic. أنشئ ٥ features جديدة (مثل `Title` من الاسم، `IsAlone`, `AgeGroup`). قارن النتائج قبل وبعد.

---

[**← الأسبوع ٦**](../week-06-model-evaluation/) · [**الأسبوع ٨ →**](../week-08-unsupervised/)

</div>
