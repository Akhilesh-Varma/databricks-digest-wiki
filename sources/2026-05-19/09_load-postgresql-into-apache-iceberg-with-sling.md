---
type: story
story_id: devto_3693742
episode_date: 2026-05-19
rank: 9
source: devto
url: "https://dev.to/flarco/load-postgresql-into-apache-iceberg-with-sling-1cm8"
title: Load PostgreSQL into Apache Iceberg with Sling
quality_score: 0.828
content_hash: "sha256:b8bcec2101a4afb42407171fa77d27b2e7f2cca21dd4fa3669a3770b48d88822"
concepts: [apache-iceberg, sling-cli, iceberg-rest-catalog, postgresql, parquet, aws-glue, nessie, lakekeeper, duckdb, apache-spark, trino, etl, schema-evolution, time-travel]
companies: [cloudflare, snowflake, amazon-web-services]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-19 10:21:47.574000"
tags: [story, source/devto]
---

## Summary
This article is a practical guide to replicating PostgreSQL data into Apache Iceberg tables using the Sling CLI tool. Sling connects directly to an Iceberg REST catalog without requiring a JVM, Spark, or manual manifest writing. The guide uses Cloudflare R2's managed Iceberg REST catalog and R2 object storage as the target. It walks through installing Sling, configuring a PostgreSQL source connection, configuring an Iceberg target connection, and running a full-refresh replication of three tables totaling 103,000 rows in 29 seconds. The article also notes that Sling supports other catalog types including AWS Glue and self-hosted options like Lakekeeper and Nessie.

## Key claims
- Sling can replicate PostgreSQL tables into Apache Iceberg using a REST catalog without requiring a JVM or Spark.
- The guide uses Cloudflare R2's managed Iceberg REST catalog and R2 object storage as the target layer.
- Sling supports REST, AWS Glue, and SQL catalog types for Iceberg targets.
- A full-refresh replication of 103,000 rows across three tables completed in 29 seconds end-to-end.
- Sling automatically creates the Iceberg namespace if it does not already exist in the catalog.
- Iceberg tables written by Sling can be read by DuckDB, Spark, Trino, Snowflake, and Athena without requiring a single shared warehouse vendor.
- Self-hosted catalogs such as Lakekeeper and Nessie are also supported with the same connection shape.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/flarco/load-postgresql-into-apache-iceberg-with-sling-1cm8>

## Related
[[concepts/apache-iceberg|apache-iceberg]] · [[concepts/sling-cli|sling-cli]] · [[concepts/iceberg-rest-catalog|iceberg-rest-catalog]] · [[concepts/postgresql|postgresql]] · [[concepts/parquet|parquet]] · [[concepts/aws-glue|aws-glue]] · [[concepts/nessie|nessie]] · [[concepts/lakekeeper|lakekeeper]] · [[concepts/etl|etl]] · [[concepts/hidden-partitioning|hidden-partitioning]] · [[concepts/object-storage|object-storage]] · [[concepts/table-format|table-format]] · [[concepts/iceberg-rest|iceberg-rest]] · [[concepts/rest-catalog|rest-catalog]] · [[concepts/partitioning|partitioning]] · [[concepts/append-flow|append-flow]] · [[concepts/warehouse|warehouse]] · [[concepts/snowflake|snowflake]] · [[concepts/analytics|analytics]] · [[concepts/postgres|postgres]] · [[concepts/iceberg|iceberg]] · [[concepts/schema|schema]] · [[concepts/spark|spark]] · [[concepts/rest|rest]] · [[concepts/sql|sql]] · [[concepts/cli|cli]] · [[concepts/api|api]] · [[concepts/aws|aws]] · [[concepts/s3|s3]] · [[companies/cloudflare|Cloudflare]] · [[companies/snowflake|Snowflake]] · [[companies/amazon-web-services|Amazon Web Services]] · [[episodes/2026-05-19|2026-05-19]]
