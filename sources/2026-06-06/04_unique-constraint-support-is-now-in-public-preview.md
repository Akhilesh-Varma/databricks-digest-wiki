---
type: story
story_id: rss_276b02328bcc
episode_date: 2026-06-06
rank: 4
source: rss_feed
url: "https://docs.databricks.com/aws/en/sql/release-notes/2026#unique-constraint-support-is-now-in-public-preview"
title: UNIQUE constraint support is now in Public Preview
quality_score: 0.786
content_hash: "sha256:2251a33e8d7eb1a81632428f0f8ac37610a2e5040ce80868688b7e1e554d7796"
concepts: [unity-catalog, delta-lake, databricks-sql, unique-constraint, photon, join-elimination, distinct-simplification, foreign-key]
companies: [databricks]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-06-06 10:18:49.045000"
tags: [story, source/rss-feed]
---

## Summary
Databricks SQL has introduced informational UNIQUE constraints on Unity Catalog Delta Lake tables, now available in Public Preview. Foreign keys can reference columns marked with UNIQUE constraints. When the RELY option is applied to a UNIQUE constraint on Photon-enabled compute, the query optimizer can perform join elimination and DISTINCT simplification. This feature is documented under the CONSTRAINT clause reference.

## Key claims
- Databricks SQL now supports informational UNIQUE constraints on Unity Catalog Delta Lake tables.
- Foreign keys can reference columns that have a UNIQUE constraint applied.
- Using RELY on a UNIQUE constraint enables join elimination on Photon-enabled compute.
- Using RELY on a UNIQUE constraint enables DISTINCT simplification on Photon-enabled compute.
- The UNIQUE constraint feature is currently in Public Preview.

## Source
- **Origin:** rss_feed
- **URL:** <https://docs.databricks.com/aws/en/sql/release-notes/2026#unique-constraint-support-is-now-in-public-preview>

## Related
[[concepts/unity-catalog|unity-catalog]] · [[concepts/delta-lake|delta-lake]] · [[concepts/databricks-sql|databricks-sql]] · [[concepts/unique-constraint|unique-constraint]] · [[concepts/photon|photon]] · [[concepts/join-elimination|join-elimination]] · [[concepts/distinct-simplification|distinct-simplification]] · [[concepts/foreign-key|foreign-key]] · [[concepts/databricks|databricks]] · [[concepts/delta|delta]] · [[concepts/sql|sql]] · [[companies/databricks|Databricks]] · [[episodes/2026-06-06|2026-06-06]]
