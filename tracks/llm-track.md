# 🤖 Track: LLMs & Agents

> **The most in-demand track in 2026.** But be careful — the surface is accessible to everyone. Depth is rare.

---

## Curriculum (8 weeks)

### Week 1: LLM Concepts
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
- When **not** to fine-tune (most of the time!)

### Week 5: Agents
- Tool calling / function calling
- Planning + reasoning
- Multi-agent systems
- Real risks (hallucinations, prompt injection)

### Week 6: Frameworks (use with caution)
- LangChain, LlamaIndex (understand their limitations)
- Anthropic SDK / OpenAI SDK directly (better for many cases)
- Pydantic AI (the new one)

### Week 7: Production LLM Apps
- Caching (semantic + exact)
- Rate limiting
- Cost optimization
- Streaming responses
- Guardrails

### Week 8: Project
Build a RAG application on a real domain + deploy.

---

## Resources

- ⭐ [Andrej Karpathy — Let's build GPT](https://www.youtube.com/watch?v=kCc8FmEb1nY)
- ⭐ [Hugging Face NLP Course](https://huggingface.co/learn/nlp-course)
- ⭐ [Anthropic Cookbook](https://github.com/anthropics/anthropic-cookbook)
- ⭐ [OpenAI Cookbook](https://github.com/openai/openai-cookbook)
- [LLM University — Cohere](https://llm.university/)
- [Simon Willison's blog](https://simonwillison.net/) — everyday applications
- [Eugene Yan — LLM Patterns](https://eugeneyan.com/writing/llm-patterns/)

---

## An Honest Opinion

LangChain helped many people get started. But in production, most serious teams (Octomind, Anthropic) **write directly against the SDKs**. Start with LangChain if you want, but be prepared to move on.

