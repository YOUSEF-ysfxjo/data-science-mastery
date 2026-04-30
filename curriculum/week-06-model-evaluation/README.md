# Week 6 — Model Evaluation

> **Industry secret:** Most "high-accuracy" models in beginner portfolios have evaluation problems. This week protects you from embarrassment in interviews.

---

## Why Accuracy Isn't Enough

Imagine a dataset where 99% are healthy and 1% are sick. A model that says "everyone is healthy" gets accuracy = 99%.
**Don't use accuracy when classes are imbalanced.**

---

## Metrics You Must Know

### Classification
- **Confusion Matrix** — TP, FP, TN, FN. **Understand it deeply.**
- **Precision** = TP / (TP + FP) — "of the predicted positives, how many are actually positive"
- **Recall (Sensitivity)** = TP / (TP + FN) — "of the actual positives, how many did we catch"
- **F1 Score** = harmonic mean of Precision and Recall
- **ROC-AUC** — threshold-independent
- **Precision-Recall Curve** — better than ROC for imbalanced data

### Regression
- **MAE, MSE, RMSE** — understand the difference
- **R²** — how much variance the model explains
- **MAPE** — for business reports

---

## Cross-Validation

- Why a single train/test split isn't enough
- K-Fold CV (default K=5)
- Stratified K-Fold for imbalanced classes
- Time Series CV (don't use regular K-Fold on time-series data)

---

## Golden Concepts

- **Overfitting** — high train accuracy, low test accuracy
- **Underfitting** — both are low
- **Bias-Variance Tradeoff** — a concept you must explain in any interview
- **Data Leakage** — when test data leaks into training (the silent disaster)

---

## Resources

- ⭐ [Scikit-learn — Model Evaluation Guide](https://scikit-learn.org/stable/modules/model_evaluation.html)
- [StatQuest — ROC and AUC](https://www.youtube.com/watch?v=4jRBRDbJemM)
- [How to evaluate ML models — Jason Brownlee](https://machinelearningmastery.com/)

---

## Challenge

Go back to Week 5's model. Re-evaluate it with 5 different metrics. Plot the confusion matrix. Identify which class the model fails on most.

---

[**← Week 5**](../week-05-supervised-ml/) · [**Week 7 →**](../week-07-feature-engineering/)

