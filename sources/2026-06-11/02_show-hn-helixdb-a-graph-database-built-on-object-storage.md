---
type: story
story_id: hn_48478148
episode_date: 2026-06-11
rank: 2
source: hacker_news
url: "https://github.com/HelixDB/helix-db/tree/main"
title: Show HN HelixDB A graph database built on object storage
quality_score: 0.815
content_hash: "sha256:e6ff905e9b092371bc6152824f1ed2161d7d9a6c8262237a80a849bd23f96b0a"
concepts: [helixdb, graph-database, object-storage, vector-search, full-text-search, graphrag, hybridrag, oltp, amazon-s3, ai-memory, database-sharding, horizontal-scaling]
companies: [helixdb]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-06-11 10:16:56.433000"
tags: [story, source/hacker-news]
---

## Summary
HelixDB is an OLTP graph database built on object storage (S3) with native vector search and full-text search, developed by two college students over the past year. The system addresses the scaling challenges of traditional graph databases by using S3 as the persistence layer, allowing unlimited graph size and horizontal node scaling with local caching for hot data. It targets AI agent workloads that require combining graph traversal, semantic vector search, and full-text filtering in a single system, eliminating the need to stitch together multiple disconnected databases. The team reports p99 latencies of 100ms for writes and 50ms for reads from cold S3 storage, and is working toward a GA cloud offering and an open-source AI memory layer built on HelixDB.

## Key claims
- HelixDB is an OLTP graph database built on object storage (S3) with native vector search and full-text search.
- Using S3 as the persistence layer removes limits on graph size and allows horizontal scaling by spinning up nodes that cache relevant subgraph subsets.
- The system achieves a p99 latency of 100ms for writes and 50ms for reads from cold S3 storage.
- Traditional graph database scaling approaches—full dataset replication or sharding—are either prohibitively expensive or inefficient due to cross-partition edge traversal.
- HelixDB targets AI agent workloads requiring large-scale data storage where only a subset of data is needed at any given time.
- The team is building a generalized open-source AI memory layer that will use HelixDB under the hood.
- Pre-filtering for vector search based on graph relationships, metadata, and sub-graphs is currently in development.

## Source
- **Origin:** hacker_news
- **URL:** <https://github.com/HelixDB/helix-db/tree/main>

## Related
[[concepts/helixdb|helixdb]] · [[concepts/graph-database|graph-database]] · [[concepts/object-storage|object-storage]] · [[concepts/vector-search|vector-search]] · [[concepts/full-text-search|full-text-search]] · [[concepts/graphrag|graphrag]] · [[concepts/hybridrag|hybridrag]] · [[concepts/oltp|oltp]] · [[concepts/amazon-s3|amazon-s3]] · [[concepts/ai-memory|ai-memory]] · [[concepts/database-sharding|database-sharding]] · [[concepts/horizontal-scaling|horizontal-scaling]] · [[concepts/relational-databases|relational-databases]] · [[concepts/vector-databases|vector-databases]] · [[concepts/memory-layer|memory-layer]] · [[concepts/ai-agents|ai-agents]] · [[concepts/metadata|metadata]] · [[concepts/having|having]] · [[concepts/cloud|cloud]] · [[concepts/ai|ai]] · [[concepts/s3|s3]] · [[companies/helixdb|HelixDB]] · [[episodes/2026-06-11|2026-06-11]]
