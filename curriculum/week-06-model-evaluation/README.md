<div dir="rtl">

# الأسبوع ٦ — تقييم النماذج
## Week 6 — Model Evaluation

> **سرّ صناعي:** أكثر النماذج "عالية الدقة" في portfolios المبتدئين، عندها مشاكل تقييم. هذا الأسبوع يحميك من الإحراج في المقابلات.

---

## ليش Accuracy ما يكفي؟

تخيّل dataset فيه ٩٩٪ غير مرضى و١٪ مرضى. نموذج يقول "كلكم سليمين" يطلع accuracy = 99%.
**لا تستخدم accuracy لما الفئات غير متوازنة.**

---

## المقاييس اللي لازم تعرفها

### Classification
- **Confusion Matrix** — TP, FP, TN, FN. **افهمها بعمق.**
- **Precision** = TP / (TP + FP) — "كم من المتوقعين موجبين فعلاً موجبين"
- **Recall (Sensitivity)** = TP / (TP + FN) — "كم من الموجبين الحقيقيين أمسكناهم"
- **F1 Score** = harmonic mean of P and R
- **ROC-AUC** — لا يعتمد على threshold
- **Precision-Recall Curve** — أحسن من ROC للـ imbalanced data

### Regression
- **MAE, MSE, RMSE** — افهم الفرق
- **R²** — كم من التباين شرحه النموذج
- **MAPE** — للـ business reports

---

## Cross-Validation

- ليش train/test split واحد ما يكفي
- K-Fold CV (افتراضياً K=5)
- Stratified K-Fold للـ imbalanced classes
- Time Series CV (لا تستخدم K-Fold عادي على بيانات زمنية)

---

## المفاهيم الذهبية

- **Overfitting** — train accuracy عالي، test accuracy منخفض
- **Underfitting** — كلاهما منخفض
- **Bias-Variance Tradeoff** — مفهوم لازم تشرحه في أي مقابلة
- **Data Leakage** — لما test data تسرّب للـ training (الكارثة الصامتة)

---

## المصادر

- ⭐ [Scikit-learn — Model Evaluation Guide](https://scikit-learn.org/stable/modules/model_evaluation.html)
- [StatQuest — ROC and AUC](https://www.youtube.com/watch?v=4jRBRDbJemM)
- [How to evaluate ML models — Jason Brownlee](https://machinelearningmastery.com/)

---

## التحدي

ارجع لنموذج الأسبوع ٥. أعد تقييمه بـ ٥ مقاييس مختلفة. اطلع confusion matrix. حدد فئة من الفئات النموذج يفشل فيها بشكل خاص.

---

[**← الأسبوع ٥**](../week-05-supervised-ml/) · [**الأسبوع ٧ →**](../week-07-feature-engineering/)

</div>
