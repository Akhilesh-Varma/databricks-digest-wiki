---
type: story
story_id: rss_f629aba6cef3
episode_date: 2026-05-18
rank: 10
source: rss_feed
url: "https://arxiv.org/abs/2605.15957"
title: To GPU or Not to GPU Vector Search in Relational Engines
quality_score: 0.796
content_hash: "sha256:24a33d4a11be6e7c3517c318369a1e082deaec8a38df21f5b3eb5c0379688273"
concepts: [vector-search, tpc-h-benchmark, gpu-accelerated-query-processing, vector-index, nvlink, pcie, embeddings, sql, relational-database-engine]
companies: []
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-18 10:21:01.233000"
tags: [story, source/rss-feed]
---

## Summary
This paper investigates whether integrating GPU-based vector processing into relational database engines offers advantages over traditional CPU-based approaches for vector search workloads. The authors extend the TPC-H benchmark with vector data from text and images and define representative SQL vector search queries. They build a modular execution engine capable of running these queries on both CPU and GPU configurations, testing across various memory layouts, index types, and interconnects including PCIe and NVLink. Counter-intuitively, they find that relational components benefit more from GPU acceleration than the vector search components themselves, and that data movement costs can negate GPU advantages. By redesigning the vector index organization to reduce index size, they ultimately achieve faster performance for both relational and vector search components on the GPU, especially over fast interconnects.

## Key claims
- Most existing database engines implement vector search on CPUs, even though GPUs dominate AI/ML and LLM workloads.
- The authors extend the TPC-H benchmark with vector data from text and images to create representative SQL vector search queries.
- A modular execution engine was developed to run SQL vector search queries across both CPU and GPU.
- Relational query components benefit more from GPU acceleration than the vector search components themselves.
- When vector search requires moving data and indexes across interconnects, using the GPU is not always the best option even with fast interconnects like NVLink.
- A redesigned vector index organization reduces index size, making GPU-based vector search more competitive.
- With the proposed improvements, both relational and vector search components run faster on the GPU, particularly on fast interconnects.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2605.15957>

## Related
[[concepts/vector-search|vector-search]] · [[concepts/tpc-h-benchmark|tpc-h-benchmark]] · [[concepts/gpu-accelerated-query-processing|gpu-accelerated-query-processing]] · [[concepts/vector-index|vector-index]] · [[concepts/nvlink|nvlink]] · [[concepts/embeddings|embeddings]] · [[concepts/sql|sql]] · [[concepts/relational-database-engine|relational-database-engine]] · [[concepts/tpc-h|tpc-h]] · [[concepts/llms|llms]] · [[concepts/ai|ai]] · [[episodes/2026-05-18|2026-05-18]]
