## Why Prompt Caching?

LLM systems often repeat:
- Identical system prompts
- Reused few-shot examples
- Similar user queries
- Repeated retrieval contexts

This leads to:
- Increased token cost
- Higher latency
- Redundant computation
- Scalability bottlenecks

This repository explores multiple caching architectures 
to reduce cost and improve performance in AI systems.

---

## Implemented Architectures

### 1. Deterministic Prompt Cache
Exact-match SHA-256 hashing based caching layer.

### 2. Semantic Prompt Cache
Embedding similarity-based caching layer that reuses LLM responses for semantically similar prompts using cosine similarity thresholds.

### 3. RAG-Aware Prompt Cache
Context-safe caching layer that optimizes Retrieval-Augmented Generation by caching retrieval results and binding generation reuse to document-set hashing.
