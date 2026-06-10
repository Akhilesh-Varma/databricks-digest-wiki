---
type: story
story_id: devto_3528616
episode_date: 2026-04-21
rank: 8
source: devto
url: "https://dev.to/manveer_chawla_64a7283d5a/clickhouse-native-json-support-in-2026-a-pr-by-pr-analysis-1hdp"
title: ClickHouse Native JSON Support in 2026 A PR-by-PR Analysis
quality_score: 0.852
content_hash: "sha256:d88b9a027fe68aa4fc4c2eadfe19d65e82b18680cc76172095d1ecfdd3b0f646"
concepts: [clickhouse, jsonbench, native-json-support]
companies: [clickhouse, mongodb, elasticsearch]
people: []
extractor_model: llama-3.3-70b-versatile
extracted_at: "2026-04-28 04:04:35.064000"
tags: [story, source/devto]
---

## Summary
ClickHouse has full native JSON support since version 25.3, with a columnar implementation that preserves native types and supports primary key indexing. This is a significant improvement over its previous string-based JSON storage, which required full column scans. The new JSON type is 2,500x faster than MongoDB for aggregations on the JSONBench benchmark. The native JSON type has undergone significant development, with 80 merged PRs, and is now production-ready. The legacy type was fully removed in version 25.11.

## Key claims
- ClickHouse has native JSON support since version 25.3
- The JSON type stores each path as a separate columnar subcolumn with native type preservation
- ClickHouse's native JSON type is 2,500x faster than MongoDB for aggregations on the JSONBench benchmark
- The native JSON type supports primary key indexing and selective path reads
- The legacy JSON type was fully removed in version 25.11

## Source
- **Origin:** devto
- **URL:** <https://dev.to/manveer_chawla_64a7283d5a/clickhouse-native-json-support-in-2026-a-pr-by-pr-analysis-1hdp>

## Related
[[concepts/clickhouse|clickhouse]] · [[concepts/jsonbench|jsonbench]] · [[concepts/native-json-support|native-json-support]] · [[concepts/elasticsearch|elasticsearch]] · [[concepts/postgresql|postgresql]] · [[concepts/analytics|analytics]] · [[concepts/indexing|indexing]] · [[concepts/metadata|metadata]] · [[concepts/mongodb|mongodb]] · [[concepts/schema|schema]] · [[concepts/duckdb|duckdb]] · [[concepts/json|json]] · [[companies/clickhouse|ClickHouse]] · [[companies/mongodb|MongoDB]] · [[companies/elasticsearch|Elasticsearch]] · [[episodes/2026-04-21|2026-04-21]]
