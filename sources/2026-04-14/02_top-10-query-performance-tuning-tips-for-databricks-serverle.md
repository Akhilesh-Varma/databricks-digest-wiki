---
type: story
story_id: community_0fd805d2f795
episode_date: 2026-04-14
rank: 2
source: databricks_community
url: "https://community.databricks.com/t5/technical-blog/top-10-query-performance-tuning-tips-for-databricks-serverless/ba-p/43218"
title: Top 10 query performance tuning tips for Databricks Serverless SQL
quality_score: 0.78
content_hash: "sha256:c1b2b2e7ebb9f9b4f0b8600d96f057fd3eece92b069ce3a33ddf301fd1caf457"
concepts: [databricks-serverless-sql, delta-lake, photon, lakehouse, explain, acid-guarantees, auto-scaling, common-table-expressions-cte, data-explorer]
companies: [databricks]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:18:32.569000"
tags: [story, source/databricks-community]
---

## Summary
The article presents ten query performance tuning tips for Databricks Serverless SQL (DBSQL), aimed at data analysts and SQL users. It categorizes optimizations into resource, storage, and query optimization areas. Key advice includes avoiding SELECT *, using LIMIT and WHERE clauses, choosing appropriate data types, leveraging caching, and using Photon-compatible functions. The article also recommends running maintenance commands like ANALYZE, OPTIMIZE, and VACUUM, and understanding query plans via EXPLAIN. These tips are intended to reduce cost and improve execution speed on the Lakehouse platform.

## Key claims
- Databricks Serverless SQL (DBSQL) provides instant and elastic compute with lower total cost of ownership compared to traditional cloud data warehouses.
- SELECT * on large tables is an I/O-intensive operation that can cause bottlenecks when many users profile tables simultaneously.
- Using the LIMIT clause restricts rows returned, reducing memory consumption and network data transfer.
- Leveraging Delta format improves query performance through columnar storage, advanced optimizations, and ACID guarantees.
- Running ANALYZE, OPTIMIZE, and VACUUM are recommended maintenance commands to improve query performance in DBSQL.
- Photon-compatible (Photonizable) functions should be preferred to take advantage of Databricks' vectorized query engine.
- Query optimization is the responsibility of SQL users, not just the engineering or platform team, and poorly written queries can negate the benefits of large compute resources.

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/technical-blog/top-10-query-performance-tuning-tips-for-databricks-serverless/ba-p/43218>

## Related
[[concepts/databricks-serverless-sql|databricks-serverless-sql]] · [[concepts/delta-lake|delta-lake]] · [[concepts/photon|photon]] · [[concepts/lakehouse|lakehouse]] · [[concepts/query-performance-tuning|query-performance-tuning]] · [[concepts/dbsql-serverless|dbsql-serverless]] · [[concepts/data-warehouses|data-warehouses]] · [[concepts/databricks-sql|databricks-sql]] · [[concepts/databricks|databricks]] · [[concepts/warehouse|warehouse]] · [[concepts/analytics|analytics]] · [[concepts/optimize|optimize]] · [[concepts/vacuum|vacuum]] · [[concepts/delta|delta]] · [[concepts/sql|sql]] · [[companies/databricks|Databricks]] · [[episodes/2026-04-14|2026-04-14]]
