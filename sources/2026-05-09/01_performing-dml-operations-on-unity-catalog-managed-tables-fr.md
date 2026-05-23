---
type: story
story_id: community_4b4eb2264d82
episode_date: 2026-05-09
rank: 1
source: databricks_community
url: "https://community.databricks.com/t5/technical-blog/performing-dml-operations-on-unity-catalog-managed-tables-from/ba-p/156308"
title: Performing DML Operations on Unity Catalog Managed Tables from External Engines
quality_score: 0.78
content_hash: "sha256:e7328a5119a1d669044d41f2e8afcd7268e27a1b8195300dfa9b00100d05c488"
concepts: [unity-catalog, catalog-commits, delta-lake, delta-kernel, apache-spark-structured-streaming, apache-spark, duckdb, apache-flink, iceberg-rest, predictive-optimization, m2m-oauth, delta-table-transaction-log, multi-table-transactions]
companies: [databricks, starburst, streamnative, apache-software-foundation]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-09 10:18:25.798000"
tags: [story, source/databricks-community]
---

## Summary
Databricks has released a Beta feature enabling external engines—including Apache Spark, DuckDB, Apache Flink, Starburst, and StreamNative Kafka Service—to perform full DML operations (create, read, write) on Unity Catalog-managed Delta tables outside of Databricks. Unity Catalog acts as a centralized commit coordinator through 'Catalog Commits,' serializing transactions across engines to prevent log corruption and maintain consistency. The feature ships with Delta Lake 4.2.0 and Unity Catalog 0.4.1, requires granting EXTERNAL_USE_SCHEMA and M2M OAuth authentication, and uses the Unity Catalog REST API. Predictive Optimization continues to manage table health (compaction, vacuuming, statistics) even when tables are written by external engines. This extends Unity Catalog's open interoperability vision, complementing existing Iceberg REST support for managed Iceberg tables.

## Key claims
- External engines including Apache Spark, DuckDB, Apache Flink, Starburst, and StreamNative Kafka Service can now create, read, and write Unity Catalog-managed Delta tables from outside Databricks.
- Unity Catalog acts as a centralized commit coordinator (Catalog Commits), serializing all external writes to prevent transaction log corruption.
- The feature ships with Delta Lake 4.2.0 and Unity Catalog 0.4.1.
- External access requires granting EXTERNAL_USE_SCHEMA permission and authenticating via M2M OAuth through the Unity Catalog REST API.
- Predictive Optimization (compaction, vacuuming, statistics) continues to function on tables written entirely by external engines.
- Managed Iceberg tables already support external writes through Iceberg REST in Public Preview, meaning both open formats under Unity Catalog now offer full external read/write/create.
- Delta Kernel is the open-source library that enables connector authors to implement catalog-commits-based external access.

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/technical-blog/performing-dml-operations-on-unity-catalog-managed-tables-from/ba-p/156308>

## Related
[[concepts/unity-catalog|unity-catalog]] · [[concepts/catalog-commits|catalog-commits]] · [[concepts/delta-lake|delta-lake]] · [[concepts/delta-kernel|delta-kernel]] · [[concepts/apache-spark-structured-streaming|apache-spark-structured-streaming]] · [[concepts/apache-spark|apache-spark]] · [[concepts/duckdb|duckdb]] · [[concepts/apache-flink|apache-flink]] · [[concepts/iceberg-rest|iceberg-rest]] · [[concepts/predictive-optimization|predictive-optimization]] · [[concepts/m2m-oauth|m2m-oauth]] · [[concepts/delta-table-transaction-log|delta-table-transaction-log]] · [[concepts/structured-streaming|structured-streaming]] · [[concepts/credential-vending|credential-vending]] · [[concepts/transaction-log|transaction-log]] · [[concepts/data-lakehouse|data-lakehouse]] · [[concepts/delta-tables|delta-tables]] · [[concepts/open-source|open-source]] · [[concepts/governance|governance]] · [[concepts/databricks|databricks]] · [[concepts/compaction|compaction]] · [[concepts/lakehouse|lakehouse]] · [[concepts/snapshot|snapshot]] · [[concepts/rest-api|rest-api]] · [[concepts/iceberg|iceberg]] · [[concepts/delta|delta]] · [[concepts/oauth|oauth]] · [[concepts/kafka|kafka]] · [[concepts/spark|spark]] · [[concepts/rest|rest]] · [[concepts/sdk|sdk]] · [[concepts/api|api]] · [[concepts/dml|dml]] · [[concepts/uc|uc]] · [[companies/databricks|Databricks]] · [[companies/starburst|Starburst]] · [[companies/streamnative|StreamNative]] · [[companies/apache-software-foundation|Apache Software Foundation]] · [[episodes/2026-05-09|2026-05-09]]
