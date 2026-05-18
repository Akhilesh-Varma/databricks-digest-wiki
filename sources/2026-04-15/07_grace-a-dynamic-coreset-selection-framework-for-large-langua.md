---
type: story
story_id: rss_ac51f284ec90
episode_date: 2026-04-15
rank: 7
source: rss_feed
url: "https://arxiv.org/abs/2604.11810"
title: GRACE A Dynamic Coreset Selection Framework for Large Language Model Optimization
quality_score: 0.836
content_hash: "sha256:621001c68b9af92816682f9cafcec5ecc8e4e1d0c3b5fdf8f7dbccdd305ebf66"
concepts: [grace, coreset-selection, large-language-models, transformer-architecture, k-nn-graph, gradient-based-importance-metrics]
companies: []
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:17:25.858000"
tags: [story, source/rss-feed]
---

## Summary
The paper introduces GRACE, a graph-guided adaptive and dynamic coreset selection framework designed to optimize Large Language Model training. Existing coreset selection methods struggle to adapt to the dynamic nature of LLM training and face scalability challenges. GRACE addresses these issues by dynamically constructing and updating coresets using representation diversity combined with gradient-based importance metrics. It employs a k-NN graph-based propagation mechanism to reduce the computational cost of frequent updates. Experiments on three benchmarks show GRACE improves both training efficiency and downstream task performance across multiple LLMs.

## Key claims
- Existing coreset selection methods fail to adapt to the dynamic nature of LLM training and struggle with scalability.
- GRACE dynamically constructs and updates coresets by combining representation diversity with gradient-based importance metrics.
- GRACE uses a k-NN graph-based propagation mechanism to reduce the computational cost of frequent score and embedding updates.
- GRACE is evaluated on three benchmarks across diverse LLMs and tasks.
- GRACE significantly improves training efficiency and downstream performance compared to existing methods.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2604.11810>

## Related
[[concepts/grace|grace]] · [[concepts/coreset-selection|coreset-selection]] · [[concepts/large-language-models|large-language-models]] · [[concepts/transformer-architecture|transformer-architecture]] · [[concepts/k-nn-graph|k-nn-graph]] · [[concepts/gradient-based-importance-metrics|gradient-based-importance-metrics]] · [[concepts/embeddings|embeddings]] · [[concepts/optimize|optimize]] · [[concepts/llms|llms]] · [[concepts/llm|llm]] · [[episodes/2026-04-15|2026-04-15]]
