---
type: story
story_id: rss_60af579b3839
episode_date: 2026-05-30
rank: 3
source: rss_feed
url: "https://docs.databricks.com/aws/en/release-notes/runtime/18#databricks-runtime-18-may-29-2026"
title: "Databricks Runtime 18 May 29, 2026"
quality_score: 0.806
content_hash: "sha256:643f916a1a7c4abda77153547f7a4881c5b51cf762e092f7855fd2834454cbd2"
concepts: [databricks-runtime, structured-streaming, unity-catalog, foreign-catalog-tables]
companies: [databricks, snowflake]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-30 10:17:53.856000"
tags: [story, source/rss-feed]
---

## Summary
Databricks Runtime 18 (released May 29, 2026) introduces two notable fixes. First, Structured Streaming deduplication now correctly treats NaN values with different bit patterns as duplicates when a double or float column is used as a deduplication key, closing a gap where distinct NaN representations were not deduplicated. Second, a bug was fixed where table-level permissions on Unity Catalog foreign catalog tables (such as Snowflake connection tables) could be inadvertently removed during metadata refresh, causing INSUFFICIENT_PERMISSIONS errors. Permissions are now preserved across foreign table metadata refreshes.

## Key claims
- Databricks Runtime 18 was released on May 29, 2026.
- Structured Streaming deduplication now treats NaN values with different bit patterns as duplicates when a double or float column is the deduplication key.
- Previously, NaN values with different internal representations were incorrectly treated as distinct entries and were not deduplicated.
- A bug fix preserves table-level permissions on Unity Catalog foreign catalog tables during metadata refresh.
- Before the fix, metadata refresh could remove permissions from foreign catalog tables such as Snowflake connection tables, causing INSUFFICIENT_PERMISSIONS query failures.

## Source
- **Origin:** rss_feed
- **URL:** <https://docs.databricks.com/aws/en/release-notes/runtime/18#databricks-runtime-18-may-29-2026>

## Related
[[concepts/databricks-runtime|databricks-runtime]] · [[concepts/structured-streaming|structured-streaming]] · [[concepts/unity-catalog|unity-catalog]] · [[concepts/deduplication|deduplication]] · [[concepts/snowflake|snowflake]] · [[concepts/streaming|streaming]] · [[concepts/metadata|metadata]] · [[companies/databricks|Databricks]] · [[companies/snowflake|Snowflake]] · [[episodes/2026-05-30|2026-05-30]]
