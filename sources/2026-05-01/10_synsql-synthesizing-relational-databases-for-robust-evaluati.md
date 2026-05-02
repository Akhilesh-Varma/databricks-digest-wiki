---
type: story
story_id: rss_6270ed9508d7
episode_date: 2026-05-01
rank: 10
source: rss_feed
url: "https://arxiv.org/abs/2604.27261"
title: SynSQL Synthesizing Relational Databases for Robust Evaluation of Text-to-SQL Systems
quality_score: 0.796
content_hash: "sha256:d8f1f3143099f869614e747b894fac006d2fef491c235153bdb6ec3b3e3307ca"
concepts: [synsql, text-to-sql, spider-benchmark, bird-benchmark, spider-2-0, large-language-models, structured-generation, schema-consistent-data-synthesis, iterative-refinement]
companies: []
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-01 10:20:57.339000"
tags: [story, source/rss-feed]
---

## Summary
SynSQL is a framework introduced to address fragility in text-to-SQL evaluation, where correctness is typically judged by executing queries on a single static database. The framework synthesizes test databases conditioned on question-schema alignment through three stages: schema selection, question-guided data synthesis, and constraint-aware critique with iterative refinement. Evaluated across ten text-to-SQL models on Spider, BIRD, and Spider 2.0 benchmarks, SynSQL-generated databases reveal performance drops of 3–14% compared to static evaluation, exposing errors masked by benchmark artifacts. The work also investigates whether large language models can synthesize semantically meaningful, schema-consistent relational data from natural language questions, positioning synthetic database generation as a new lens for studying LLM reasoning and robustness.

## Key claims
- Text-to-SQL evaluation is fragile because correctness is judged by executing queries on a single static database, which may not generalize to alternative database instances.
- SynSQL synthesizes test databases conditioned on question-schema alignment rather than gold SQL queries.
- The framework decomposes database synthesis into three stages: schema selection, question-guided data synthesis, and constraint-aware critique with iterative refinement.
- SynSQL-generated databases reveal performance drops of 3–14% across ten text-to-SQL models compared to static benchmark evaluation.
- These performance drops expose errors that are masked by artifacts in fixed benchmark databases.
- The study investigates the ability of large language models to synthesize semantically meaningful, schema-consistent relational data directly from natural language questions.
- Synthetic database generation is proposed as a new methodology for studying LLM reasoning, controllability, and robustness in structured environments.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2604.27261>

## Related
[[concepts/synsql|synsql]] · [[concepts/text-to-sql|text-to-sql]] · [[concepts/spider-benchmark|spider-benchmark]] · [[concepts/bird-benchmark|bird-benchmark]] · [[concepts/spider-2-0|spider-2-0]] · [[concepts/large-language-models|large-language-models]] · [[concepts/structured-generation|structured-generation]] · [[concepts/schema-consistent-data-synthesis|schema-consistent-data-synthesis]] · [[concepts/text-to-sql-models|text-to-sql-models]] · [[concepts/schema|schema]] · [[concepts/llms|llms]] · [[concepts/sql|sql]] · [[concepts/llm|llm]] · [[episodes/2026-05-01|2026-05-01]]
