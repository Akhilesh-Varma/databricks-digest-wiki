---
type: story
story_id: rss_1af7689ee95c
episode_date: 2026-04-08
rank: 3
source: rss_feed
url: "https://arxiv.org/abs/2511.07663"
title: Cortex AISQL A Production SQL Engine for Unstructured Data
quality_score: 0.911
content_hash: "sha256:76342334a5828416db291148c134533ff1e1eaedbc2d730cdacf9e1a7c207764"
concepts: [cortex-aisql, ai-aware-query-optimization, adaptive-model-cascades, semantic-join-query-rewriting, large-language-model, multi-label-classification, query-execution-engine, semantic-operations]
companies: [snowflake]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:32:46.378000"
tags: [story, source/rss-feed]
---

## Summary
Snowflake's Cortex AISQL is a production SQL engine that integrates native semantic operations directly into SQL, enabling declarative queries over both structured and unstructured data. The system addresses fundamental challenges of running AI inference at production scale, including high cost, unknown selectivity at compile time, and latency characteristics unlike traditional SQL. Three novel techniques are introduced: AI-aware query optimization, adaptive model cascades, and semantic join query rewriting. These techniques deliver speedups ranging from 2x to 70x while maintaining high prediction quality. AISQL is deployed in production at Snowflake, powering analytics, search, and content understanding workloads.

## Key claims
- Cortex AISQL integrates native semantic operations directly into SQL, allowing relational and semantic reasoning in a single declarative query.
- AI-aware query optimization treats LLM inference cost as a first-class objective during query planning, achieving 2-8x speedups.
- Adaptive model cascades route most rows through a fast proxy model and escalate uncertain cases to an oracle model, achieving 2-6x speedups while retaining 90-95% of oracle model quality.
- Semantic join query rewriting reformulates join operations as multi-label classification tasks, reducing quadratic time complexity to linear and achieving 15-70x speedups.
- Semantic operations pose unique challenges because their cost and selectivity are unknown at query compilation time.
- AISQL is deployed in production at Snowflake and powers customer workloads across analytics, search, and content understanding.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2511.07663>

## Related
[[concepts/cortex-aisql|cortex-aisql]] · [[concepts/ai-aware-query-optimization|ai-aware-query-optimization]] · [[concepts/adaptive-model-cascades|adaptive-model-cascades]] · [[concepts/semantic-join-query-rewriting|semantic-join-query-rewriting]] · [[concepts/large-language-model|large-language-model]] · [[concepts/multi-label-classification|multi-label-classification]] · [[concepts/query-execution-engine|query-execution-engine]] · [[concepts/semantic-operations|semantic-operations]] · [[concepts/time-complexity|time-complexity]] · [[concepts/query-planning|query-planning]] · [[concepts/language-model|language-model]] · [[concepts/snowflake|snowflake]] · [[concepts/analytics|analytics]] · [[concepts/optimize|optimize]] · [[concepts/linear|linear]] · [[concepts/sql|sql]] · [[concepts/llm|llm]] · [[concepts/ai|ai]] · [[companies/snowflake|Snowflake]] · [[episodes/2026-04-08|2026-04-08]]
