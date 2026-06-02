---
type: story
story_id: rss_1f37a3716d30
episode_date: 2026-06-02
rank: 10
source: rss_feed
url: "https://arxiv.org/abs/2606.00774"
title: SCOPE Cost-Efficient Model Selection for Compound AI Systems under Quality Constraints
quality_score: 0.756
content_hash: "sha256:82bb23aec18a0e846f059156be8bfd1d95b6b55a2a0f42704c359f18d8072906"
concepts: [compound-ai-system, llm, large-language-model, optimization-algorithm, quality-threshold, confidence-bounds]
companies: []
people: []
extractor_model: gemini-2.5-flash-lite
extracted_at: "2026-06-02 10:20:53.993000"
tags: [story, source/rss-feed]
---

## Summary
SCOPE is a new optimization algorithm designed to reduce the cost of compound AI systems, which use multiple LLM modules for complex tasks. Existing systems often use a single expensive LLM for all modules, leading to high costs, especially in data management. SCOPE addresses this by selecting diverse LLMs with varying capabilities and pricing for each module to meet quality thresholds at a lower average cost. It achieves this by exploiting per-query results for rapid estimation and using confidence bounds, offering theoretical guarantees and outperforming baselines in evaluations.

## Key claims
- Compound AI systems use multiple LLM modules for complex tasks, but often incur prohibitive costs by using a single expensive LLM across all modules.
- SCOPE is a cost-efficient optimization algorithm for selecting LLMs in compound AI systems to minimize average cost while meeting quality thresholds.
- SCOPE estimates system cost and quality using per-query results, unlike existing methods that rely on expensive dataset-level evaluations.
- SCOPE constructs confidence bounds to guide the search for optimal LLM combinations.
- SCOPE provides theoretical guarantees for meeting quality thresholds and achieving near-optimal average cost.
- Evaluations show SCOPE finds solutions with up to 20 times lower cost during search and up to 6 times lower final cost compared to competitors.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2606.00774>

## Related
[[concepts/compound-ai-system|compound-ai-system]] · [[concepts/llm|llm]] · [[concepts/large-language-model|large-language-model]] · [[concepts/optimization-algorithm|optimization-algorithm]] · [[concepts/quality-threshold|quality-threshold]] · [[concepts/confidence-bounds|confidence-bounds]] · [[concepts/analytics|analytics]] · [[concepts/llms|llms]] · [[concepts/ai|ai]] · [[episodes/2026-06-02|2026-06-02]]
