<div dir="rtl">

# 🧠 Data Science Mastery — دليل علم البيانات الشامل

> **مو مجرد قائمة روابط — هذا منهج عملي تتعلم منه، تتدرب عليه، وتبني فيه ملفك المهني.**
>
> *Not another link dump — a working curriculum you learn from, practice on, and build your portfolio inside.*

دليل ثنائي اللغة (عربي/إنجليزي) لكل شخص يبي يدخل علم البيانات بجدّ — من الصفر للوظيفة الأولى.
صُمم لطلاب الجامعات السعودية والعرب الطموحين، ومبني على أحسن المصادر المتوفرة (مايكروسوفت، ستانفورد، KAUST Academy، DeepLearning.AI، Hugging Face).

---

## ليش هذا المستودع مختلف؟ — Why this is different

أكثر القوائم الموجودة في GitHub فيها مشكلة واحدة: **روابط بدون طريق.** تفتح المستودع تحصل 200 رابط، تطفّش، تروح.

هذا الدليل مبني على ٣ مبادئ:

| المبدأ | الشرح |
|---|---|
| 🛤️ **منهج تسلسلي (12 أسبوع)** | تعرف وش تسوي اليوم، وش بكرة، وش بعد شهرين. مو "اقرأ كل شيء". |
| 🔨 **التعلم بالممارسة** | كل أسبوع فيه تمرين عملي، notebook قابل للتشغيل، وتحدي ترفعه على GitHub. |
| 🎯 **آراء واضحة، مو حياد** | ما نسرد ١٥ كورس — نختار واحد ونقول ليش. التنسيق هو القيمة. |

---

## المنهج — The 12-Week Curriculum

| الأسبوع | الموضوع | المخرج العملي |
|:---:|---|---|
| **01** | [أساسيات Python لعلم البيانات](curriculum/week-01-python-foundations/) | Notebook: تحليل ملف CSV حقيقي |
| **02** | [الرياضيات اللي تحتاجها فعلاً](curriculum/week-02-math-for-ds/) | حل تمارين Linear Algebra + Probability |
| **03** | [معالجة البيانات بـ Pandas](curriculum/week-03-data-wrangling/) | تنظيف dataset متسخ من Kaggle |
| **04** | [تصور البيانات — Visualization](curriculum/week-04-visualization/) | تقرير EDA كامل بـ matplotlib + seaborn |
| **05** | [التعلم الموجَّه — Supervised ML](curriculum/week-05-supervised-ml/) | نموذج Regression + Classification |
| **06** | [تقييم النماذج — Evaluation](curriculum/week-06-model-evaluation/) | Cross-validation + confusion matrix |
| **07** | [هندسة الميزات — Feature Engineering](curriculum/week-07-feature-engineering/) | تحسين accuracy على dataset حقيقي |
| **08** | [التعلم غير الموجَّه — Unsupervised](curriculum/week-08-unsupervised/) | Clustering + PCA على بيانات حقيقية |
| **09** | [الشبكات العصبية — Neural Networks](curriculum/week-09-neural-networks/) | بناء NN من الصفر بـ PyTorch |
| **10** | [الرؤية الحاسوبية — Computer Vision](curriculum/week-10-computer-vision/) | Image classifier بـ Transfer Learning |
| **11** | [معالجة اللغة + LLMs](curriculum/week-11-nlp-llms/) | Fine-tune model عربي على Hugging Face |
| **12** | [مشروع التخرج — Capstone](curriculum/week-12-capstone/) | مشروع كامل يدخل portfolio |

> **توقع** ١٠–١٥ ساعة بالأسبوع. المنهج للجادّين فقط — مو تصفّح.

---

## كيف تستخدم المستودع — How to use this repo

```bash
# 1. اعمل Fork للمستودع (هذا أول تمرين Git لك)
# 2. clone النسخة الخاصة فيك
git clone https://github.com/<your-username>/data-science-mastery-ar.git
cd data-science-mastery-ar

# 3. ابدأ من الأسبوع الأول
cd curriculum/week-01-python-foundations
```

كل أسبوع فيه:
- 📖 `README.md` — الدرس (بالعربي والإنجليزي)
- 🧪 `exercise.md` — تمرين عملي
- ❓ `quiz.md` — ٥ أسئلة للمراجعة
- 🔗 موارد مختارة — مو ١٥ رابط، بس اللي يستاهل

---

## الأقسام الإضافية — Additional Sections

| المجلد | المحتوى |
|---|---|
| 📚 [`awesome-list/`](awesome-list/) | كورسات وكتب وقنوات يوتيوب مختارة بعناية (مو dump) |
| 📐 [`templates/`](templates/) | قوالب جاهزة: README للمشاريع، Profile README، notebook template |
| 💼 [`interview-prep/`](interview-prep/) | أسئلة مقابلات Data Science (SQL, Python, ML, statistics) |
| 🏭 [`real-world/`](real-world/) | كيف يستخدم علم البيانات في Stripe, Airbnb, Netflix — case studies |
| 🛣️ [`tracks/`](tracks/) | تخصصات بعد الأسبوع ١٢: NLP, CV, MLOps, Research |
| 🎮 [`practice-playground/`](practice-playground/) | فرع فيه bugs ومشاكل عمداً — تمرّن git, PRs, conflicts |

---

## مناهج بديلة (للمقارنة) — Alternative roadmaps

نحترم اللي قبلنا. هذه المراجع اللي تأثرنا فيها:

- [roadmap.sh — AI/Data Scientist](https://roadmap.sh/ai-data-scientist) — visual roadmap
- [Microsoft — Data Science for Beginners](https://github.com/microsoft/Data-Science-For-Beginners) — 10-week curriculum
- [Open Source Society University — Data Science](https://github.com/ossu/data-science) — degree-equivalent
- [Awesome Data Science](https://github.com/academic/awesome-datascience) — comprehensive list
- [Applied ML (eugeneyan)](https://github.com/eugeneyan/applied-ml) — production case studies

**الفرق:** هذي المراجع كلها إنجليزية، وأكثرها قوائم بدون منهج. هذا المستودع عربي + إنجليزي + منهج متسلسل + تطبيق على GitHub نفسه.

---

## للمساهمة — Contributing

تبي تضيف مصدر أو تصلح خطأ؟ اقرأ [`CONTRIBUTING.md`](CONTRIBUTING.md).
وعملية المساهمة نفسها هي تمرين Git — fork, branch, PR.

---

## الترخيص — License

MIT — استخدم، عدّل، انشر. بس اذكر المصدر إذا قدرت.

---

<sub>صُنع بـ ❤️ في مكة المكرمة — Made with care in Makkah</sub>
<sub>المُنسّق: [Yousef Ammar](https://github.com/YOUSEF-ysfxjo) — Data Scientist @ Qanoniah · AI Engineer @ Moasherat</sub>

</div>
