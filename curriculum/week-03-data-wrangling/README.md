# Week 3 — Data Wrangling with Pandas

> **Reality:** 70% of a data scientist's time is spent cleaning data, not building models. This week teaches the skill that won't make it onto your LinkedIn but will define your value at work.

---

## What You Learn

### Day 1: Reading Data from Everywhere
- CSV, Excel, JSON, Parquet
- SQL databases (`pd.read_sql`)
- APIs (`requests` + `pd.json_normalize`)
- Web scraping with Pandas (`pd.read_html`)

### Day 2: Handling Missing Values
- When to drop? When to impute?
- `fillna` with mean/median/mode
- `KNN imputation`
- Creating an `is_missing` feature (the absence itself sometimes carries information)

### Day 3: Merging, Joining, Concatenation
- `merge` (inner, left, right, outer) — understand the difference
- `concat` for stacking
- `join` on index
- Duplicate issues after merge

### Day 4: Transformations
- `apply`, `map`, `applymap` — when to use which
- `pd.get_dummies` for categorical data
- `pd.cut` and `pd.qcut` for binning
- Working with dates (`pd.to_datetime`, `.dt` accessors)

### Day 5: Advanced Group Operations
- `groupby` + `agg` with multiple functions
- `transform` (returns same size) vs `agg`
- `pivot_table` and `crosstab`
- Window functions: `rolling`, `expanding`

### Day 6: Performance
- When to use `vectorization` instead of `apply`
- `dtype` optimization (`int64` → `int8` where applicable)
- `chunksize` for large files
- Polars (the faster Pandas alternative — get familiar with it)

### Day 7: Weekly Challenge

---

## Curated Resources

### Primary ⭐
**[Pandas in Action — Boris Paskhaver](https://www.manning.com/books/pandas-in-action)** — a paid book worth it. If you can't get it, the first chapters of Python Data Science Handbook work too.

### For Practice
**[Pandas Exercises (GitHub)](https://github.com/guipsamora/pandas_exercises)** — 200+ graduated exercises. **This is the most important link of the week.**

### In Arabic
**[Hesham Asem — Pandas](https://www.youtube.com/@HeshamAsem)** — practical tutorials.

---

## Common Pitfalls

```python
# ❌ Wrong: may produce SettingWithCopyWarning
df[df["age"] > 25]["salary"] = 5000

# ✅ Correct
df.loc[df["age"] > 25, "salary"] = 5000

# ❌ Very slow on large dataframes
df["new"] = df["col"].apply(lambda x: x * 2)

# ✅ 100× faster
df["new"] = df["col"] * 2

# ❌ Consumes a lot of memory
df = pd.read_csv("huge.csv")

# ✅ For large files
chunks = pd.read_csv("huge.csv", chunksize=10000)
for chunk in chunks:
    process(chunk)
```

---

## Weekly Challenge

Work on a real messy dataset — we suggest [NYC 311 Service Requests](https://data.cityofnewyork.us/Social-Services/311-Service-Requests-from-2010-to-Present/erm2-nwhp).

1. Download a sample (1 million rows).
2. Identify the important columns (70% of the columns are unnecessary).
3. Clean missing values.
4. Convert date columns.
5. Produce 5 groupby insights.
6. Document the steps in a notebook.

---

[**← Week 2**](../week-02-math-for-ds/) · [**Week 4 →**](../week-04-visualization/)

