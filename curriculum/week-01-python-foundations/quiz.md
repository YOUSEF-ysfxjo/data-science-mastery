<div dir="rtl">

# Quiz — الأسبوع ١

جاوب بدون فتح المراجع. الإجابات تحت (مغلقة).

---

**١.** ما الفرق بين `df.loc[0]` و `df.iloc[0]`؟

<details><summary>الإجابة</summary>

`loc` يستخدم الـ **labels** (أسماء الـ index)، بينما `iloc` يستخدم الـ **positions** (الأرقام). لو الـ index ما بدأ من ٠، النتائج تختلف.
</details>

---

**٢.** ليش `np.array` أسرع من `list` في العمليات الحسابية؟

<details><summary>الإجابة</summary>

NumPy arrays مخزّنة في الذاكرة كـ **contiguous block** بنوع موحّد، فالـ CPU يقدر يستخدم vectorization (SIMD). Lists فيها pointers لـ Python objects متفرقة.
</details>

---

**٣.** وش الفرق بين `df.dropna()` و `df.dropna(inplace=True)`؟

<details><summary>الإجابة</summary>

الأول يرجع **DataFrame جديد** ما يعدّل الأصلي. الثاني يعدّل الأصلي ويرجع `None`. أكثر developers Pandas يفضّلون الأول (`df = df.dropna()`) لأنه أوضح.
</details>

---

**٤.** كيف تطلع متوسط الراتب لكل مدينة من DataFrame فيه أعمدة `city`, `salary`؟

<details><summary>الإجابة</summary>

```python
df.groupby("city")["salary"].mean()
```
</details>

---

**٥.** متى تستخدم `.copy()`؟

<details><summary>الإجابة</summary>

لما تبي تعمل DataFrame جديد ما يأثر على الأصلي. خاصة لو راح تعدّل عليه. بدون `.copy()` ممكن تحصل `SettingWithCopyWarning` في Pandas.
</details>

</div>
