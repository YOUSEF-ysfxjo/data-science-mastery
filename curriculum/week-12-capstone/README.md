# Week 12 — Capstone Project

> **The idea:** one complete project, published professionally, as the star of your portfolio.

---

## Criteria for a Good Project

✅ Solves a real problem (not "Iris classification")
✅ Uses real data (not a pre-built sklearn dataset)
✅ End-to-end: from data collection to deployment
✅ Well documented (excellent README + blog post)
✅ Reproducible on another person's machine

---

## Project Ideas

### Level 1 (Acceptable)
- A car price prediction model for the Saudi market (web scraping from haraj.com)
- Sentiment analysis of Arabic tweets about a sporting event
- A movie recommendation system (collaborative filtering)

### Level 2 (Excellent)
- An Arabic complaint classification system with MARBERT (with an API)
- A prediction model for Hajj operations completion time (if you have Ministry of Hajj data)
- An Arabic chatbot with RAG on a legal/medical dataset

### Level 3 (Outstanding — opens doors)
- A published paper + repo + dataset
- A top 10% ranking in a Kaggle competition
- A real contribution to a major open source project (Hugging Face, Pandas, etc.)

---

## Golden Project Structure

```
my-capstone/
├── README.md                # ⭐ The star — write it well
├── notebooks/
│   ├── 01-eda.ipynb
│   ├── 02-modeling.ipynb
│   └── 03-evaluation.ipynb
├── src/
│   ├── data.py             # data loading & preprocessing
│   ├── features.py
│   ├── train.py
│   ├── evaluate.py
│   └── api.py              # FastAPI for deployment (if applicable)
├── models/                  # saved models (.gitignore if large)
├── data/                    # usually .gitignore
├── tests/
├── Dockerfile
├── requirements.txt
├── .gitignore
└── LICENSE
```

Use [Cookiecutter Data Science](https://github.com/drivendataorg/cookiecutter-data-science) as a template.

---

## A Great README Contains:

1. Clear title + logo/image
2. The problem statement
3. Solution architecture (diagram)
4. Results (metrics + visualizations)
5. How to run it (`make run` or clone & install steps)
6. Tech stack
7. Future work
8. License

See [`templates/project-readme-template.md`](../../templates/project-readme-template.md) for the template.

---

## Final Submission

1. **Repo on GitHub** — public, well-documented
2. **Blog post** — Medium / LinkedIn / Hashnode (800–1500 words)
3. **Demo** — if feasible: Hugging Face Space, Streamlit Cloud, or deploy on Railway
4. **LinkedIn post** — image + 3 things you learned
5. **(Bonus)** A 3-minute YouTube video explaining the project

---

## After the Capstone — Next Steps

- Choose a track from [`tracks/`](../../tracks/) to specialize in
- Start applying for summer internships
- Contribute to open source
- Write a paper if you have research results
- Keep learning — the field moves fast

---

🎉 **Congratulations. If you made it here, you're no longer a beginner. This is the start of your real journey.**

[**← Week 11**](../week-11-nlp-llms/) · [**Back to Curriculum**](../README.md)

