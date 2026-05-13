---
type: story
story_id: devto_3658589
episode_date: 2026-05-13
rank: 9
source: devto
url: "https://dev.to/slotix/duckdb-postgres-and-parquet-when-one-sql-query-becomes-a-workflow-5d71"
title: "DuckDB, Postgres, and Parquet when one SQL query becomes a workflow"
quality_score: 0.852
content_hash: "sha256:e026419f772ec1015ce058a831be5de1c159513610464f2b9d8babcae0942ee0"
concepts: [duckdb, postgresql, parquet, s3-object-storage, etl, duckdb-postgresql-extension, schema-inspection]
companies: []
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-13 10:22:49.036000"
tags: [story, source/devto]
---

## Summary
The article explores how DuckDB has simplified cross-source SQL queries by allowing direct access to Postgres databases, Parquet files, and S3 object storage without traditional ETL staging steps. While DuckDB solves much of the query engine problem, the author argues that repeatable, trustworthy workflows still require managing saved connections, S3 paths, schema checks, exports, and reruns. The piece traces how a simple Python wrapper around a DuckDB query gradually accumulates responsibilities until it becomes an unplanned pipeline. The author highlights that schema inspection and confidence in re-running queries are the harder, unsolved parts of the workflow. Ultimately, the article frames DuckDB as a powerful query tool whose surrounding workflow infrastructure remains scattered and fragile.

## Key claims
- DuckDB can query Postgres, Parquet files, and S3 object storage using plain SQL without prior data exports.
- DuckDB's PostgreSQL extension enables direct cross-source joins between database tables and file-based data.
- The query engine problem is largely solved by DuckDB, but the surrounding workflow for repeatability is not.
- Python wrapper scripts around DuckDB queries tend to accumulate responsibilities until they become unplanned pipelines.
- Schema inspection—knowing which tables and columns exist—is a prerequisite for trusting cross-source queries.
- Traditional cross-source workflows required exports, staging tables, notebooks, and temporary scripts before DuckDB.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/slotix/duckdb-postgres-and-parquet-when-one-sql-query-becomes-a-workflow-5d71>

## Related
[[concepts/duckdb|duckdb]] · [[concepts/postgresql|postgresql]] · [[concepts/parquet|parquet]] · [[concepts/s3-object-storage|s3-object-storage]] · [[concepts/duckdb-postgresql-extension|duckdb-postgresql-extension]] · [[concepts/object-storage|object-storage]] · [[concepts/workflows|workflows]] · [[concepts/postgres|postgres]] · [[concepts/pipeline|pipeline]] · [[concepts/schema|schema]] · [[concepts/python|python]] · [[concepts/sql|sql]] · [[concepts/s3|s3]] · [[episodes/2026-05-13|2026-05-13]]
