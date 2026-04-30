# Week 7 — Feature Engineering

> **The golden rule:** Strong features + simple model > weak features + complex model.

---

## What You Learn

### Encoding
- One-Hot Encoding — for unordered categorical data
- Label Encoding — for ordinal data
- Target Encoding — powerful but needs cross-validation to avoid leakage
- Binary Encoding — for high-cardinality categories

### Scaling
- StandardScaler (mean=0, std=1) — for distance-based models
- MinMaxScaler [0, 1] — for neural networks
- RobustScaler — when you have outliers

### Feature Creation
- Interaction features (x1 × x2)
- Polynomial features
- Date features (day of week, month, is_weekend)
- Text features (length, word count, sentiment)
- Aggregations (mean salary per city, count of orders per user)

### Feature Selection
- Correlation analysis
- Recursive Feature Elimination (RFE)
- Feature importance from Random Forest / XGBoost
- SHAP values

---

## Gradient Boosting — The Stars

- **XGBoost** — was king of Kaggle for years
- **LightGBM** — faster, better for large datasets
- **CatBoost** — handles categorical data automatically

Tip: Start with LightGBM in most projects.

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

Always use Pipelines. They prevent leakage and make deployment easier.

---

## Resources

- ⭐ [Feature Engineering A–Z (Kaggle Course)](https://www.kaggle.com/learn/feature-engineering)
- [Feature Engineering for ML — Alice Zheng (Book)](https://www.oreilly.com/library/view/feature-engineering-for/9781491953235/)
- [SHAP Documentation](https://shap.readthedocs.io/)

---

## Challenge

Go back to Titanic. Create 5 new features (e.g., `Title` from the name, `IsAlone`, `AgeGroup`). Compare results before and after.

---

[**← Week 6**](../week-06-model-evaluation/) · [**Week 8 →**](../week-08-unsupervised/)

