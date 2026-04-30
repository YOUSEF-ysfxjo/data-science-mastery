# Week 11 — Natural Language Processing + LLMs

> **This is the most in-demand week in the market in 2026. Take it seriously.**

---

## What You Learn

### Classical NLP (fast — two days)
- Tokenization, Stemming, Lemmatization
- TF-IDF and Bag of Words
- Word Embeddings: Word2Vec, GloVe, FastText

### The Modern Era (most of the week)
- **Transformers Architecture** — read "Attention is All You Need"
- **BERT** — encoder-only, excellent for classification
- **GPT family** — decoder-only, for generation
- **Hugging Face Transformers library** — your primary tool

### Arabic-Specific
- **MARBERT** — best general-purpose Arabic model
- **AraBERT** — older but powerful
- **AceGPT** — Arabic LLM
- **Allam** — Saudi LLM (SDAIA)

### LLMs and RAG
- Prompt engineering
- Function calling
- Embeddings + Vector Databases (Qdrant, Pinecone)
- RAG (Retrieval Augmented Generation)
- Frameworks: LangChain, LlamaIndex (for context only — raw code is more important)

---

## Basic Hugging Face Code

```python
from transformers import pipeline

classifier = pipeline("sentiment-analysis", model="UBC-NLP/MARBERT")
result = classifier("الخدمة كانت ممتازة جداً")
print(result)
```

```python
from transformers import AutoTokenizer, AutoModelForSequenceClassification
import torch

tokenizer = AutoTokenizer.from_pretrained("UBC-NLP/MARBERT")
model = AutoModelForSequenceClassification.from_pretrained(
    "UBC-NLP/MARBERT", num_labels=3
)

inputs = tokenizer("النص العربي هنا", return_tensors="pt")
with torch.no_grad():
    outputs = model(**inputs)
```

---

## Resources

- ⭐ **[Hugging Face NLP Course](https://huggingface.co/learn/nlp-course)** — free, excellent, practical
- ⭐ **[The Illustrated Transformer — Jay Alammar](http://jalammar.github.io/illustrated-transformer/)** — the best visual explanation
- ⭐ **[Andrej Karpathy — Let's build GPT from scratch](https://www.youtube.com/watch?v=kCc8FmEb1nY)** — you build GPT yourself
- [Speech and Language Processing — Jurafsky & Martin (free)](https://web.stanford.edu/~jurafsky/slp3/)
- [SimCSE Paper](https://arxiv.org/abs/2104.08821) — sentence embeddings

---

## Challenge

Choose an Arabic task: sentiment analysis, intent classification, or NER.
1. Choose a dataset from Hugging Face Datasets
2. Fine-tune MARBERT
3. Upload the model to Hugging Face Hub with a complete Model Card
4. Write a blog post on LinkedIn explaining the project

> **This is the most important challenge in the entire curriculum — it goes directly into your portfolio.**

---

[**← Week 10**](../week-10-computer-vision/) · [**Week 12 →**](../week-12-capstone/)

