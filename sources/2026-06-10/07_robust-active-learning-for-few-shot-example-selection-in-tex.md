---
type: story
story_id: rss_755ca195aa0f
episode_date: 2026-06-10
rank: 7
source: rss_feed
url: "https://arxiv.org/abs/2606.10125"
title: Robust Active Learning for Few-Shot Example Selection in Text-to-SQL
quality_score: 0.796
content_hash: "sha256:2639ad210d18a726d5b4e05ec47a09a700eda3fbd7a566d6602fe32c31872d75"
concepts: [text-to-sql, few-shot-example-selection, active-learning, large-language-models, semantic-query-embeddings, heteroscedastic-mutual-information, partition-matroid-constraints, submodular-optimization, constrained-experimental-design, kernel-misspecification]
companies: []
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-06-10 10:18:50.248000"
tags: [story, source/rss-feed]
---

## Summary
This paper addresses the problem of selecting high-quality few-shot examples for text-to-SQL systems powered by large language models. The authors frame the selection process as a constrained experimental design problem over a low-dimensional semantic embedding manifold. They propose a stratified greedy algorithm that maximizes a heteroscedastic mutual information objective, subject to partition matroid constraints for spatial diversity. The paper proves submodularity and approximate monotonicity of the objective, providing a constant-factor approximation guarantee, and establishes a spectral bound showing graceful degradation under kernel misspecification. Empirical results confirm that the method reduces annotation effort while preserving retrieval accuracy.

## Key claims
- Few-shot example retrieval is the dominant paradigm for grounding LLMs in domain-specific text-to-SQL systems.
- Expert annotation of example banks is prohibitively expensive, motivating active selection methods.
- The authors formalize few-shot example selection as a constrained experimental design problem over a semantic query embedding manifold.
- A stratified greedy algorithm is proposed that maximizes a heteroscedastic mutual information objective under partition matroid constraints.
- The heteroscedastic mutual information objective is proven to be submodular and approximately monotonic on the intrinsic manifold.
- A spectral bound is established showing the approximation guarantee degrades gracefully rather than catastrophically under kernel misspecification.
- Empirical results show the proposed strategy significantly reduces labeling effort while maintaining high text-to-SQL retrieval accuracy.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2606.10125>

## Related
[[concepts/text-to-sql|text-to-sql]] · [[concepts/few-shot-example-selection|few-shot-example-selection]] · [[concepts/active-learning|active-learning]] · [[concepts/large-language-models|large-language-models]] · [[concepts/semantic-query-embeddings|semantic-query-embeddings]] · [[concepts/heteroscedastic-mutual-information|heteroscedastic-mutual-information]] · [[concepts/partition-matroid-constraints|partition-matroid-constraints]] · [[concepts/submodular-optimization|submodular-optimization]] · [[concepts/constrained-experimental-design|constrained-experimental-design]] · [[concepts/embeddings|embeddings]] · [[concepts/llms|llms]] · [[concepts/sql|sql]] · [[episodes/2026-06-10|2026-06-10]]
