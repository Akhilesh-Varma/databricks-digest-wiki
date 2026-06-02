---
type: story
story_id: devto_3692577
episode_date: 2026-05-19
rank: 8
source: devto
url: "https://dev.to/engineersguide/bigquery-snowflake-redshift-databricks-fabric-where-each-one-silently-inflates-your-bill-1o86"
title: "BigQuery, Snowflake, Redshift, Databricks, Fabric where each one silently inflates your bill"
quality_score: 0.886
content_hash: "sha256:6d28405ec42d4822c201ce00eb8321c15dc36b2ed15d0dbf9be601ce2ba66b99"
concepts: [scan-tax, idle-tax, complexity-tax, scale-to-zero-architecture, managed-ducklake, duckdb, egress-fees, bigquery, snowflake, redshift, microsoft-fabric]
companies: [google, snowflake, amazon-web-services, databricks, microsoft, motherduck, teradata, oracle]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-19 10:21:31.405000"
tags: [story, source/devto]
---

## Summary
The article analyzes hidden pricing mechanics in major cloud data warehouses—BigQuery, Snowflake, Redshift, Databricks, and Microsoft Fabric—identifying three core 'taxes': the Scan Tax (per-terabyte query charges), the Idle Tax (minimum billing windows for inactive compute), and the Complexity Tax (opaque billing units). The author draws on personal experience, including a $50,000 BigQuery bill from a single exploratory query, to illustrate how these models punish growth, experimentation, and idle time. Storage costs are described as largely commoditized and predictable, while compute, concurrency, and architecture are where vendors extract margin. MotherDuck is presented as an alternative that claims to eliminate these taxes through 1-second billing minimums, true scale-to-zero, and flat compute pricing via its Managed DuckLake offering.

## Key claims
- A single exploratory BigQuery query on an unpartitioned table generated a $50,000 bill overnight.
- The Scan Tax charges users per terabyte scanned, punishing exploratory queries on large unpartitioned tables.
- The Idle Tax imposes minimum billing windows (e.g., 60-second minimums) even when compute is inactive.
- The Complexity Tax refers to opaque, vendor-specific billing units that are difficult for customers to predict or audit.
- Storage costs across major vendors are largely commoditized, hovering around $23/TB/month for Snowflake and $0.01/GB/month for BigQuery long-term storage.
- MotherDuck claims to address these hidden taxes with a 1-second billing minimum, scale-to-zero architecture, and flat compute pricing.
- Moving from on-premises data warehouses (Teradata, Oracle) to the cloud replaced upfront hardware costs with a new set of hidden operational taxes.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/engineersguide/bigquery-snowflake-redshift-databricks-fabric-where-each-one-silently-inflates-your-bill-1o86>

## Related
[[concepts/scan-tax|scan-tax]] · [[concepts/idle-tax|idle-tax]] · [[concepts/complexity-tax|complexity-tax]] · [[concepts/scale-to-zero-architecture|scale-to-zero-architecture]] · [[concepts/managed-ducklake|managed-ducklake]] · [[concepts/egress-fees|egress-fees]] · [[concepts/bigquery|bigquery]] · [[concepts/snowflake|snowflake]] · [[concepts/redshift|redshift]] · [[concepts/microsoft-fabric|microsoft-fabric]] · [[concepts/cloud-data-warehouse|cloud-data-warehouse]] · [[concepts/data-warehouses|data-warehouses]] · [[concepts/data-warehouse|data-warehouse]] · [[concepts/databricks|databricks]] · [[concepts/warehouses|warehouses]] · [[concepts/warehouse|warehouse]] · [[concepts/teradata|teradata]] · [[concepts/cloud|cloud]] · [[concepts/s3|s3]] · [[companies/google|Google]] · [[companies/snowflake|Snowflake]] · [[companies/amazon-web-services|Amazon Web Services]] · [[companies/databricks|Databricks]] · [[companies/microsoft|Microsoft]] · [[companies/motherduck|MotherDuck]] · [[companies/teradata|Teradata]] · [[companies/oracle|Oracle]] · [[episodes/2026-05-19|2026-05-19]]
