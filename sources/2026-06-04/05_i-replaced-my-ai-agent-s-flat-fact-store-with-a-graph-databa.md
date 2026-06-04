---
type: story
story_id: hn_48383578
episode_date: 2026-06-04
rank: 5
source: hacker_news
url: "https://news.ycombinator.com/item?id=48383578"
title: "I Replaced My AI Agent's Flat Fact Store with a Graph Database"
quality_score: 0.761
content_hash: "sha256:6757f402eab6070bc9decdd78e4d4c3f9d1d688c7c94462e6863072f0d19e174"
concepts: [falkordb, localclaw, hnsw-vector-search, supersedes-edge, jsonl-fact-store, named-entity-recognition, ollama, router-specialist-architecture, neo4j, memgraph, qdrant, qwen3-embedding, phi4-mini, redis-wire-protocol]
companies: [devmesh]
people: [peter-green]
extractor_model: claude-sonnet-4-6
extracted_at: "2026-06-04 10:22:08.121000"
tags: [story, source/hacker-news]
---

## Summary
The author describes replacing a JSONL flat fact store in their local AI agent framework, LocalClaw, with FalkorDB, a graph database running in Docker at 85MB. The flat store suffered from near-duplicate facts, inability to traverse relationships between entities, and no temporal versioning of facts. FalkorDB provides native HNSW vector search, graph traversal via ABOUT edges, and temporal fact evolution via SUPERSEDES edges, all in a single container without external dependencies. The author also details a hybrid scoring formula combining vector similarity, recency, and importance tiers, and explains how injecting existing typed entities into NER prompts improved entity extraction consistency over time.

## Key claims
- LocalClaw is a local-model-first AI agent framework running on personal hardware via Ollama with no cloud or API costs.
- The original JSONL flat fact store accumulated 14 near-duplicate facts and could not traverse relationships between entities across multiple hops.
- FalkorDB was chosen over Neo4j and Memgraph because it runs in Docker, uses the Redis wire protocol, supports native HNSW vector search, and fits in 85MB.
- SUPERSEDES edges between facts enable temporal queries, allowing the system to answer what it knew about a topic at a previous point in time.
- Entity extraction reliability improved by injecting existing typed entities from the graph into the NER prompt as reference context before classifying new entities.
- A hybrid scoring formula weights vector similarity at 0.5, recency at 0.2, and importance at 0.3, using a 1-5 importance tier system.
- The author concludes that the model should handle meaning while code handles arithmetic, deduplication, and scoring to avoid unexplainable failures.

## Source
- **Origin:** hacker_news
- **URL:** <https://news.ycombinator.com/item?id=48383578>

## Related
[[concepts/falkordb|falkordb]] · [[concepts/localclaw|localclaw]] · [[concepts/hnsw-vector-search|hnsw-vector-search]] · [[concepts/supersedes-edge|supersedes-edge]] · [[concepts/jsonl-fact-store|jsonl-fact-store]] · [[concepts/named-entity-recognition|named-entity-recognition]] · [[concepts/ollama|ollama]] · [[concepts/vector-search|vector-search]] · [[concepts/vector-index|vector-index]] · [[concepts/embeddings|embeddings]] · [[concepts/ai-agent|ai-agent]] · [[concepts/explain|explain]] · [[concepts/docker|docker]] · [[concepts/cloud|cloud]] · [[concepts/redis|redis]] · [[concepts/spark|spark]] · [[concepts/hnsw|hnsw]] · [[concepts/api|api]] · [[concepts/ai|ai]] · [[companies/devmesh|DevMesh]] · [[people/peter-green|Peter Green]] · [[episodes/2026-06-04|2026-06-04]]
