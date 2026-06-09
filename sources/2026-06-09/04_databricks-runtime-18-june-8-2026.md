---
type: story
story_id: rss_98430b98c458
episode_date: 2026-06-09
rank: 4
source: rss_feed
url: "https://docs.databricks.com/aws/en/release-notes/runtime/18#databricks-runtime-18-june-8-2026"
title: "Databricks Runtime 18 June 8, 2026"
quality_score: 0.766
content_hash: "sha256:cc0431a362e4f2a08b63a454d2a9b5832e45f8ffc444df8231999d0fbad76216"
concepts: [apache-spark, databricks-runtime, nearest-by, dsv2-data-source-v2, sql-path, partialmerge-aggregate-execution, bounded-k-way-merging, v2-catalog-tables]
companies: [databricks, apache-software-foundation]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-06-09 10:16:44.408000"
tags: [story, source/rss-feed]
---

## Summary
Databricks Runtime 18 (released June 8, 2026) introduces several Apache Spark bug fixes and improvements. Notable additions include support for NEAREST BY as a SQL join type for top-K nearest-neighbor queries, DESCRIBE TABLE ... PARTITION support for v2 catalog tables, and extended SQL PATH support via SET PATH and CURRENT_PATH. UPDATE queries on DSv2 tables now expose operation metrics, and DSv2 partition predicates support nested partition columns. Additionally, a bug affecting aggregate queries with PartialMerge or Final execution was fixed, and large external sorts now use bounded k-way merging to reduce out-of-memory errors.

## Key claims
- NEAREST BY is now a supported SQL join type for top-K nearest-neighbor queries in Databricks Runtime 18.
- DESCRIBE TABLE ... PARTITION is now supported for v2 catalog tables, previously only available for v1 tables.
- SET PATH is now a supported SQL statement, and CURRENT_PATH returns the current SQL path.
- SQL PATH is now persisted in view and SQL function definitions and included in DESCRIBE output.
- UPDATE queries on DSv2 tables now include operation metrics in query output.
- A bug causing aggregate queries using PartialMerge or Final aggregate execution to fail due to missing required input attributes has been fixed.
- Large external sorts now use bounded k-way merging to reduce out-of-memory errors when spilling data to disk.

## Source
- **Origin:** rss_feed
- **URL:** <https://docs.databricks.com/aws/en/release-notes/runtime/18#databricks-runtime-18-june-8-2026>

## Related
[[concepts/apache-spark|apache-spark]] · [[concepts/databricks-runtime|databricks-runtime]] · [[concepts/nearest-by|nearest-by]] · [[concepts/dsv2-data-source-v2|dsv2-data-source-v2]] · [[concepts/sql-path|sql-path]] · [[concepts/v2-catalog-tables|v2-catalog-tables]] · [[concepts/spark|spark]] · [[concepts/sql|sql]] · [[companies/databricks|Databricks]] · [[companies/apache-software-foundation|Apache Software Foundation]] · [[episodes/2026-06-09|2026-06-09]]
