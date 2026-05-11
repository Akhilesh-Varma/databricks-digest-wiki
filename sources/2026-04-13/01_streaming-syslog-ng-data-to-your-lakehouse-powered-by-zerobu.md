---
type: story
story_id: community_4ea10d2a9f4c
episode_date: 2026-04-13
rank: 1
source: databricks_community
url: "https://community.databricks.com/t5/technical-blog/streaming-syslog-ng-data-to-your-lakehouse-powered-by-zerobus/ba-p/153979"
title: Streaming syslog-ng data to your lakehouse Powered by Zerobus Ingest OTEL
quality_score: 0.78
content_hash: "sha256:599385dc223da43c410bd6638e5c3cea3f2ccefb0cb51a3a9e4a98ea99202c8d"
concepts: [syslog-ng, zerobus-ingest-otel, opentelemetry-protocol-otlp, delta-lake, auto-loader, kafka, grpc, protobuf, oauth2, bsd-syslog-rfc-3164, enhanced-syslog-rfc-5424, journald]
companies: [databricks, zerobus]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:21:20.707000"
tags: [story, source/databricks-community]
---

## Summary
This article describes how to stream syslog-ng log data directly into a Databricks lakehouse using Zerobus Ingest's native OpenTelemetry Protocol (OTLP) endpoint. Syslog-ng is a widely deployed open source log management daemon capable of high-throughput collection, parsing, and forwarding of logs from servers, network devices, IoT fleets, and applications. Previously, getting syslog-ng data into Databricks required intermediate infrastructure such as Kafka or object storage with Auto Loader. With syslog-ng's native OTLP gRPC output (available since version 4.3) and Zerobus Ingest's OTLP endpoint, logs can be sent directly to Delta tables in the lakehouse. The article covers common syslog-ng use cases including centralized log aggregation, security auditing, infrastructure monitoring, application log forwarding, and IoT telemetry.

## Key claims
- syslog-ng has supported native OTLP gRPC output since version 4.3, with performance improvements including batching and multiple workers added in version 4.6.
- Zerobus Ingest now includes a native OTLP gRPC Collector endpoint, enabling direct ingestion of syslog-ng data into a Databricks lakehouse.
- Previously, streaming syslog-ng data into Databricks required intermediate infrastructure such as Kafka, dual-writing to object storage, or custom pipelines.
- syslog-ng supports disk-based buffering to ensure reliable message delivery even when downstream destinations are temporarily unavailable.
- syslog-ng's automatic OAuth2 token management via the cloud-auth block handles token fetching and renewal for cloud destinations without manual intervention.
- Common syslog-ng use cases include centralized log aggregation, security and audit logging, infrastructure monitoring, application log forwarding, and IoT edge telemetry.

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/technical-blog/streaming-syslog-ng-data-to-your-lakehouse-powered-by-zerobus/ba-p/153979>

## Related
[[concepts/syslog-ng|syslog-ng]] · [[concepts/zerobus-ingest-otel|zerobus-ingest-otel]] · [[concepts/opentelemetry-protocol-otlp|opentelemetry-protocol-otlp]] · [[concepts/delta-lake|delta-lake]] · [[concepts/grpc|grpc]] · [[concepts/data-engineering|data-engineering]] · [[concepts/zerobus-ingest|zerobus-ingest]] · [[concepts/data-lakehouse|data-lakehouse]] · [[concepts/object-storage|object-storage]] · [[concepts/opentelemetry|opentelemetry]] · [[concepts/open-source|open-source]] · [[concepts/databricks|databricks]] · [[concepts/telemetry|telemetry]] · [[concepts/lakehouse|lakehouse]] · [[concepts/pipeline|pipeline]] · [[concepts/python|python]] · [[concepts/delta|delta]] · [[concepts/otlp|otlp]] · [[concepts/iot|iot]] · [[companies/databricks|Databricks]] · [[companies/zerobus|Zerobus]] · [[episodes/2026-04-13|2026-04-13]]
