<div dir="rtl">

# 💼 التحضير للمقابلات — Interview Prep

أكثر مقابلات Data Science في السوق السعودي والعربي تتركز على ٤ محاور.

---

## ١. SQL — لا غنى عنه

### المواضيع
- Joins (INNER, LEFT, RIGHT, FULL, SELF)
- GROUP BY + HAVING + aggregations
- Window functions: ROW_NUMBER, RANK, LAG, LEAD
- CTEs (`WITH`)
- Subqueries vs JOINs
- Indexing basics

### الموارد
- ⭐ [Mode SQL Tutorial](https://mode.com/sql-tutorial/) — مجاني، شامل
- ⭐ [StrataScratch](https://www.stratascratch.com/) — أسئلة من Amazon, Google, Meta
- [LeetCode SQL 50](https://leetcode.com/studyplan/top-sql-50/)
- [DataLemur](https://datalemur.com/)

### أسئلة كلاسيكية
1. ثاني أعلى راتب
2. المنتجات اللي زاد طلبها شهرياً
3. نسبة المستخدمين النشطين شهرياً (MAU%)
4. cumulative sum لكل category

---

## ٢. Python + Pandas

أكثر شيء بيسألونك:
- اكتب function تحسب moving average بدون استخدام `rolling()`
- اقلب long → wide format
- detect outliers بـ IQR
- اعمل lifetime value لكل عميل من جدول طلبات

---

## ٣. Machine Learning

### مفاهيم لازم تشرحها بدون تردد

| المفهوم | المدة |
|---|---|
| Bias-Variance Tradeoff | ٦٠ ث |
| Overfitting + ٣ حلول | ٤٥ ث |
| Cross-Validation | ٣٠ ث |
| ROC vs PR Curve | ٤٥ ث |
| Bagging vs Boosting | ٤٥ ث |
| Gradient Descent + variants | ٦٠ ث |
| Regularization (L1 vs L2) | ٤٥ ث |
| Curse of Dimensionality | ٣٠ ث |
| Class Imbalance — ٤ حلول | ٦٠ ث |

### الموارد
- ⭐ [Machine Learning Interviews — Chip Huyen](https://huyenchip.com/ml-interviews-book/) — مجاني
- [Data Science Interviews — Alexey Grigorev](https://github.com/alexeygrigorev/data-science-interviews)

---

## ٤. Case Studies (CRISP-DM)

استخدم هذا الإطار لأي سؤال تطبيقي:

1. **Business Understanding** — وش المشكلة من زاوية الـ business؟
2. **Data Understanding** — وش متاح؟
3. **Data Preparation** — كيف ننظف؟
4. **Modeling** — وش النماذج المرشحة؟
5. **Evaluation** — كيف نعرف نجح؟
6. **Deployment** — كيف نوصلها للمستخدم؟

### مثال
> "كيف تبني نموذج تصنيف شكاوى لتطبيق سعودي؟"

اشرح كل ٦ خطوات. ركز على:
- جمع البيانات (web scraping؟ annotated؟)
- العربية (dialects, code-mixing)
- اختيار MARBERT vs AraBERT
- المقاييس (F1 macro للـ imbalanced)
- API بـ FastAPI + Docker

---

## ✅ Portfolio Checklist قبل المقابلة

- [ ] GitHub profile فيه README واضح
- [ ] ٣ مشاريع pinned، الأفضل أولاً
- [ ] كل مشروع: README جيد + screenshots
- [ ] LinkedIn متوافق مع GitHub
- [ ] لو في paper: link مباشر
- [ ] HF models بـ Model Cards كاملة
- [ ] جاهز تشرح كل مشروع في ٦٠ ث

</div>
