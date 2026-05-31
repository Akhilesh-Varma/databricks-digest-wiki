---
type: story
story_id: devto_3512349
episode_date: 2026-04-17
rank: 7
source: devto
url: "https://dev.to/ptimizeroracle/stop-rewriting-the-same-llm-boilerplate-batch-process-dataframes-in-3-lines-48g2"
title: Stop Rewriting the Same LLM Boilerplate Batch-Process DataFrames in 3 Lines
quality_score: 0.892
content_hash: "sha256:ff821b4460aa17cb3ec5c401a5f9d93810b2f6219248dc1cbc3ea1cff3bae843"
concepts: [ondine, pydantic, langchain, llamaindex, sqlite-fts5, parquet, retrieval-augmented-generation]
companies: [openai]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:10:04.314000"
tags: [story, source/devto]
---

## Summary
The author describes repeatedly rewriting the same LLM batch-processing boilerplate across multiple projects after a painful 158K-row GPT-4 job crashed at row 91K with no checkpoint. To solve this, they built an open-source Python library called Ondine that processes DataFrames with LLMs in minimal code. Ondine includes automatic checkpointing to Parquet, hard dollar-cap cost control, Pydantic-enforced structured output with auto-retry, multi-row batching for throughput, and an anti-hallucination layer backed by a Rust SQLite FTS5 context store. The library is positioned to fill a gap between agent-focused tools like LangChain and RAG-focused tools like LlamaIndex for simple prompt-per-row DataFrame workflows.

## Key claims
- A 158K-row GPT-4 batch job crashed at row 91K with no checkpoint, losing all progress and requiring a restart from zero.
- Ondine reduces LLM DataFrame batch processing to approximately 3 lines of code, replacing ~150 lines of boilerplate.
- Ondine saves checkpoints to Parquet after every batch, enabling resume from the last saved position after a crash.
- A hard dollar cap stops execution when the cost limit is reached rather than merely logging a warning.
- Pydantic schema enforcement with up to 3 automatic retries on malformed output prevents bad JSON from silently polluting large result sets.
- Multi-row batching packs N rows into a single API call, reducing 10K calls to ~200 and significantly cutting wall time.
- An anti-hallucination layer using Rust-backed SQLite FTS5 checks each output against its source input and flags unsupported assertions or contradictions.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/ptimizeroracle/stop-rewriting-the-same-llm-boilerplate-batch-process-dataframes-in-3-lines-48g2>

## Related
[[concepts/ondine|ondine]] · [[concepts/pydantic|pydantic]] · [[concepts/sqlite-fts5|sqlite-fts5]] · [[concepts/parquet|parquet]] · [[concepts/schema-enforcement|schema-enforcement]] · [[concepts/checkpointing|checkpointing]] · [[concepts/dataframes|dataframes]] · [[concepts/dataframe|dataframe]] · [[concepts/schema|schema]] · [[concepts/sqlite|sqlite]] · [[concepts/python|python]] · [[concepts/json|json]] · [[concepts/api|api]] · [[concepts/rag|rag]] · [[concepts/llm|llm]] · [[companies/openai|OpenAI]] · [[episodes/2026-04-17|2026-04-17]]
