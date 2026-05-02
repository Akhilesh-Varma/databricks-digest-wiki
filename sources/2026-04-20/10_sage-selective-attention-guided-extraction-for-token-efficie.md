---
type: story
story_id: rss_1ea298413167
episode_date: 2026-04-20
rank: 10
source: rss_feed
url: "https://arxiv.org/abs/2604.15583"
title: SAGE Selective Attention-Guided Extraction for Token-Efficient
quality_score: 0.876
content_hash: "sha256:a0955238ee057e95515bcd14d9fa15bfa75563298eafbb02801b9eefc78daecf"
concepts: [selective-attention-guided-extraction, retrieval-augmented-generation, language-model]
companies: []
people: []
extractor_model: llama-3.3-70b-versatile
extracted_at: "2026-04-28 04:06:31.040000"
tags: [story, source/rss-feed]
---

## Summary
The paper introduces SAGE, a training-free context reduction framework that uses a lightweight local language model to convert attention signals into a query-specific relevance heatmap. This heatmap is then used to select the top-scoring units under a user-defined token budget, reducing the context and improving answer quality. SAGE surpasses traditional reduction techniques across multiple long-document QA benchmarks, enabling a 90% reduction in tokens with competitive accuracy. The framework is designed to address the limitations of fixed position heuristics and standard retrieval-augmented generation. SAGE achieves a top-4 rank on QuALITY-hard while constrained to a 10 context budget.

## Key claims
- SAGE is a training-free, plug-and-play context reduction framework.
- SAGE uses a lightweight local language model to convert attention signals into a query-specific relevance heatmap.
- SAGE introduces differential attention strategies to better isolate question-relevant evidence.
- SAGE enables a 90% reduction in tokens with competitive accuracy.
- SAGE surpasses traditional reduction techniques across multiple long-document QA benchmarks.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2604.15583>

## Related
[[concepts/selective-attention-guided-extraction|selective-attention-guided-extraction]] · [[concepts/retrieval-augmented-generation|retrieval-augmented-generation]] · [[concepts/language-model|language-model]] · [[concepts/large-language-models|large-language-models]] · [[concepts/semantic-similarity|semantic-similarity]] · [[concepts/rag|rag]] · [[concepts/llm|llm]] · [[episodes/2026-04-20|2026-04-20]]
