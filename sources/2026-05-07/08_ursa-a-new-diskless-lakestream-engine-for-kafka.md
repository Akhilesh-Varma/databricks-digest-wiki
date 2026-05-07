---
type: story
story_id: devto_3625613
episode_date: 2026-05-07
rank: 8
source: devto
url: "https://dev.to/kozlovski/ursa-a-new-diskless-lakestream-engine-for-kafka-3l8o"
title: Ursa a new Diskless Lakestream engine for Kafka
quality_score: 0.839
content_hash: "sha256:1926a5595507ea59e480979846cc499400fa5b6f7636cd4b6f2c2827916ad0f5"
concepts: [diskless-topics, apache-kafka, ursa, apache-iceberg, delta-lake, lakestream, kip-352, open-table-format]
companies: [warpstream, amazon-web-services]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-07 10:20:07.108000"
tags: [story, source/devto]
---

## Summary
Ursa is a new diskless lakestream engine being integrated into Apache Kafka via a minimally invasive fork planned to be open-sourced soon. It introduces diskless topics—pioneered by WarpStream—that store data directly in object storage like S3, achieving roughly 10x lower infrastructure costs by eliminating cross-AZ replication traffic and expensive EBS storage. Ursa is natively integrated with Apache Iceberg and Delta Lake, storing topic data in open-table formats without additional ETL jobs or data copies. Unlike some competing approaches, Ursa supports both diskless and traditional topics within the same cluster, toggled per-topic without a full cluster migration. The trade-off of diskless architectures is significantly higher end-to-end latency, typically 1000–2000ms compared to 50–100ms for standard Kafka.

## Key claims
- Ursa is a minimally invasive fork of Apache Kafka that adds diskless topic support without altering the existing codebase paths.
- Diskless Kafka topics store events directly to S3 instead of broker-local disks, making brokers stateless and leaderless.
- WarpStream pioneered the diskless Kafka architecture in 2023, achieving approximately 10x lower infrastructure costs.
- Ursa natively supports Apache Iceberg and Delta Lake, storing topic data in open-table formats without extra ETL jobs or data copies.
- Diskless topics in Ursa can be enabled per-topic with a configuration switch, not a full cluster migration.
- Diskless Kafka architectures incur 10x–20x higher end-to-end latency (1000–2000ms p99) compared to standard Kafka (50–100ms).
- AWS cross-AZ traffic and EBS storage costs are the primary drivers of high infrastructure costs in traditional Kafka deployments.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/kozlovski/ursa-a-new-diskless-lakestream-engine-for-kafka-3l8o>

## Related
[[concepts/diskless-topics|diskless-topics]] · [[concepts/apache-kafka|apache-kafka]] · [[concepts/ursa|ursa]] · [[concepts/apache-iceberg|apache-iceberg]] · [[concepts/delta-lake|delta-lake]] · [[concepts/lakestream|lakestream]] · [[concepts/open-table-format|open-table-format]] · [[concepts/governance|governance]] · [[concepts/explain|explain]] · [[concepts/iceberg|iceberg]] · [[concepts/delta|delta]] · [[concepts/kafka|kafka]] · [[concepts/rest|rest]] · [[concepts/aws|aws]] · [[concepts/etl|etl]] · [[concepts/s3|s3]] · [[companies/warpstream|WarpStream]] · [[companies/amazon-web-services|Amazon Web Services]] · [[episodes/2026-05-07|2026-05-07]]
