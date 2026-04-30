# Week 1 — Python Foundations for Data Science

> **Goal:** By the end of this week, you can open a data file, read it with NumPy/Pandas, and extract basic statistics without Googling every line.

---

## Why Python?

Data science needs a language that is:
- Easy to write (focus on the problem, not the syntax)
- Has powerful libraries (NumPy, Pandas, Scikit-learn, PyTorch)
- Has a huge community (answers to every question)

R is an excellent language but Python has won in industry. R remains useful for academic statistics.

---

## What You Learn This Week

### Day 1–2: Python Basics (if you don't know it yet)
- Variables, types, lists, dicts, tuples, sets
- Control flow: `if`, `for`, `while`
- Functions, scope, `*args`, `**kwargs`
- List comprehensions — **very important**
- File I/O: reading and writing files

> **If you already know Python:** skip to Day 3.

### Day 3: NumPy
- `np.array` — why is it faster than a list?
- Vectorization (don't use `for` loops on arrays)
- Broadcasting
- Indexing & slicing
- Random numbers (`np.random`)

### Day 4–5: Pandas (Introduction)
- `Series` and `DataFrame`
- Reading CSV, Excel, JSON
- `.head()`, `.info()`, `.describe()`
- Filtering rows, selecting columns
- Basic `.groupby()`

### Day 6: Jupyter + Git
- Why Jupyter notebooks for exploration
- VS Code + notebook extension (better than Jupyter Lab for most people)
- Basic Git: `init`, `add`, `commit`, `push`
- Connecting GitHub to your account

### Day 7: Weekly Challenge
[See `exercise.md`](exercise.md)

---

## Curated Resources (3 only, not 15)

### Primary Resource ⭐
**[Python Data Science Handbook — Jake VanderPlas](https://jakevdp.github.io/PythonDataScienceHandbook/)** — free, notebooks runnable in Colab. Read Chapters 1–3.

### For Complete Beginners
**[Python for Everybody — Dr. Charles Severance (Coursera)](https://www.coursera.org/specializations/python)** — free to audit. Take Course 1 + 2 if Python is new to you.

### In Arabic
**[Elzero Web School — Mastering Python (Arabic playlist)](https://www.youtube.com/playlist?list=PLDoPjvoNmBAyE_gei5d18qkfIe-Z8mocs)** — clear, structured lessons from beginner to advanced.

> **Don't distract yourself.** Pick one and commit. The rest is noise.

---

## Pandas Commands You'll Use Every Day

```python
import pandas as pd

df = pd.read_csv("data.csv")     # read file
df.head()                         # first 5 rows
df.info()                         # column types + null counts
df.describe()                     # numerical statistics
df.shape                          # (rows, columns)
df.columns                        # column names

df["age"]                         # single column (Series)
df[["age", "salary"]]             # multiple columns
df[df["age"] > 25]                # filter
df.groupby("city")["salary"].mean()  # group and aggregate
```

Memorize these 10 lines. They cover 80% of your daily work.

---

## After You Finish

- ✅ Push the challenge notebook to GitHub in a repo named `ds-week-01`
- ✅ Write a simple README.md: what you did, what you learned, what was challenging
- ✅ Share the repo on LinkedIn — `#100DaysOfDataScience`
- ✅ Review [`quiz.md`](quiz.md) before moving to Week 2

---

## Common Mistakes This Week

| Mistake | Fix |
|---|---|
| Using `for loop` on a NumPy array | Use vectorized operations |
| Forgetting `inplace=True` or not saving the result | `df = df.dropna()` instead of `df.dropna()` |
| Confusing `.loc[]` with `.iloc[]` | `loc` for labels, `iloc` for positions |
| Modifying a DataFrame while iterating over it | Use `.copy()` when in doubt |

---

[**← Main Curriculum**](../README.md) · [**Exercise →**](exercise.md) · [**Week 2 →**](../week-02-math-for-ds/)

