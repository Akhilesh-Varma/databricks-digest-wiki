---
type: story
story_id: rss_42c9b38c9a3b
episode_date: 2026-05-08
rank: 10
source: rss_feed
url: "https://arxiv.org/abs/2605.05467"
title: Nitsum Serving Tiered LLM Requests with Adaptive Tensor Parallelism
quality_score: 0.716
content_hash: "sha256:b699d19b78bade0a5a68e446ef96e534b0c88e4f4b64d9144f2d72e88aa09e60"
concepts: [tensor-parallelism, llm-serving, tiered-slo, kv-migration, prefill-decode-disaggregation, goodput, ttft, tpot]
companies: []
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-08 10:23:33.797000"
tags: [story, source/rss-feed]
---

## Summary
Nitsum is a distributed LLM serving system that treats tensor parallelism (TP) as a dynamic runtime control rather than a static deployment choice. It targets multi-tenant deployments where latency-critical interactive requests and relaxed background workloads must coexist under a fixed GPU budget, a setting called tiered-SLO. Nitsum jointly optimizes TP level, prefill-decode GPU split, and request scheduling, and introduces TP-aware weight reuse and fast KV migration to make frequent TP adaptation practical. Experiments on real traces show Nitsum improves SLO-compliant goodput over state-of-the-art systems by up to 5.3 times.

## Key claims
- Nitsum treats tensor parallelism as a first-class runtime control surface rather than a static deployment choice.
- The system targets a tiered-SLO setting where both latency-critical and background workloads share a fixed GPU budget.
- Nitsum jointly optimizes tensor parallelism level, prefill-decode GPU split, and request scheduling.
- TP-aware weight reuse and fast KV migration are introduced to make frequent tensor parallelism adaptation practical.
- Nitsum improves SLO-compliant goodput over state-of-the-art systems by up to 5.3 times on real traces.
- Existing LLM serving systems mainly optimize request-level controls such as queuing and batching while keeping execution configuration static.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2605.05467>

## Related
[[concepts/tensor-parallelism|tensor-parallelism]] · [[concepts/llm-serving|llm-serving]] · [[concepts/tiered-slo|tiered-slo]] · [[concepts/kv-migration|kv-migration]] · [[concepts/prefill-decode-disaggregation|prefill-decode-disaggregation]] · [[concepts/goodput|goodput]] · [[concepts/optimize|optimize]] · [[concepts/llm|llm]] · [[episodes/2026-05-08|2026-05-08]]
