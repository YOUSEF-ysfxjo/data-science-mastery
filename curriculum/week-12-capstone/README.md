<div dir="rtl">

# الأسبوع ١٢ — مشروع التخرج (Capstone)
## Week 12 — Capstone Project

> **الفكرة:** مشروع واحد كامل، نشر بشكل احترافي، يكون نجم portfolio حقك.

---

## معايير المشروع الجيد

✅ يحل مشكلة حقيقية (مو "Iris classification")
✅ بيانات حقيقية (مو dataset جاهز من sklearn)
✅ كامل: من جمع البيانات للـ deployment
✅ موثّق (README ممتاز + blog post)
✅ يقدر يشتغل على جهاز شخص ثاني (reproducible)

---

## أمثلة لأفكار مشاريع

### مستوى ١ (مقبول)
- نموذج توقع أسعار سيارات في السوق السعودي (web scraping من haraj.com)
- تحليل مشاعر تغريدات عربية حول حدث رياضي
- نظام توصية أفلام (collaborative filtering)

### مستوى ٢ (ممتاز)
- نظام تصنيف شكاوى عربية بـ MARBERT (مع API)
- نموذج توقع وقت إنجاز Hajj operations (لو عندك بيانات وزارة الحج)
- chatbot عربي بـ RAG على dataset قانوني/طبي

### مستوى ٣ (مذهل — يفتح أبواب)
- بحث منشور (paper) + repo + dataset
- مشروع في مسابقة Kaggle بترتيب top 10%
- مساهمة فعلية في open source project كبير (Hugging Face, Pandas, etc.)

---

## بنية المشروع الذهبية

```
my-capstone/
├── README.md                # ⭐ النجم — اكتبه ممتاز
├── notebooks/
│   ├── 01-eda.ipynb
│   ├── 02-modeling.ipynb
│   └── 03-evaluation.ipynb
├── src/
│   ├── data.py             # data loading & preprocessing
│   ├── features.py
│   ├── train.py
│   ├── evaluate.py
│   └── api.py              # FastAPI لو فيه deployment
├── models/                  # نماذج محفوظة (.gitignore لو كبيرة)
├── data/                    # عادة .gitignore
├── tests/
├── Dockerfile
├── requirements.txt
├── .gitignore
└── LICENSE
```

استخدم [Cookiecutter Data Science](https://github.com/drivendataorg/cookiecutter-data-science) كقالب.

---

## README ممتاز يحتوي:

١. عنوان واضح + شعار/صورة
٢. الـ problem statement
٣. الـ solution architecture (مخطط)
٤. النتائج (metrics + visualizations)
٥. كيف تشغّله (`make run` أو خطوات clone & install)
٦. Tech stack
٧. أعمال مستقبلية
٨. الترخيص

شوف [`templates/project-readme-template.md`](../../templates/project-readme-template.md) للقالب.

---

## التسليم النهائي

١. **Repo على GitHub** — public, well-documented
٢. **Blog post** — Medium / LinkedIn / Hashnode (٨٠٠–١٥٠٠ كلمة)
٣. **Demo** — إذا ينفع: Hugging Face Space أو Streamlit Cloud أو deploy على Railway
٤. **LinkedIn post** — صورة + ٣ نقاط من اللي تعلمته
٥. **(مكافأة)** فيديو ٣ دقائق على YouTube يشرح المشروع

---

## بعد الـ Capstone — الخطوات التالية

- اختار track من [`tracks/`](../../tracks/) للتخصص
- ابدأ تتقدم لتدريبات صيفية
- ساهم في open source
- اكتب paper لو عندك نتائج بحثية
- استمر تتعلم — الـ field يتحرك بسرعة

---

🎉 **مبروك. لو وصلت هنا، مو مبتدئ بعد. هذا بداية رحلتك الفعلية.**

[**← الأسبوع ١١**](../week-11-nlp-llms/) · [**العودة للمنهج**](../README.md)

</div>
