---
type: story
story_id: rss_1cfd8353fb5b
episode_date: 2026-06-11
rank: 3
source: rss_feed
url: "https://docs.databricks.com/aws/en/release-notes/runtime/18#databricks-runtime-18-june-10-2026"
title: "Databricks Runtime 18 June 10, 2026"
quality_score: 0.886
content_hash: "sha256:b9778267fbd0d1fb877699297a603fb725144f5a59d20447136323096bf8b7e6"
concepts: [databricks-runtime, lakeflow-spark-declarative-pipelines, structured-streaming, apache-spark, photon, parquet, on-demand-state-repartitioning]
companies: [databricks, apache-software-foundation]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-06-11 10:17:13.687000"
tags: [story, source/rss-feed]
---

## Summary
Databricks Runtime 18 reached general availability on June 10, 2026, introducing several new features and bug fixes. Notable additions include the ability to set streaming query IDs on demand in Lakeflow Spark Declarative Pipelines, new SQL functions for working with IPv4, IPv6, and CIDR blocks, and on-demand state repartitioning for stateful Structured Streaming queries. The release also ships Apache Spark bug fixes, including corrected null handling in LEFT OUTER JOIN LATERAL expressions with EXPLODE and improved Parquet schema resolution behavior in Photon.

## Key claims
- Databricks Runtime 18 is generally available as of June 10, 2026.
- Lakeflow Spark Declarative Pipelines can now set the streaming query ID on demand.
- New SQL functions for IPv4, IPv6, and CIDR block operations are available in Public Preview, including ip_host, ip_cidr, ip_version, and related variants.
- On-demand state repartitioning for stateful Structured Streaming queries is available in Public Preview, allowing shuffle partition count changes without losing checkpoint state.
- A bug causing incorrect null handling in LEFT OUTER JOIN LATERAL expressions containing EXPLODE has been fixed.
- Photon now defers duplicate field_id errors in Parquet schema resolution until the affected field is actually accessed.

## Source
- **Origin:** rss_feed
- **URL:** <https://docs.databricks.com/aws/en/release-notes/runtime/18#databricks-runtime-18-june-10-2026>

## Related
[[concepts/databricks-runtime|databricks-runtime]] · [[concepts/lakeflow-spark-declarative-pipelines|lakeflow-spark-declarative-pipelines]] · [[concepts/structured-streaming|structured-streaming]] · [[concepts/apache-spark|apache-spark]] · [[concepts/photon|photon]] · [[concepts/on-demand-state-repartitioning|on-demand-state-repartitioning]] · [[concepts/spark-declarative-pipelines|spark-declarative-pipelines]] · [[concepts/left-outer-join-lateral|left-outer-join-lateral]] · [[concepts/declarative-pipelines|declarative-pipelines]] · [[concepts/databricks-runtime-18|databricks-runtime-18]] · [[concepts/databricks|databricks]] · [[concepts/streaming|streaming]] · [[concepts/lakeflow|lakeflow]] · [[concepts/shuffle|shuffle]] · [[concepts/schema|schema]] · [[concepts/spark|spark]] · [[concepts/sql|sql]] · [[companies/databricks|Databricks]] · [[companies/apache-software-foundation|Apache Software Foundation]] · [[episodes/2026-06-11|2026-06-11]]
