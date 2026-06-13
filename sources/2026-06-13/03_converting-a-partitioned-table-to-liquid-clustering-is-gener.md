---
type: story
story_id: rss_768d878a5153
episode_date: 2026-06-13
rank: 3
source: rss_feed
url: "https://docs.databricks.com/aws/en/release-notes/product/2026/june#converting-a-partitioned-table-to-liquid-clustering-is-generally-available"
title: Converting a partitioned table to liquid clustering is generally available
quality_score: 0.766
content_hash: "sha256:b01335f7f043529ddc077f62c4574b75903902b6cdc0cafee1bd0189f9d88060"
concepts: [liquid-clustering, delta-lake, databricks-runtime, table-partitioning]
companies: [databricks]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-06-13 10:16:37.242000"
tags: [story, source/rss-feed]
---

## Summary
Databricks has made generally available the ability to convert existing partitioned Delta Lake tables to liquid clustering using the ALTER TABLE ... REPLACE PARTITIONED BY WITH CLUSTER BY syntax. The conversion process is designed to minimize downtime for both readers and writers during the migration. This feature supports both external and managed tables and requires Databricks Runtime 18.1 or higher.

## Key claims
- Converting a partitioned Delta Lake table to liquid clustering is now generally available.
- The conversion uses the ALTER TABLE ... REPLACE PARTITIONED BY WITH CLUSTER BY syntax.
- The conversion process minimizes reader and writer downtime.
- Both external and managed tables are supported for conversion.
- The feature requires Databricks Runtime 18.1 or above.

## Source
- **Origin:** rss_feed
- **URL:** <https://docs.databricks.com/aws/en/release-notes/product/2026/june#converting-a-partitioned-table-to-liquid-clustering-is-generally-available>

## Related
[[concepts/liquid-clustering|liquid-clustering]] · [[concepts/delta-lake|delta-lake]] · [[concepts/databricks-runtime|databricks-runtime]] · [[concepts/table-partitioning|table-partitioning]] · [[concepts/databricks-runtime-18|databricks-runtime-18]] · [[concepts/cluster-by|cluster-by]] · [[concepts/databricks|databricks]] · [[concepts/delta|delta]] · [[companies/databricks|Databricks]] · [[episodes/2026-06-13|2026-06-13]]
