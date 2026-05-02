---
type: story
story_id: community_8327bc3acabe
episode_date: 2026-04-18
rank: 4
source: databricks_community
url: "https://community.databricks.com/t5/technical-blog/your-telemetry-your-lakehouse-introducing-native-opentelemetry/ba-p/153976"
title: "Your Telemetry, Your Lakehouse Introducing Native OpenTelemetry Support in Zerobus Ingest"
quality_score: 0.74
content_hash: "sha256:7c585be0e2953df2b667e764e9f09c71de3a10c4ca5c4793b80d04a169833b38"
concepts: [zerobus-ingest, opentelemetry-protocol-otlp, opentelemetry, unity-catalog, delta-tables, opentelemetry-collector, auto-loader, fluent-bit, telegraf, syslog-ng, apache-kafka]
companies: [databricks]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:06:07.863000"
tags: [story, source/databricks-community]
---

## Summary
Databricks has announced that Zerobus Ingest now natively supports the OpenTelemetry Protocol (OTLP), enabling teams to stream traces, logs, and metrics directly into Unity Catalog Delta tables. Previously, getting OpenTelemetry telemetry data into a lakehouse required workarounds such as extracting from third-party vendors, dual-writing to object storage, or routing through Kafka. The new Zerobus Ingest OTEL integration acts as the OTLP backend, replacing proprietary observability vendors and eliminating the need for custom libraries or intermediary pipelines. The feature is currently available in Beta and works with standard OpenTelemetry SDKs and collectors already in use by most teams.

## Key claims
- Zerobus Ingest now natively supports the OpenTelemetry Protocol (OTLP), allowing telemetry data to flow directly into Unity Catalog Delta tables.
- Zerobus Ingest OTEL is available in Beta and supports streaming of traces, logs, and metrics.
- No custom libraries or intermediary pipelines are required when using Zerobus Ingest OTEL with standard OpenTelemetry SDKs and collectors.
- Previously, teams had to rely on extracting data from third-party vendors, dual-writing to object storage, or using Kafka as an intermediary to get telemetry into Databricks.
- OpenTelemetry is described as the dominant open source framework for observability, with SDKs for every major programming language.
- Zerobus Ingest OTEL serves as the OTLP backend endpoint that collectors point to, replacing proprietary observability vendor backends.

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/technical-blog/your-telemetry-your-lakehouse-introducing-native-opentelemetry/ba-p/153976>

## Related
[[concepts/zerobus-ingest|zerobus-ingest]] · [[concepts/opentelemetry-protocol-otlp|opentelemetry-protocol-otlp]] · [[concepts/opentelemetry|opentelemetry]] · [[concepts/unity-catalog|unity-catalog]] · [[concepts/delta-tables|delta-tables]] · [[concepts/opentelemetry-collector|opentelemetry-collector]] · [[concepts/zerobus-ingest-otel|zerobus-ingest-otel]] · [[concepts/open-source|open-source]] · [[concepts/databricks|databricks]] · [[concepts/telemetry|telemetry]] · [[concepts/lakehouse|lakehouse]] · [[concepts/pipeline|pipeline]] · [[concepts/parquet|parquet]] · [[concepts/delta|delta]] · [[concepts/kafka|kafka]] · [[concepts/otlp|otlp]] · [[concepts/s3|s3]] · [[companies/databricks|Databricks]] · [[episodes/2026-04-18|2026-04-18]]
