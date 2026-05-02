---
type: story
story_id: rss_b269696218d7
episode_date: 2026-04-13
rank: 4
source: rss_feed
url: "https://docs.databricks.com/aws/en/release-notes/whats-coming#upcoming-behavioral-change-void-columns-included-in-delta-table-reads"
title: Upcoming behavioral change VOID columns included in Delta table reads
quality_score: 0.828
content_hash: "sha256:f0290fc8e08b1ee8afb7f33b21ee2c95878cb12e8fc62c075523299bcb45ef31"
concepts: [delta-lake, void-type, dataframe-reads, time-travel-queries]
companies: [databricks]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:22:30.268000"
tags: [story, source/rss-feed]
---

## Summary
In mid-June 2026, Delta Lake will change its behavior to fully support VOID columns in table reads. Previously, VOID columns were silently skipped during path-based DataFrame reads and time travel queries. After the change, these columns will be included in query output. This may cause queries that depend on column count or position, such as INSERT INTO ... SELECT, to fail or return incorrect results. Users are advised to review any queries reading from Delta Lake tables that contain VOID columns.

## Key claims
- Delta Lake will fully support VOID columns starting mid-June 2026.
- Prior to this change, VOID columns were silently skipped in path-based DataFrame reads and time travel queries.
- After the change, VOID columns will be included in query output.
- Queries depending on column count or position, such as INSERT INTO ... SELECT, may fail or produce incorrect results.
- Users should review queries that read from Delta Lake tables with VOID columns to ensure compatibility.

## Source
- **Origin:** rss_feed
- **URL:** <https://docs.databricks.com/aws/en/release-notes/whats-coming#upcoming-behavioral-change-void-columns-included-in-delta-table-reads>

## Related
[[concepts/delta-lake|delta-lake]] · [[concepts/void-type|void-type]] · [[concepts/dataframe-reads|dataframe-reads]] · [[concepts/time-travel-queries|time-travel-queries]] · [[concepts/time-travel|time-travel]] · [[concepts/dataframe|dataframe]] · [[concepts/delta|delta]] · [[concepts/spark|spark]] · [[companies/databricks|Databricks]] · [[episodes/2026-04-13|2026-04-13]]
