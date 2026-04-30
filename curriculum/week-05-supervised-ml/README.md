# Week 5 — Supervised Machine Learning

> **This week's goal:** Understand the difference between Regression and Classification, and train your first model.

---

## Core Concepts

- **Supervised Learning:** you have `X` (features) and `y` (target). You learn the function `f(X) → y`.
- **Regression:** `y` is a continuous number (e.g., house price).
- **Classification:** `y` is a category (e.g., survived/didn't survive, spam/not spam).
- **Train/Test Split:** 80/20 is typical. Don't forget `random_state` for reproducibility.

---

## Algorithms You Learn This Week

### Regression
- **Linear Regression** — the foundation. Understand it deeply.
- **Ridge & Lasso** — Linear Regression with regularization.

### Classification
- **Logistic Regression** — classification despite the name (historical).
- **Decision Trees** — easy to interpret.
- **Random Forest** — an ensemble of decision trees. Best baseline for most problems.
- **K-Nearest Neighbors (KNN)** — the simplest. Learn it to understand its limitations.

> **Note:** XGBoost / LightGBM are deferred to Week 7.

---

## Core Code (memorize this)

```python
from sklearn.model_selection import train_test_split
from sklearn.ensemble import RandomForestClassifier
from sklearn.metrics import accuracy_score

X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42
)

model = RandomForestClassifier(n_estimators=100, random_state=42)
model.fit(X_train, y_train)

preds = model.predict(X_test)
print(accuracy_score(y_test, preds))
```

---

## Resources

- ⭐ **[Scikit-learn User Guide](https://scikit-learn.org/stable/user_guide.html)** — your reference forever. Read Sections 1.1, 1.4, 1.10, 1.11.
- ⭐ **[StatQuest — Josh Starmer](https://www.youtube.com/@statquest)** — the best channel for ML with intuition.
- **[Hands-On ML with Scikit-Learn — Aurélien Géron (Book)](https://www.oreilly.com/library/view/hands-on-machine-learning/9781098125967/)** — ⭐⭐⭐ the book everyone recommends. Read Chapters 1–4.

---

## Challenge

Work on the [Kaggle Titanic Competition](https://www.kaggle.com/c/titanic). Try 3 different models and compare them. Submit your score and get a ranking.

---

[**← Week 4**](../week-04-visualization/) · [**Week 6 →**](../week-06-model-evaluation/)

