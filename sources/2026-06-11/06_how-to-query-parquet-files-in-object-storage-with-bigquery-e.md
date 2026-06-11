---
type: story
story_id: devto_3872102
episode_date: 2026-06-11
rank: 6
source: devto
url: "https://dev.to/mirlan_de/how-to-query-parquet-files-in-object-storage-with-bigquery-external-tables-cfo"
title: How to Query Parquet Files in Object Storage with BigQuery External Tables
quality_score: 0.899
content_hash: "sha256:3c7128fd6ef9b8ce31415f66183ac93482bb242cbb5cbc8c0fd34d1f3caaf586"
concepts: [bigquery-external-tables, parquet, hive-partitioning, bigquery-omni-biglake, duckdb, trino, apache-spark, clickhouse, polars]
companies: [google, amazon-web-services]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-06-11 10:17:49.233000"
tags: [story, source/devto]
---

## Summary
This tutorial explains how to query Parquet files stored in object storage (GCS or Amazon S3) using BigQuery external tables, avoiding the need to copy data into BigQuery-managed storage. External tables allow BigQuery to read data directly from object storage at query time, reducing storage costs and enabling vendor portability. The article covers setting up a GCS bucket with Hive-style partitioning, writing Parquet files with Python, and creating BigQuery external tables. It also notes that the same Parquet files can be queried by other engines like DuckDB, Trino, Spark, ClickHouse, or Polars, making the approach engine-agnostic. The main tradeoff is slightly slower query performance compared to native BigQuery tables.

## Key claims
- BigQuery external tables allow querying Parquet files in object storage without copying data into BigQuery-managed storage.
- GCS standard storage costs $0.02/GB/month, the same as active BigQuery native storage, but long-term BigQuery storage drops to $0.01/GB/month.
- Hive-style partitioning (e.g., by date) in the object storage path is automatically recognized by BigQuery and can reduce query costs by 10-100x.
- Parquet files in object storage are queryable by multiple engines including BigQuery, DuckDB, Trino, Spark, ClickHouse, and Polars, enabling vendor portability.
- External tables are slightly slower than native BigQuery tables because data must be read from GCS rather than BigQuery's internal storage.
- BigQuery Omni BigLake enables external tables over Amazon S3 in addition to GCS.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/mirlan_de/how-to-query-parquet-files-in-object-storage-with-bigquery-external-tables-cfo>

## Related
[[concepts/bigquery-external-tables|bigquery-external-tables]] · [[concepts/parquet|parquet]] · [[concepts/hive-partitioning|hive-partitioning]] · [[concepts/bigquery-omni-biglake|bigquery-omni-biglake]] · [[concepts/s3-compatible-storage|s3-compatible-storage]] · [[concepts/data-engineering|data-engineering]] · [[concepts/object-storage|object-storage]] · [[concepts/partitioning|partitioning]] · [[concepts/analytics|analytics]] · [[concepts/amazon-s3|amazon-s3]] · [[concepts/bigquery|bigquery]] · [[concepts/biglake|biglake]] · [[concepts/schema|schema]] · [[concepts/python|python]] · [[concepts/spark|spark]] · [[concepts/gcs|gcs]] · [[concepts/s3|s3]] · [[companies/google|Google]] · [[companies/amazon-web-services|Amazon Web Services]] · [[episodes/2026-06-11|2026-06-11]]
