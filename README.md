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
