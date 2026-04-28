---
type: story
story_id: rss_b593e3959090
episode_date: 2026-04-23
rank: 10
source: rss_feed
url: "https://arxiv.org/abs/2604.20121"
title: A GPU-Accelerated Framework for Multi-Attribute Range Filtered Approximate Nearest Neighbor Search
quality_score: 0.716
content_hash: "sha256:9ba85b894fbcc8e8efaf7cb1b09c9c5549afa03805cec4cb5e7e7e182af0607b"
concepts: [garfield, gmg-index, range-filtered-approximate-nearest-neighbor-search]
companies: []
people: []
extractor_model: llama-3.3-70b-versatile
extracted_at: "2026-04-28 04:01:44.649000"
tags: [story, source/rss-feed]
---

## Summary
The paper introduces Garfield, a GPU-accelerated framework for multi-attribute range filtered approximate nearest neighbor search. Garfield overcomes existing bottlenecks by designing a lightweight index structure and hardware-aware execution pipeline. It achieves this through the GMG index, which partitions data into cells and builds local graph indexes. Garfield reduces index size and delivers higher throughput than state-of-the-art methods. The framework is designed to handle large datasets and leverages the computational capabilities of GPUs.

## Key claims
- Garfield is a GPU-accelerated framework for multi-attribute range filtered approximate nearest neighbor search.
- The framework introduces the GMG index, which partitions data into cells and builds local graph indexes.
- Garfield reduces index size by 4.4x compared to state-of-the-art RFANNS methods.
- Garfield delivers 119.8x higher throughput than state-of-the-art RFANNS methods.
- The framework features a cell-oriented out-of-core pipeline to handle large datasets.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2604.20121>

## Related
[[concepts/garfield|garfield]] · [[concepts/gmg-index|gmg-index]] · [[concepts/range-filtered-approximate-nearest-neighbor-search|range-filtered-approximate-nearest-neighbor-search]] · [[concepts/pipeline|pipeline]] · [[concepts/linear|linear]] · [[episodes/2026-04-23|2026-04-23]]
