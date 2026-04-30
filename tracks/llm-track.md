<div dir="rtl">

# 🤖 Track: LLMs & Agents

> **الأكثر طلباً في ٢٠٢٦.** بس انتبه — السطح متاح للجميع. العمق نادر.

---

## المنهج (٨ أسابيع)

### Week 1: مفاهيم LLMs
- Tokenization (BPE, SentencePiece)
- Pre-training vs fine-tuning vs RLHF
- Scaling laws
- Quantization (GPTQ, AWQ)

### Week 2: Prompt Engineering
- Zero-shot, few-shot, chain-of-thought
- ReAct pattern
- Anthropic / OpenAI cookbooks
- Evaluation (Promptfoo)

### Week 3: RAG
- Embeddings: OpenAI, Cohere, Nomic, BGE
- Vector DBs: Qdrant (recommended), Pinecone, Weaviate
- Chunking strategies
- Hybrid search (BM25 + dense)
- Reranking (Cohere Rerank, ColBERT)

### Week 4: Fine-tuning
- LoRA, QLoRA
- Hugging Face TRL
- Domain adaptation
- متى **لا** تعمل fine-tune (أكثر الحالات!)

### Week 5: Agents
- Tool calling / function calling
- Planning + reasoning
- Multi-agent systems
- المخاطر الحقيقية (hallucinations, prompt injection)

### Week 6: Frameworks (بحذر)
- LangChain, LlamaIndex (افهم limitations)
- Anthropic SDK / OpenAI SDK مباشرة (الأفضل لكثير من الحالات)
- Pydantic AI (الجديد)

### Week 7: Production LLM Apps
- Caching (semantic + exact)
- Rate limiting
- Cost optimization
- Streaming responses
- Guardrails

### Week 8: مشروع
ابنِ RAG تطبيق على domain حقيقي + deploy.

---

## مصادر

- ⭐ [Andrej Karpathy — Let's build GPT](https://www.youtube.com/watch?v=kCc8FmEb1nY)
- ⭐ [Hugging Face NLP Course](https://huggingface.co/learn/nlp-course)
- ⭐ [Anthropic Cookbook](https://github.com/anthropics/anthropic-cookbook)
- ⭐ [OpenAI Cookbook](https://github.com/openai/openai-cookbook)
- [LLM University — Cohere](https://llm.university/)
- [Simon Willison's blog](https://simonwillison.net/) — تطبيقات يومية
- [Eugene Yan — LLM Patterns](https://eugeneyan.com/writing/llm-patterns/)

---

## رأي صريح

LangChain ساعد كثيرين يبدأون. لكن في الإنتاج، أكثر الفرق الجادة (Octomind, Anthropic) **يكتبون مباشرة على الـ SDKs**. ابدأ بـ LangChain لو حاب، لكن استعد لتركها.

</div>
