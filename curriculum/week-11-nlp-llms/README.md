<div dir="rtl">

# الأسبوع ١١ — معالجة اللغة الطبيعية + LLMs
## Week 11 — NLP + Large Language Models

> **هذا الأسبوع الأكثر طلباً في السوق ٢٠٢٦. خذه بجدّية.**

---

## ماذا تتعلم

### NLP الكلاسيكي (سريع — يومين)
- Tokenization, Stemming, Lemmatization
- TF-IDF و Bag of Words
- Word Embeddings: Word2Vec, GloVe, FastText

### العصر الحديث (جل الأسبوع)
- **Transformers Architecture** — اقرأ "Attention is All You Need"
- **BERT** — encoder-only، ممتاز للـ classification
- **GPT family** — decoder-only، للـ generation
- **Hugging Face Transformers library** — أداتك الأساسية

### العربي خصوصاً
- **MARBERT** — أحسن نموذج عربي عام
- **AraBERT** — قديم لكنه قوي
- **AceGPT** — Arabic LLM
- **Allam** — Saudi LLM (SDAIA)

### LLMs و RAG
- Prompt engineering
- Function calling
- Embeddings + Vector Databases (Qdrant, Pinecone)
- RAG (Retrieval Augmented Generation)
- Frameworks: LangChain, LlamaIndex (للسياق فقط، الانطلاقة من الكود الخام أهم)

---

## كود أساسي بـ Hugging Face

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

## المصادر

- ⭐ **[Hugging Face NLP Course](https://huggingface.co/learn/nlp-course)** — مجاني، ممتاز، عملي
- ⭐ **[The Illustrated Transformer — Jay Alammar](http://jalammar.github.io/illustrated-transformer/)** — أفضل شرح بصري
- ⭐ **[Andrej Karpathy — Let's build GPT from scratch](https://www.youtube.com/watch?v=kCc8FmEb1nY)** — تبني GPT بإيدك
- [Speech and Language Processing — Jurafsky & Martin (مجاني)](https://web.stanford.edu/~jurafsky/slp3/)
- [SimCSE Paper](https://arxiv.org/abs/2104.08821) — sentence embeddings

---

## التحدي

اختر مهمة عربية: تحليل مشاعر، تصنيف نية، أو NER.
١. اختر dataset من Hugging Face Datasets
٢. fine-tune MARBERT
٣. ارفع النموذج على Hugging Face Hub بـ Model Card كامل
٤. اكتب blog post على LinkedIn يشرح المشروع

> **هذا أهم تحدي في المنهج كله — يدخل portfolio حقك مباشرة.**

---

[**← الأسبوع ١٠**](../week-10-computer-vision/) · [**الأسبوع ١٢ →**](../week-12-capstone/)

</div>
