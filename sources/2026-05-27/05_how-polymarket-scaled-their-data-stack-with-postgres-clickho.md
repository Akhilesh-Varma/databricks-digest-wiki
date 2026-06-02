---
type: story
story_id: devto_3762603
episode_date: 2026-05-27
rank: 5
source: devto
url: "https://dev.to/nevosaynevo/how-polymarket-scaled-their-data-stack-with-postgres-clickhouse-4982"
title: How Polymarket Scaled Their Data Stack with Postgres ClickHouse
quality_score: 0.939
content_hash: "sha256:20598cbdb0f671aa59b22c8a85189599c5ff2b6f86171faa11b93f8697153624"
concepts: [clickhouse, postgresql, materialized-views, oltp, olap, clickpipes, goldsky-subgraphs, columnar-database, dbt, data-warehouse]
companies: [polymarket, goldsky]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-27 10:18:57.101000"
tags: [story, source/devto]
---

## Summary
Polymarket, a prediction market platform with billions in monthly trading volume, faced severe performance issues as analytical workloads overwhelmed their PostgreSQL database, causing dashboard timeouts and leaderboard slowdowns. They adopted a hybrid architecture by keeping PostgreSQL for transactional (OLTP) workloads and introducing ClickHouse as a dedicated columnar analytics engine for OLAP workloads. Data is ingested into ClickHouse via three paths: on-chain trading data through Goldsky subgraphs, web analytics from S3 via ClickPipes, and off-chain metadata synced from Postgres. Rewriting the leaderboard using ClickHouse materialized views reduced query times from timeouts to sub-50ms, with the API now handling hundreds of requests per second at 25ms average latency. The case illustrates the value of separating OLTP and OLAP concerns early and using purpose-built tools for each workload type.

## Key claims
- Polymarket grew to billions in dollars of monthly trading volume, causing PostgreSQL analytical queries to time out.
- Polymarket adopted ClickHouse as a dedicated columnar analytics engine while retaining PostgreSQL for transactional workloads.
- On-chain trading data is ingested into ClickHouse via Goldsky subgraphs streaming.
- Web analytics are loaded from S3 into ClickHouse using ClickPipes.
- Rewriting the leaderboard with ClickHouse materialized views reduced query latency from timeouts to sub-50ms.
- The leaderboard API now handles hundreds of requests per second at an average latency of 25ms.
- The hybrid architecture enabled cheaper development of new leaderboard categories and dashboards.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/nevosaynevo/how-polymarket-scaled-their-data-stack-with-postgres-clickhouse-4982>

## Related
[[concepts/clickhouse|clickhouse]] · [[concepts/postgresql|postgresql]] · [[concepts/materialized-views|materialized-views]] · [[concepts/oltp|oltp]] · [[concepts/olap|olap]] · [[concepts/clickpipes|clickpipes]] · [[concepts/goldsky-subgraphs|goldsky-subgraphs]] · [[concepts/columnar-database|columnar-database]] · [[concepts/data-warehouse|data-warehouse]] · [[concepts/real-time-analytics|real-time-analytics]] · [[concepts/warehouse|warehouse]] · [[concepts/analytics|analytics]] · [[concepts/streaming|streaming]] · [[concepts/postgres|postgres]] · [[concepts/metadata|metadata]] · [[concepts/views|views]] · [[concepts/api|api]] · [[concepts/s3|s3]] · [[companies/polymarket|Polymarket]] · [[companies/goldsky|Goldsky]] · [[episodes/2026-05-27|2026-05-27]]
