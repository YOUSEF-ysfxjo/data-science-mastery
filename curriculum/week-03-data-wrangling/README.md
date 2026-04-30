<div dir="rtl">

# الأسبوع ٣ — معالجة البيانات بـ Pandas
## Week 3 — Data Wrangling

> **حقيقة:** ٧٠٪ من وقت Data Scientist في تنظيف البيانات، مو في بناء النماذج. هذا الأسبوع يعلّمك المهارة اللي ما تنشرها على LinkedIn بس تحدد قيمتك في الشغل.

---

## ماذا تتعلم

### يوم ١: قراءة البيانات من كل مكان
- CSV, Excel, JSON, Parquet
- SQL databases (`pd.read_sql`)
- APIs (`requests` + `pd.json_normalize`)
- Web scraping بـ Pandas (`pd.read_html`)

### يوم ٢: التعامل مع Missing Values
- متى تحذف؟ متى تعوّض؟
- `fillna` بـ mean/median/mode
- `KNN imputation`
- إنشاء feature `is_missing` (المعلومة في الفقد نفسه أحياناً)

### يوم ٣: Merging, Joining, Concatenation
- `merge` (inner, left, right, outer) — افهم الفرق
- `concat` للـ stacking
- `join` على index
- مشاكل الـ duplicates بعد الـ merge

### يوم ٤: Transformations
- `apply`, `map`, `applymap` — متى أيهم
- `pd.get_dummies` للـ categorical
- `pd.cut` و `pd.qcut` للـ binning
- التعامل مع التواريخ (`pd.to_datetime`, `.dt` accessors)

### يوم ٥: Group operations المتقدمة
- `groupby` + `agg` بدوال متعددة
- `transform` (يرجع نفس الحجم) vs `agg`
- `pivot_table` و `crosstab`
- Window functions: `rolling`, `expanding`

### يوم ٦: الأداء
- متى تستخدم `vectorization` بدل `apply`
- `dtype` optimization (`int64` → `int8` لو ينفع)
- `chunksize` للملفات الكبيرة
- Polars (بديل Pandas الأسرع — تعرّف عليه)

### يوم ٧: التحدي الأسبوعي

---

## المصادر المختارة

### الأساسي ⭐
**[Pandas in Action — Boris Paskhaver](https://www.manning.com/books/pandas-in-action)** — كتاب مدفوع لكنه يستاهل. لو ما تقدر، الفصول الأولى في Python Data Science Handbook.

### للممارسة
**[Pandas Exercises (GitHub)](https://github.com/guipsamora/pandas_exercises)** — ٢٠٠+ تمرين متدرّج. **هذا أهم رابط في الأسبوع.**

### بالعربي
**[Hesham Asem — Pandas](https://www.youtube.com/@HeshamAsem)** — شروحات عملية.

---

## الفخاخ الشائعة

```python
# ❌ خطأ: يعطي SettingWithCopyWarning أحياناً
df[df["age"] > 25]["salary"] = 5000

# ✅ صحيح
df.loc[df["age"] > 25, "salary"] = 5000

# ❌ بطيء جداً على dataframes كبيرة
df["new"] = df["col"].apply(lambda x: x * 2)

# ✅ أسرع ١٠٠×
df["new"] = df["col"] * 2

# ❌ يستهلك ذاكرة كثير
df = pd.read_csv("huge.csv")

# ✅ للملفات الضخمة
chunks = pd.read_csv("huge.csv", chunksize=10000)
for chunk in chunks:
    process(chunk)
```

---

## التحدي الأسبوعي

اشتغل على dataset حقيقي متسخ — اقترحنا [NYC 311 Service Requests](https://data.cityofnewyork.us/Social-Services/311-Service-Requests-from-2010-to-Present/erm2-nwhp).

١. حمّل sample (١ مليون صف).
٢. حدد الأعمدة المهمة (٧٠٪ من الأعمدة لا تحتاجها).
٣. نظف missing values.
٤. حوّل التواريخ.
٥. اعمل ٥ groupby insights.
٦. وثّق الخطوات في notebook.

---

[**← الأسبوع ٢**](../week-02-math-for-ds/) · [**الأسبوع ٤ →**](../week-04-visualization/)

</div>
