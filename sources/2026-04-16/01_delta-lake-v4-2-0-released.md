---
type: story
story_id: github_release_delta-io_delta_309660403
episode_date: 2026-04-16
rank: 1
source: github_releases
url: "https://github.com/delta-io/delta/releases/tag/v4.2.0"
title: Delta Lake v4.2.0 released
quality_score: 0.857
content_hash: "sha256:ddc781ec78d6745d27a54359eeb10bbe417237b4cc4f4fd6d2300e816d39ebfe"
concepts: [delta-lake, unity-catalog, delta-kernel, apache-spark, apache-flink, delta-spark-v2-connector, kernel-based-flink-connector, dynamic-partition-overwrite, variant-column, replace-table-rtas]
companies: [delta-io-linux-foundation]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:11:34.460000"
tags: [story, source/github-releases]
---

## Summary
Delta Lake 4.2.0 has been released with significant new features across its Spark, Flink, and Kernel components. Key highlights include enhancements to Unity Catalog Managed Table support, an experimental Kernel-based Flink connector for reading and writing catalog-managed Delta tables, and general availability of Variant columns and Geospatial types in Delta Kernel. The release also introduces improved security hardening, including stronger validation and dependency security scanning to reduce supply-chain risk. Delta Spark 4.2.0 is built on Apache Spark 4.1.0 and 4.0.1.

## Key claims
- Delta Lake 4.2.0 introduces REPLACE TABLE RTAS and Dynamic Partition Overwrite support for Unity Catalog Managed Tables.
- A new experimental Kernel-based Flink connector enables Apache Flink to read, write, and interact with catalog-managed Delta tables.
- Delta Kernel now supports Geospatial types (geometry and geography) with bounding-box data skipping as a new feature.
- Variant columns and collated string types are now generally available in Delta Kernel.
- The Delta Spark V2 connector gains experimental enhanced streaming read capabilities, including startingTimestamp and skipChangeCommits options.
- Delta Lake 4.2.0 underwent security hardening with stronger validation and dependency security scanning to reduce supply-chain risk.
- Delta Spark 4.2.0 is built on Apache Spark 4.1.0 and Apache Spark 4.0.1.

## Source
- **Origin:** github_releases
- **URL:** <https://github.com/delta-io/delta/releases/tag/v4.2.0>

## Related
[[concepts/delta-lake|delta-lake]] · [[concepts/unity-catalog|unity-catalog]] · [[concepts/delta-kernel|delta-kernel]] · [[concepts/apache-spark|apache-spark]] · [[concepts/apache-flink|apache-flink]] · [[concepts/delta-spark-v2-connector|delta-spark-v2-connector]] · [[concepts/kernel-based-flink-connector|kernel-based-flink-connector]] · [[concepts/data-skipping|data-skipping]] · [[concepts/delta-tables|delta-tables]] · [[concepts/streaming|streaming]] · [[concepts/schema|schema]] · [[concepts/delta|delta]] · [[concepts/spark|spark]] · [[companies/delta-io-linux-foundation|Delta.io (Linux Foundation)]] · [[episodes/2026-04-16|2026-04-16]]
