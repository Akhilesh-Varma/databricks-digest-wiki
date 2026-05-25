---
type: story
story_id: rss_388e4f889bbf
episode_date: 2026-05-25
rank: 6
source: rss_feed
url: "https://arxiv.org/abs/2605.23105"
title: Conceptual Schema Inference for Tabular Datasets using Large Language Models
quality_score: 0.796
content_hash: "sha256:ac6e82640e2e5b2555e410ac56e599016b3edab1bbc3b21f5a5dd2d46319ec90"
concepts: [conceptual-schema-inference, large-language-models, gesi, emsi, table-embeddings, data-lakes, dataset-discovery, hierarchical-type-inference, web-tables]
companies: []
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-25 10:18:32.776000"
tags: [story, source/rss-feed]
---

## Summary
This paper addresses the problem of conceptual schema inference for large, heterogeneous collections of tabular data from data lakes, web tables, and open data portals. The authors propose two LLM-based approaches: GeSI, which uses generative LLMs to infer hierarchical entity types and attributes from table- and column-level semantics, and EmSI, which uses LLM-based table embeddings to cluster tables and construct hierarchical schemas from shared attribute patterns. Both methods operate solely on column headers and cell values without requiring manual annotation. The paper includes an experimental analysis evaluating conciseness, structural quality, and scalability, as well as an end-to-end case study. The work complements prior research on dataset discovery by focusing on the automated derivation of conceptual schemas capturing entity types, attributes, and inter-type relationships.

## Key claims
- Tabular data from data lakes, web tables, and open data portals suffers from representational inconsistencies due to heterogeneous sources.
- GeSI uses generative LLMs to infer hierarchical entity types and attributes from table- and column-level semantics and integrates them into a global schema capturing cross-type relationships.
- EmSI employs LLM-based table embeddings to group tables by column-level semantics and constructs hierarchical structures from shared attribute patterns.
- Both approaches rely only on column headers and cell values, requiring no additional metadata or manual labeling.
- The proposed methods are evaluated on conciseness, structural quality of inferred schema components, and scalability to large repositories.
- Conceptual schema inference is framed as a complementary problem to dataset discovery and exploration in tabular data management.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2605.23105>

## Related
[[concepts/conceptual-schema-inference|conceptual-schema-inference]] · [[concepts/large-language-models|large-language-models]] · [[concepts/gesi|gesi]] · [[concepts/emsi|emsi]] · [[concepts/table-embeddings|table-embeddings]] · [[concepts/data-lakes|data-lakes]] · [[concepts/dataset-discovery|dataset-discovery]] · [[concepts/hierarchical-type-inference|hierarchical-type-inference]] · [[concepts/large-language-model|large-language-model]] · [[concepts/language-model|language-model]] · [[concepts/embeddings|embeddings]] · [[concepts/schema|schema]] · [[concepts/llms|llms]] · [[concepts/llm|llm]] · [[episodes/2026-05-25|2026-05-25]]
