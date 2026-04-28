---
type: story
story_id: hn_47914367
episode_date: 2026-04-27
rank: 4
source: hacker_news
url: "https://github.com/sachitrafa/YourMemory"
title: Show HN AI memory with biological decay 52 recall
quality_score: 0.591
content_hash: "sha256:844ac01c6682ab462ac8513233bdbc65b15ea74d7d7746134e8f89fa43d5eafa"
concepts: [rag, ebbinghaus-forgetting-curve, context-window, spaced-repetition, vector-store, semantic-search, duckdb, mcp-server]
companies: []
people: []
extractor_model: gemini-2.5-flash-lite
extracted_at: "2026-04-28 03:21:01.149000"
tags: [story, source/hacker-news]
---

## Summary
This project introduces a novel approach to AI memory management inspired by biological decay, specifically the Ebbinghaus forgetting curve. Unlike static filing cabinets, this system treats memory as a dynamic substrate where recall strengthens data and unused information is pruned. It addresses the "logical neighbor" problem by layering a graph over a vector store, achieving significantly higher recall and reduced token waste compared to traditional stateless vector stores. The core hypothesis is that managing what to forget is as crucial as remembering for long-running AI projects.

## Key claims
- Most RAG setups fail due to treating memory statically, leading to context window bloat and degraded reasoning.
- This implementation uses the Ebbinghaus forgetting curve to manage context dynamically.
- Memories are strengthened by recall and pruned when unused, mimicking biological decay.
- A graph layer is added over the vector store to solve the "logical neighbor" problem in semantic search.
- The system achieved 52 Recall 5 on the LoCoMo dataset, nearly doubling the accuracy of stateless vector stores.
- Token waste was reduced by approximately 84% compared to stateless vector stores.
- The project hypothesizes that managing what to forget is critical for AI agents handling long-running projects.

## Source
- **Origin:** hacker_news
- **URL:** <https://github.com/sachitrafa/YourMemory>

## Related
[[concepts/rag|rag]] · [[concepts/ebbinghaus-forgetting-curve|ebbinghaus-forgetting-curve]] · [[concepts/context-window|context-window]] · [[concepts/spaced-repetition|spaced-repetition]] · [[concepts/vector-store|vector-store]] · [[concepts/semantic-search|semantic-search]] · [[concepts/linear|linear]] · [[concepts/ai|ai]] · [[episodes/2026-04-27|2026-04-27]]
