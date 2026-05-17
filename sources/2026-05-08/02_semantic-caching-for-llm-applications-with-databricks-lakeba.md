---
type: story
story_id: community_c388de5c4476
episode_date: 2026-05-08
rank: 2
source: databricks_community
url: "https://community.databricks.com/t5/technical-blog/semantic-caching-for-llm-applications-with-databricks-lakebase/ba-p/151564"
title: Semantic Caching for LLM Applications with Databricks Lakebase and pgvector
quality_score: 0.78
content_hash: "sha256:34a84e06de9327ad2c18765d50bedc8ff9673b17b86bf84153c153b348de9cff"
concepts: [semantic-caching, pgvector, databricks-lakebase, databricks-foundation-model-apis, unity-catalog, hnsw, ivfflat, cosine-similarity, retrieval-augmented-generation, vector-embeddings, sqlalchemy, psycopg2]
companies: [databricks]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-08 10:21:37.345000"
tags: [story, source/databricks-community]
---

## Summary
The article describes how to build a semantic caching layer for LLM-powered applications using Databricks Lakebase (managed PostgreSQL) and the pgvector extension. Instead of exact-match caching, semantic caching embeds user queries into dense vectors and uses cosine similarity to find previously cached responses with the same intent, even if phrased differently. The architecture integrates Databricks Foundation Model APIs for embedding generation, pgvector for similarity search, and Lakebase for managed, autoscaling PostgreSQL storage. The approach reduces both token costs and response latency for repetitive-query workloads such as customer support bots and FAQ assistants. Unity Catalog can be used for governance and access control over the Lakebase databases.

## Key claims
- Semantic caching matches user queries by semantic intent rather than exact keyword overlap, allowing phrases like 'reset my password' and 'recover account credentials' to share a single cached response.
- Databricks Lakebase is a managed, autoscaling PostgreSQL service with pgvector built in, eliminating the need for a separate vector database.
- The caching workflow embeds each incoming prompt using Databricks Foundation Model APIs, searches pgvector for the nearest cached vector, and returns the cached answer on a cache hit above a similarity threshold.
- pgvector supports IVFFlat and HNSW index types with sub-millisecond lookups for datasets ranging from thousands to low millions of vectors.
- Lakebase databases can be registered with Unity Catalog for governance and access control.
- Semantic caching is most beneficial when users ask repetitive questions differently and when answer freshness tolerance is acceptable; it is less useful for truly unique or rapidly changing queries.
- The entire semantic cache implementation can be built in a single Databricks notebook using standard PostgreSQL clients such as psycopg2 or SQLAlchemy.

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/technical-blog/semantic-caching-for-llm-applications-with-databricks-lakebase/ba-p/151564>

## Related
[[concepts/semantic-caching|semantic-caching]] · [[concepts/pgvector|pgvector]] · [[concepts/databricks-lakebase|databricks-lakebase]] · [[concepts/databricks-foundation-model-apis|databricks-foundation-model-apis]] · [[concepts/hnsw|hnsw]] · [[concepts/ivfflat|ivfflat]] · [[concepts/cosine-similarity|cosine-similarity]] · [[concepts/vector-embeddings|vector-embeddings]] · [[concepts/foundation-model|foundation-model]] · [[concepts/vector-database|vector-database]] · [[concepts/semantic-cache|semantic-cache]] · [[concepts/access-control|access-control]] · [[concepts/vector-search|vector-search]] · [[concepts/vector-store|vector-store]] · [[concepts/open-source|open-source]] · [[concepts/autoscaling|autoscaling]] · [[concepts/governance|governance]] · [[concepts/databricks|databricks]] · [[concepts/postgresql|postgresql]] · [[concepts/workflows|workflows]] · [[concepts/lakebase|lakebase]] · [[concepts/postgres|postgres]] · [[concepts/sdk|sdk]] · [[concepts/rag|rag]] · [[concepts/llm|llm]] · [[concepts/ai|ai]] · [[companies/databricks|Databricks]] · [[episodes/2026-05-08|2026-05-08]]
