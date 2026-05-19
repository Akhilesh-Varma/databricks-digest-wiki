---
type: story
story_id: devto_3594245
episode_date: 2026-05-01
rank: 9
source: devto
url: "https://dev.to/jaksontate/how-to-migrate-mysql-to-clickhouse-with-zero-downtime-hl2"
title: How to Migrate MySQL to ClickHouse with Zero Downtime
quality_score: 0.817
content_hash: "sha256:5794c610e6bf92307921ab5dfa861c95cfdf2d470a707845fc6c627a14e8176c"
concepts: [change-data-capture, materializedmysql, debezium, redpanda, clickhouse, mysql-binary-logs, bare-metal-deployment, apache-kafka, clickpipes]
companies: [clickhouse, confluent, redpanda]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-01 10:20:43.125000"
tags: [story, source/devto]
---

## Summary
This article provides a guide for migrating MySQL to ClickHouse with zero downtime using a Change Data Capture (CDC) pipeline built on Debezium and Redpanda on bare metal servers. It warns against using the now-deprecated MaterializedMySQL engine, which was removed in ClickHouse version 24.12 due to instability at scale. The author argues that managed SaaS platforms like Confluent Cloud introduce high egress costs and latency, making bare metal deployments preferable. The guide covers schema mapping, historical data snapshots, and live CDC streaming as a multi-phase migration blueprint. Key pitfalls such as tombstone handling, storage tax, and fault tolerance during cutover are also addressed.

## Key claims
- ClickHouse officially deprecated and removed the MaterializedMySQL engine in version 24.12.
- MaterializedMySQL failed to handle complex schema migrations and crashed under heavy replication loads.
- Change Data Capture (CDC) is described as the enterprise standard for zero-downtime MySQL-to-ClickHouse replication.
- Using managed SaaS platforms like Confluent Cloud for CDC can result in high network egress fees when syncing terabytes across cloud regions.
- Hosting Redpanda and ClickHouse on bare metal servers co-located with the MySQL source ensures sub-millisecond latency and avoids per-gigabyte cloud billing.
- Debezium reads MySQL binary logs and pushes change events to a message broker such as Redpanda.
- Engineers must manually map MySQL data types to ClickHouse types, carefully handling nulls, financial decimals, and timezones.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/jaksontate/how-to-migrate-mysql-to-clickhouse-with-zero-downtime-hl2>

## Related
[[concepts/change-data-capture|change-data-capture]] · [[concepts/materializedmysql|materializedmysql]] · [[concepts/debezium|debezium]] · [[concepts/redpanda|redpanda]] · [[concepts/clickhouse|clickhouse]] · [[concepts/mysql-binary-logs|mysql-binary-logs]] · [[concepts/bare-metal-deployment|bare-metal-deployment]] · [[concepts/streaming-pipeline|streaming-pipeline]] · [[concepts/data-engineering|data-engineering]] · [[concepts/schema-mapping|schema-mapping]] · [[concepts/egress-fees|egress-fees]] · [[concepts/snapshot|snapshot]] · [[concepts/pipeline|pipeline]] · [[concepts/schema|schema]] · [[concepts/kafka|kafka]] · [[concepts/mysql|mysql]] · [[concepts/saas|saas]] · [[companies/clickhouse|ClickHouse]] · [[companies/confluent|Confluent]] · [[companies/redpanda|Redpanda]] · [[episodes/2026-05-01|2026-05-01]]
