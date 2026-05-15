---
type: story
story_id: rss_f182309932eb
episode_date: 2026-04-07
rank: 2
source: rss_feed
url: "https://arxiv.org/abs/2510.17586"
title: DeepEye-SQL A Software-Engineering-Inspired Text-to-SQL Framework
quality_score: 0.932
content_hash: "sha256:223d509d2f5980536e197f3a2185f6e36b0ddbc574fa3e476929f3e95714d4ef"
concepts: [text-to-sql, deepeye-sql, software-development-life-cycle, large-language-models, mixture-of-experts, schema-linking, n-version-sql-generation, bird-benchmark, spider-benchmark, execution-guided-adjudication]
companies: []
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:35:38.239000"
tags: [story, source/rss-feed]
---

## Summary
DeepEye-SQL is a software-engineering-inspired framework that reframes Text-to-SQL as a structured software development problem governed by the Software Development Life Cycle (SDLC). It addresses the lack of structured orchestration in existing LLM-based Text-to-SQL solutions by integrating four stages: schema linking with relational closure, N-version SQL generation, a Syntax-Logic-Quality verification tool-chain, and confidence-aware selection via execution-guided adjudication. Using open-source Mixture-of-Experts LLMs with 30B total parameters (3B activated) and no fine-tuning, DeepEye-SQL achieves 73.5% execution accuracy on BIRD-Dev, 75.07% on the official BIRD-Test leaderboard, and 89.8% on Spider-Test. The results demonstrate that principled orchestration outperforms approaches relying on larger models or extensive training.

## Key claims
- DeepEye-SQL reframes Text-to-SQL as a software engineering problem governed by the Software Development Life Cycle (SDLC).
- The framework integrates schema linking with relational closure, N-version SQL generation, a Syntax-Logic-Quality tool-chain, and confidence-aware selection.
- DeepEye-SQL achieves 73.5% execution accuracy on BIRD-Dev and 75.07% on the official BIRD-Test leaderboard.
- The system achieves 89.8% execution accuracy on Spider-Test, outperforming state-of-the-art solutions.
- DeepEye-SQL uses open-source MoE LLMs with 30B total parameters and only 3B activated parameters without any fine-tuning.
- Principled orchestration, rather than LLM scaling alone, is identified as the key to system-level reliability in Text-to-SQL.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2510.17586>

## Related
[[concepts/text-to-sql|text-to-sql]] · [[concepts/deepeye-sql|deepeye-sql]] · [[concepts/software-development-life-cycle|software-development-life-cycle]] · [[concepts/large-language-models|large-language-models]] · [[concepts/mixture-of-experts|mixture-of-experts]] · [[concepts/schema-linking|schema-linking]] · [[concepts/n-version-sql-generation|n-version-sql-generation]] · [[concepts/bird-benchmark|bird-benchmark]] · [[concepts/spider-benchmark|spider-benchmark]] · [[concepts/orchestration|orchestration]] · [[concepts/schema|schema]] · [[concepts/llms|llms]] · [[concepts/sql|sql]] · [[concepts/llm|llm]] · [[episodes/2026-04-07|2026-04-07]]
