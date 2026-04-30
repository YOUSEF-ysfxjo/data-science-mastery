<div dir="rtl">

# الأسبوع ٥ — التعلم الموجَّه (Supervised ML)
## Week 5 — Supervised Machine Learning

> **هدفك هذا الأسبوع:** تفهم الفرق بين Regression و Classification، وتدرّب أول نموذج لك.

---

## المفاهيم الأساسية

- **Supervised Learning:** عندك `X` (features) و `y` (target). تتعلم الدالة `f(X) → y`.
- **Regression:** `y` رقم متصل (مثل سعر بيت).
- **Classification:** `y` فئة (مثل نجا/ما نجا، spam/not spam).
- **Train/Test Split:** ٨٠/٢٠ عادة. ولا تنس `random_state` للتكرار.

---

## الخوارزميات اللي تتعلمها هذا الأسبوع

### Regression
- **Linear Regression** — الأساس. افهمه بعمق.
- **Ridge & Lasso** — Linear Regression مع regularization.

### Classification
- **Logistic Regression** — classification لكن اسمه regression (موروث).
- **Decision Trees** — سهل التفسير.
- **Random Forest** — مجموعة decision trees. أحسن baseline في أكثر المسائل.
- **K-Nearest Neighbors (KNN)** — الأبسط. تعلّمه عشان تفهم limitations.

> **ملاحظة:** XGBoost / LightGBM موّجلين للأسبوع ٧.

---

## الكود الأساسي (احفظه)

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

## المصادر

- ⭐ **[Scikit-learn User Guide](https://scikit-learn.org/stable/user_guide.html)** — مرجعك للأبد. اقرأ Sections 1.1, 1.4, 1.10, 1.11.
- ⭐ **[StatQuest — Josh Starmer](https://www.youtube.com/@statquest)** — أحسن قناة لشرح ML بـ intuition.
- **[Hands-On ML with Scikit-Learn — Aurélien Géron (Book)](https://www.oreilly.com/library/view/hands-on-machine-learning/9781098125967/)** — ⭐⭐⭐ الكتاب اللي ينصح فيه الجميع. اقرأ Chapters 1–4.

---

## التحدي

اشتغل على [Kaggle Titanic Competition](https://www.kaggle.com/c/titanic). جرّب ٣ نماذج وقارن. ارفع نتيجتك واحصل على ranking.

---

[**← الأسبوع ٤**](../week-04-visualization/) · [**الأسبوع ٦ →**](../week-06-model-evaluation/)

</div>
