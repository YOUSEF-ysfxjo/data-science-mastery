# Quiz — Week 1

Answer without opening any references. Answers are below (collapsed).

---

**1.** What is the difference between `df.loc[0]` and `df.iloc[0]`?

<details><summary>Answer</summary>

`loc` uses **labels** (index names), while `iloc` uses **positions** (integer indices). If the index doesn't start at 0, the results will differ.
</details>

---

**2.** Why is `np.array` faster than a `list` for numerical operations?

<details><summary>Answer</summary>

NumPy arrays are stored in memory as a **contiguous block** of a uniform type, so the CPU can use vectorization (SIMD). Lists contain pointers to scattered Python objects.
</details>

---

**3.** What is the difference between `df.dropna()` and `df.dropna(inplace=True)`?

<details><summary>Answer</summary>

The first returns a **new DataFrame** without modifying the original. The second modifies the original and returns `None`. Most Pandas developers prefer the first form (`df = df.dropna()`) because it's more explicit.
</details>

---

**4.** How do you get the average salary per city from a DataFrame with `city` and `salary` columns?

<details><summary>Answer</summary>

```python
df.groupby("city")["salary"].mean()
```
</details>

---

**5.** When should you use `.copy()`?

<details><summary>Answer</summary>

When you want to create a new DataFrame that won't affect the original, especially if you plan to modify it. Without `.copy()` you may get a `SettingWithCopyWarning` in Pandas.
</details>

