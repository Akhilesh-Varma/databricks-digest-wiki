---
type: story
story_id: devto_3727315
episode_date: 2026-05-23
rank: 7
source: devto
url: "https://dev.to/alexmercedcoder/hands-on-with-apache-iceberg-using-dremio-cloud-fa4"
title: Hands-On with Apache Iceberg Using Dremio Cloud
quality_score: 0.83
content_hash: "sha256:83ba7874aee0d7fc6155842ab0c683693af58cf33e77cf347a6f9e70ac967616"
concepts: [apache-iceberg, dremio-cloud, columnar-cloud-cache-c3, open-catalog, polaris-catalog, hidden-partitioning, partition-pruning, arrow-flight, semantic-layer, lakehouse, nvme-ssd, odbc, jdbc]
companies: [dremio, apache-software-foundation, tableau, microsoft, looker, apache-superset]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-23 10:19:47.408000"
tags: [story, source/devto]
---

## Summary
This article is Part 14 of a 15-part Apache Iceberg Masterclass and provides a practical walkthrough of working with Apache Iceberg on Dremio Cloud. It covers table creation with hidden partitioning, data ingestion from various sources, and optimization features. The article explains Dremio's Columnar Cloud Cache (C3), which stores frequently accessed Iceberg data on local NVMe SSDs to reduce query latency. It also describes how Dremio's semantic layer and federation capabilities enable governed analytics across BI tools and heterogeneous data sources. The piece highlights Dremio's Polaris-based Open Catalog for metadata management and access control.

## Key claims
- Dremio Cloud automatically creates a Polaris-based Open Catalog for Iceberg tables that handles metadata management, access control, and automatic optimization.
- Dremio's Columnar Cloud Cache (C3) stores frequently accessed Iceberg data on local NVMe SSDs, reducing query latency from hundreds of milliseconds to single-digit milliseconds.
- C3 operates transparently, automatically tracking access patterns and caching the most-queried data without manual configuration.
- Dremio can federate queries across PostgreSQL, MySQL, Oracle, MongoDB, S3 files, and other sources, enabling data migration into Iceberg tables with a single INSERT...SELECT statement.
- Dremio exposes Iceberg data through ODBC, JDBC, and Arrow Flight endpoints, allowing BI tools such as Tableau, Power BI, Looker, and Superset to query Iceberg tables as traditional databases.
- Dremio's semantic layer allows creation of governed SQL views that serve as the interface between raw data and consumers, with wikis and tags to aid discoverability and AI-powered analytics.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/alexmercedcoder/hands-on-with-apache-iceberg-using-dremio-cloud-fa4>

## Related
[[concepts/apache-iceberg|apache-iceberg]] · [[concepts/dremio-cloud|dremio-cloud]] · [[concepts/columnar-cloud-cache-c3|columnar-cloud-cache-c3]] · [[concepts/open-catalog|open-catalog]] · [[concepts/polaris-catalog|polaris-catalog]] · [[concepts/hidden-partitioning|hidden-partitioning]] · [[concepts/semantic-layer|semantic-layer]] · [[concepts/metadata-management|metadata-management]] · [[concepts/partition-evolution|partition-evolution]] · [[concepts/data-ingestion|data-ingestion]] · [[concepts/streaming-data|streaming-data]] · [[concepts/access-control|access-control]] · [[concepts/object-storage|object-storage]] · [[concepts/partitioning|partitioning]] · [[concepts/governance|governance]] · [[concepts/postgresql|postgresql]] · [[concepts/s3-tables|s3-tables]] · [[concepts/analytics|analytics]] · [[concepts/streaming|streaming]] · [[concepts/ai-agent|ai-agent]] · [[concepts/power-bi|power-bi]] · [[concepts/bi-tools|bi-tools]] · [[concepts/metadata|metadata]] · [[concepts/mongodb|mongodb]] · [[concepts/tableau|tableau]] · [[concepts/iceberg|iceberg]] · [[concepts/dremio|dremio]] · [[concepts/python|python]] · [[concepts/cloud|cloud]] · [[concepts/views|views]] · [[concepts/minio|minio]] · [[concepts/mysql|mysql]] · [[concepts/nvme|nvme]] · [[concepts/sql|sql]] · [[concepts/ai|ai]] · [[concepts/s3|s3]] · [[companies/dremio|Dremio]] · [[companies/apache-software-foundation|Apache Software Foundation]] · [[companies/tableau|Tableau]] · [[companies/microsoft|Microsoft]] · [[companies/looker|Looker]] · [[companies/apache-superset|Apache Superset]] · [[episodes/2026-05-23|2026-05-23]]
