# 💼 Interview Prep

Most Data Science interviews in the Saudi and Arab market focus on 4 areas.

---

## 1. SQL — Non-Negotiable

### Topics
- Joins (INNER, LEFT, RIGHT, FULL, SELF)
- GROUP BY + HAVING + aggregations
- Window functions: ROW_NUMBER, RANK, LAG, LEAD
- CTEs (`WITH`)
- Subqueries vs JOINs
- Indexing basics

### Resources
- ⭐ [Mode SQL Tutorial](https://mode.com/sql-tutorial/) — free, comprehensive
- ⭐ [StrataScratch](https://www.stratascratch.com/) — questions from Amazon, Google, Meta
- [LeetCode SQL 50](https://leetcode.com/studyplan/top-sql-50/)
- [DataLemur](https://datalemur.com/)

### Classic Questions
1. Second highest salary
2. Products with increasing monthly demand
3. Monthly active user ratio (MAU%)
4. Cumulative sum per category

---

## 2. Python + Pandas

Most common asks:
- Write a function that computes a moving average without using `rolling()`
- Pivot from long → wide format
- Detect outliers with IQR
- Compute lifetime value per customer from an orders table

---

## 3. Machine Learning

### Concepts You Must Explain Without Hesitation

| Concept | Duration |
|---|---|
| Bias-Variance Tradeoff | 60 sec |
| Overfitting + 3 solutions | 45 sec |
| Cross-Validation | 30 sec |
| ROC vs PR Curve | 45 sec |
| Bagging vs Boosting | 45 sec |
| Gradient Descent + variants | 60 sec |
| Regularization (L1 vs L2) | 45 sec |
| Curse of Dimensionality | 30 sec |
| Class Imbalance — 4 solutions | 60 sec |

### Resources
- ⭐ [Machine Learning Interviews — Chip Huyen](https://huyenchip.com/ml-interviews-book/) — free
- [Data Science Interviews — Alexey Grigorev](https://github.com/alexeygrigorev/data-science-interviews)

---

## 4. Case Studies (CRISP-DM)

Use this framework for any applied question:

1. **Business Understanding** — what is the problem from a business perspective?
2. **Data Understanding** — what data is available?
3. **Data Preparation** — how do we clean it?
4. **Modeling** — what candidate models?
5. **Evaluation** — how do we know it worked?
6. **Deployment** — how does it reach the user?

### Example
> "How would you build a complaint classification model for a Saudi app?"

Walk through all 6 steps. Focus on:
- Data collection (web scraping? annotated?)
- Arabic (dialects, code-mixing)
- Choosing MARBERT vs AraBERT
- Metrics (F1 macro for imbalanced)
- API with FastAPI + Docker

---

## ✅ Portfolio Checklist Before the Interview

- [ ] GitHub profile with a clear README
- [ ] 3 pinned projects, best one first
- [ ] Each project: good README + screenshots
- [ ] LinkedIn aligned with GitHub
- [ ] If there's a paper: direct link
- [ ] HF models with complete Model Cards
- [ ] Ready to explain every project in 60 seconds

