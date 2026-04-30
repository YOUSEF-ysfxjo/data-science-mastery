<div dir="rtl">

# الأسبوع ١ — أساسيات Python لعلم البيانات
## Week 1 — Python Foundations for Data Science

> **الهدف:** بعد هذا الأسبوع، تقدر تفتح ملف بيانات، تقرأه بـ NumPy/Pandas، وتطلع منه إحصاءات أساسية بدون ما تجوجل كل سطر.

---

## ليش Python؟ — Why Python?

علم البيانات يحتاج لغة:
- سهلة الكتابة (تركز على المشكلة، مو على الـ syntax)
- عندها مكتبات قوية (NumPy, Pandas, Scikit-learn, PyTorch)
- مجتمع ضخم (إجابات لكل سؤال)

R لغة ممتازة بس Python غلبت في الصناعة. R يبقى مفيد للإحصاء الأكاديمي.

---

## ماذا تتعلم هذا الأسبوع

### يوم ١–٢: Python أساسي (لو ما تعرف)
- Variables, types, lists, dicts, tuples, sets
- Control flow: `if`, `for`, `while`
- Functions, scope, `*args`, `**kwargs`
- List comprehensions — **مهم جداً**
- File I/O: قراءة وكتابة ملفات

> **لو تعرف Python أصلاً:** اقفز لليوم الثالث.

### يوم ٣: NumPy
- `np.array` — ليش هو أسرع من list؟
- Vectorization (لا تستخدم `for` على arrays)
- Broadcasting
- Indexing & slicing
- Random numbers (`np.random`)

### يوم ٤–٥: Pandas (مقدمة)
- `Series` و `DataFrame`
- قراءة CSV, Excel, JSON
- `.head()`, `.info()`, `.describe()`
- Filtering rows, selecting columns
- `.groupby()` المبدئي

### يوم ٦: Jupyter + Git
- ليش Jupyter notebooks للاستكشاف
- VS Code + extension للـ notebooks (أحسن من Jupyter Lab لأكثر الناس)
- Git أساسي: `init`, `add`, `commit`, `push`
- ربط GitHub بحسابك

### يوم ٧: التحدي الأسبوعي
[انظر `exercise.md`](exercise.md)

---

## المصادر المختارة (٣ بس، مو ١٥)

### المصدر الأساسي ⭐
**[Python Data Science Handbook — Jake VanderPlas](https://jakevdp.github.io/PythonDataScienceHandbook/)** — مجاني، notebooks قابلة للتشغيل في Colab. اقرأ الفصول 1–3.

### للمبتدئين تماماً
**[Python for Everybody — د. Charles Severance (Coursera)](https://www.coursera.org/specializations/python)** — مجاني للمراجعة. خذ Course 1 + 2 إذا Python جديد عليك.

### بالعربي
**[قناة محمد ضياء على يوتيوب — Python بالعربي](https://www.youtube.com/@MhdZiyaa)** — شرح هادئ وواضح.

> **لا تشتت نفسك.** اختار واحد والتزم. الباقي ضوضاء.

---

## أوامر Pandas اللي بتستخدمها كل يوم

```python
import pandas as pd

df = pd.read_csv("data.csv")     # قراءة
df.head()                         # أول ٥ صفوف
df.info()                         # أنواع الأعمدة + null counts
df.describe()                     # إحصاءات عددية
df.shape                          # (rows, columns)
df.columns                        # أسماء الأعمدة

df["age"]                         # عمود واحد (Series)
df[["age", "salary"]]             # أعمدة متعددة
df[df["age"] > 25]                # filter
df.groupby("city")["salary"].mean()  # تجميع
```

احفظ هذي ال١٠ أسطر. هي ٨٠٪ من شغلك اليومي.

---

## بعد ما تخلص

- ✅ ارفع notebook التحدي على GitHub في repo اسمه `ds-week-01`
- ✅ اكتب README.md بسيط: وش سويت، وش تعلمت، وش الصعوبات
- ✅ شارك الـ repo في LinkedIn — `#100DaysOfDataScience`
- ✅ راجع [`quiz.md`](quiz.md) قبل ما تنتقل للأسبوع ٢

---

## أخطاء شائعة هذا الأسبوع

| الخطأ | الحل |
|---|---|
| تستخدم `for loop` على NumPy array | استخدم vectorized operations |
| تنسى `inplace=True` أو لا تحفظ النتيجة | `df = df.dropna()` بدل `df.dropna()` |
| تخلط بين `.loc[]` و `.iloc[]` | `loc` للأسماء، `iloc` للأرقام |
| تعدل DataFrame وأنت تكرر عليه | استخدم `.copy()` لما تشك |

---

[**← المنهج الرئيسي**](../README.md) · [**التمرين →**](exercise.md) · [**الأسبوع ٢ →**](../week-02-math-for-ds/)

</div>
