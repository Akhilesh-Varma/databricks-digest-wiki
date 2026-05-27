---
type: story
story_id: rss_1a57d6d9dc66
episode_date: 2026-05-27
rank: 2
source: rss_feed
url: "https://docs.databricks.com/aws/en/sql/release-notes/2026#databricks-sql-version-202615-is-now-available-in-preview"
title: Databricks SQL version 2026.15 is now available in Preview
quality_score: 0.946
content_hash: "sha256:fa31f17ae83b0336fce974c27c496795fedea49961f1306360fad436b1de5d1d"
concepts: [databricks-sql, delta-lake, unity-catalog, schema-evolution, sql-udf, xpath, natural-join, left-outer-join-lateral, void-type, optimized-writes, create-or-replace-table-as-select, coordinate-reference-system, st-dwithin, st-makepoint, st-makeenvelope, describe-history, dynamic-partition-overwrite]
companies: [databricks, esri]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-27 10:18:19.646000"
tags: [story, source/rss-feed]
---

## Summary
Databricks SQL version 2026.15 is now available in the Preview channel, introducing a range of new features, behavioral fixes, and bug corrections. Key changes include NULL struct preservation in schema-evolution writes, VOID column support in Delta Lake tables, and SQL UDF dependency validation enforcement in Unity Catalog. Several bug fixes address incorrect behavior in LEFT OUTER JOIN LATERAL, NATURAL JOIN case sensitivity, and optimized writes for partitioned Unity Catalog tables created with CRTAS. New geospatial functions and improved spatial join support are also introduced in this release.

## Key claims
- Databricks SQL 2026.15 is available in the Preview channel.
- XPath evaluation no longer loads external DTDs, preventing failures caused by malformed or unreachable DTD URLs.
- NULL structs in INSERT, MERGE, and streaming writes with schema evolution are now correctly stored as NULL rather than as non-null structs with all-NULL fields.
- Delta Lake tables now support VOID columns in path-based DataFrame reads and time travel queries.
- Unity Catalog now enforces dependency validation for SQL UDFs to prevent access control bypass via the REST API.
- NATURAL JOIN now correctly applies case-insensitive column matching when spark.sql.caseSensitive is false.
- New geospatial functions st_makepoint and st_makeenvelope are introduced, and ST_DWithin is now supported as a spatial join condition.

## Source
- **Origin:** rss_feed
- **URL:** <https://docs.databricks.com/aws/en/sql/release-notes/2026#databricks-sql-version-202615-is-now-available-in-preview>

## Related
[[concepts/databricks-sql|databricks-sql]] · [[concepts/delta-lake|delta-lake]] · [[concepts/unity-catalog|unity-catalog]] · [[concepts/schema-evolution|schema-evolution]] · [[concepts/sql-udf|sql-udf]] · [[concepts/sql-user-defined-functions|sql-user-defined-functions]] · [[concepts/user-defined-functions|user-defined-functions]] · [[concepts/time-travel-queries|time-travel-queries]] · [[concepts/dataframe-reads|dataframe-reads]] · [[concepts/access-control|access-control]] · [[concepts/delta-tables|delta-tables]] · [[concepts/spatial-join|spatial-join]] · [[concepts/metric-views|metric-views]] · [[concepts/time-travel|time-travel]] · [[concepts/delta-table|delta-table]] · [[concepts/databricks|databricks]] · [[concepts/dataframe|dataframe]] · [[concepts/rest-api|rest-api]] · [[concepts/schema|schema]] · [[concepts/merge|merge]] · [[concepts/delta|delta]] · [[concepts/views|views]] · [[concepts/spark|spark]] · [[concepts/udfs|udfs]] · [[concepts/rest|rest]] · [[concepts/sql|sql]] · [[concepts/api|api]] · [[concepts/xml|xml]] · [[companies/databricks|Databricks]] · [[companies/esri|ESRI]] · [[episodes/2026-05-27|2026-05-27]]
