---
type: story
story_id: rss_e4b2ac707bd2
episode_date: 2026-04-10
rank: 2
source: rss_feed
url: "https://arxiv.org/abs/2604.08021"
title: SynQL A Controllable and Scalable Rule-Based Framework for SQL Workload Synthesis for Performance Benchmarking
quality_score: 0.916
content_hash: "sha256:5f2d209d775b924f053f8f59d08d3874813f103cbe624c4b911ef6b53a269757"
concepts: [synql, sql-workload-synthesis, learned-query-optimizer, abstract-syntax-tree, foreign-key-graph, large-language-model, tpc-h, imdb-benchmark, topological-entropy, tree-based-cost-model]
companies: []
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:27:49.381000"
tags: [story, source/rss-feed]
---

## Summary
SynQL is a deterministic, rule-based SQL workload synthesis framework designed to generate structurally diverse and execution-ready SQL queries for database performance benchmarking and learned query optimizer training. It addresses the growing difficulty of obtaining real-world SQL workloads due to privacy regulations and the inadequacy of existing tools, which either rely on too few fixed templates or suffer from LLM-based schema hallucination and topological collapse. SynQL traverses a live database's foreign-key graph to populate an Abstract Syntax Tree, guaranteeing schema and syntactic validity without probabilistic text generation. A configuration vector provides explicit parametric control over join topology, analytical intensity, and predicate selectivity. Experiments on TPC-H and IMDb benchmarks demonstrate near-maximal topological diversity and strong cost model performance (R² ≥ 0.79) with sub-millisecond inference latency.

## Key claims
- Acquiring real-world SQL workloads is increasingly difficult due to strict privacy regulations that strip executable query text from anonymised traces.
- LLM-based SQL synthesis approaches suffer from schema hallucination and topological collapse, producing simplistic join patterns that fail to stress-test query optimisers.
- SynQL generates SQL by traversing a live database's foreign-key graph to populate an Abstract Syntax Tree, guaranteeing schema and syntactic validity by construction.
- A configuration vector Theta in SynQL provides explicit parametric control over join topology (Star, Chain, Fork), analytical intensity, and predicate selectivity.
- SynQL achieves near-maximal workload diversity with a Topological Entropy of 1.53 bits on TPC-H and IMDb benchmarks.
- Tree-based cost models trained on SynQL-generated synthetic corpora achieve R² ≥ 0.79 on held-out synthetic test sets with sub-millisecond inference latency.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2604.08021>

## Related
[[concepts/synql|synql]] · [[concepts/sql-workload-synthesis|sql-workload-synthesis]] · [[concepts/learned-query-optimizer|learned-query-optimizer]] · [[concepts/abstract-syntax-tree|abstract-syntax-tree]] · [[concepts/foreign-key-graph|foreign-key-graph]] · [[concepts/tpc-h|tpc-h]] · [[concepts/topological-entropy|topological-entropy]] · [[concepts/tree-based-cost-model|tree-based-cost-model]] · [[concepts/language-model|language-model]] · [[concepts/sql|sql]] · [[concepts/llm|llm]] · [[episodes/2026-04-10|2026-04-10]]
