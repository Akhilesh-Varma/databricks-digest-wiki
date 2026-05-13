---
type: story
story_id: rss_30b951fb5c2e
episode_date: 2026-04-14
rank: 10
source: rss_feed
url: "https://arxiv.org/abs/2604.09944"
title: Horrila Cost-Based Placement of Semantic Operators in Hybrid Query Plans
quality_score: 0.796
content_hash: "sha256:cc59ac564b6558bb0479f48e12d07bf95138513fcc1ac0be69e236fcfdd66e04"
concepts: [horrila, semantic-operators, hybrid-query-plans, large-language-models, cost-based-query-optimization, dynamic-programming-cost-model, semantic-filter-placement, function-caching, sembench, semantic-sql, equi-join]
companies: []
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:21:00.112000"
tags: [story, source/rss-feed]
---

## Summary
Horrila is a cost-based query optimizer for hybrid semantic-relational query plans that incorporate large language model (LLM) operators alongside traditional relational operators. The core optimization challenge is deciding where to place semantic operators relative to relational operators: earlier placement reduces downstream data volume but increases LLM calls, while later placement reduces LLM calls via deduplication but inflates intermediate data sizes. Horrila reduces the placement problem to semantic filter placement using two equivalence-preserving rewrites and solves it with a dynamic-programming cost model that minimizes a weighted sum of LLM and relational processing costs. Evaluated on 44 semantic SQL queries across five schemas and two benchmarks, Horrila achieves up to 1.5× speedup and 4.29× cost reduction while maintaining an average F1 of 0.85 against unoptimized baselines.

## Key claims
- Horrila reduces hybrid query planning to semantic filter placement via two equivalence-preserving rewrites.
- Deferring all semantic filters to the latest possible position minimizes LLM invocations under function caching, but can cause relational processing costs to dominate on complex multi-table queries.
- Horrila uses a dynamic-programming-based cost model to find the semantic operator placement that minimizes the weighted sum of LLM and relational processing costs.
- On 44 semantic SQL queries across five schemas and two benchmarks, Horrila achieves up to 1.5× speedup and 4.29× cost reduction over the unoptimized baseline.
- Horrila maintains high output quality with an average F1 of 0.85 against the unoptimized baseline and 0.84 against human-annotated ground truth on SemBench.
- Horrila achieves the highest accuracy among six publicly available hybrid semantic-relational query systems evaluated.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2604.09944>

## Related
[[concepts/horrila|horrila]] · [[concepts/semantic-operators|semantic-operators]] · [[concepts/hybrid-query-plans|hybrid-query-plans]] · [[concepts/large-language-models|large-language-models]] · [[concepts/cost-based-query-optimization|cost-based-query-optimization]] · [[concepts/dynamic-programming-cost-model|dynamic-programming-cost-model]] · [[concepts/semantic-filter-placement|semantic-filter-placement]] · [[concepts/function-caching|function-caching]] · [[concepts/sembench|sembench]] · [[concepts/semantic-sql|semantic-sql]] · [[concepts/deduplication|deduplication]] · [[concepts/query-plans|query-plans]] · [[concepts/llms|llms]] · [[concepts/sql|sql]] · [[concepts/llm|llm]] · [[episodes/2026-04-14|2026-04-14]]
