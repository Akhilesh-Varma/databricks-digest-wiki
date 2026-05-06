---
type: story
story_id: rss_367e7d86bb31
episode_date: 2026-05-06
rank: 8
source: rss_feed
url: "https://arxiv.org/abs/2605.03465"
title: FINER-SQL Boosting Small Language Models for Text-to-SQL
quality_score: 0.756
content_hash: "sha256:0709d8f2700ab239e7cdfbe324acdd15e3ac1feb261fa8b18e36f175d9c2910e"
concepts: [text-to-sql, finer-sql, small-language-models, large-language-models, reinforcement-learning, group-relative-policy-optimization, bird-benchmark, spider-benchmark, fine-grained-execution-feedback, memory-reward, atomic-reward]
companies: []
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-06 10:20:27.469000"
tags: [story, source/rss-feed]
---

## Summary
FINER-SQL is a reinforcement learning framework designed to improve small language models (SLMs) for Text-to-SQL generation. It addresses the limitations of large language models—high cost, latency, and privacy concerns—by enabling efficient on-premise deployment with SLMs. The framework replaces sparse binary rewards with dense, interpretable reward functions: a memory reward for semantic stability and an atomic reward for partial credit on structurally correct SQL. Built on group relative policy optimization, FINER-SQL achieves up to 67.73% and 85% execution accuracy on the BIRD and Spider benchmarks using a 3B model, matching much larger LLMs while reducing inference latency to 5.57 seconds per sample.

## Key claims
- FINER-SQL is a reinforcement learning framework that enhances small language models for Text-to-SQL generation using fine-grained execution feedback.
- Conventional RL methods with sparse binary rewards provide little learning signal when generated SQLs are incorrect, causing unstable training.
- FINER-SQL introduces a memory reward that aligns reasoning with verified traces for semantic stability and an atomic reward that measures operation-level overlap for partial credit.
- The framework is built on group relative policy optimization and enables critic-free, stable optimization.
- FINER-SQL achieves up to 67.73% execution accuracy on BIRD and 85% on Spider benchmarks using a 3B model.
- Inference latency is reduced to 5.57 seconds per sample, making it competitive with much larger LLMs.
- The approach offers a cost-efficient and privacy-preserving path for high-performance Text-to-SQL generation via on-premise SLM deployment.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2605.03465>

## Related
[[concepts/text-to-sql|text-to-sql]] · [[concepts/finer-sql|finer-sql]] · [[concepts/small-language-models|small-language-models]] · [[concepts/large-language-models|large-language-models]] · [[concepts/reinforcement-learning|reinforcement-learning]] · [[concepts/group-relative-policy-optimization|group-relative-policy-optimization]] · [[concepts/bird-benchmark|bird-benchmark]] · [[concepts/spider-benchmark|spider-benchmark]] · [[concepts/fine-grained-execution-feedback|fine-grained-execution-feedback]] · [[concepts/memory-reward|memory-reward]] · [[concepts/atomic-reward|atomic-reward]] · [[concepts/llms|llms]] · [[concepts/sql|sql]] · [[episodes/2026-05-06|2026-05-06]]
