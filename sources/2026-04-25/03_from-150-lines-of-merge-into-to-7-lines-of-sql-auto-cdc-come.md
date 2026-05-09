---
type: story
story_id: community_2d6d1ffd6f7f
episode_date: 2026-04-25
rank: 3
source: databricks_community
url: "https://community.databricks.com/t5/technical-blog/from-150-lines-of-merge-into-to-7-lines-of-sql-auto-cdc-comes-to/ba-p/155355"
title: From 150 Lines of MERGE INTO to 7 Lines of SQL AUTO CDC Comes to Databricks SQL
quality_score: 0.7
content_hash: "sha256:2dfec27bd034418d69ea8e41737d27360d49155cf3365ef0e4048d0e2d940093"
concepts: [auto-cdc, merge-into, change-data-capture, scd-type-2, sql, data-warehouse, pipeline]
companies: [databricks]
people: []
extractor_model: gemini-2.5-flash-lite
extracted_at: "2026-04-27 13:06:37.193816"
tags: [story, source/databricks-community]
---

## Summary
Databricks SQL has introduced AUTO CDC, a new declarative SQL API designed to simplify the process of keeping dimension tables in data warehouses synchronized with operational data. Previously, engineers relied on complex MERGE INTO statements, often exceeding 150 lines of procedural SQL, to handle challenges like event ordering, deduplication, and delete propagation. AUTO CDC automates these tasks, reducing the required code to approximately 7 lines of SQL by allowing users to declare keys, ordering columns, and SCD types. This new feature aims to eliminate the technical debt and silent failures associated with manual CDC pipeline implementations.

## Key claims
- Keeping dimension tables synchronized with operational data is a critical but challenging pipeline pattern in data platforms.
- The MERGE INTO statement was not originally designed for Change Data Capture (CDC) and requires extensive procedural logic for reliable implementation.
- Manual CDC implementations using MERGE INTO often lead to silent failures due to issues like out-of-order records, incorrect delete handling, and complex SCD Type 2 logic.
- AUTO CDC is a new declarative SQL API in Databricks SQL that automates deduplication, ordering, delete handling, checkpointing, and history tracking for CDC pipelines.
- AUTO CDC reduces the complexity of implementing SCD Type 2 pipelines from approximately 150 lines of procedural SQL to about 7 lines.
- AUTO CDC is currently available in Beta within the Databricks SQL Query Editor and runs directly on SQL warehouses.

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/technical-blog/from-150-lines-of-merge-into-to-7-lines-of-sql-auto-cdc-comes-to/ba-p/155355>

## Related
[[concepts/auto-cdc|auto-cdc]] · [[concepts/merge-into|merge-into]] · [[concepts/change-data-capture|change-data-capture]] · [[concepts/scd-type-2|scd-type-2]] · [[concepts/window-functions|window-functions]] · [[concepts/technical-debt|technical-debt]] · [[concepts/databricks-sql|databricks-sql]] · [[concepts/sql-warehouse|sql-warehouse]] · [[concepts/deduplication|deduplication]] · [[concepts/data-platform|data-platform]] · [[concepts/databricks|databricks]] · [[concepts/merge|merge]] · [[concepts/api|api]] · [[companies/databricks|Databricks]] · [[episodes/2026-04-25|2026-04-25]]
