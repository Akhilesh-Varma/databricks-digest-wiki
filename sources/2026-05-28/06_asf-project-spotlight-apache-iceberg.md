---
type: story
story_id: devto_3766846
episode_date: 2026-05-28
rank: 6
source: devto
url: "https://dev.to/theasf/asf-project-spotlight-apache-iceberg-fl5"
title: ASF Project Spotlight Apache Iceberg
quality_score: 0.833
content_hash: "sha256:e3e9c823e0016880d17292fbacd5080c152d8f2a1ad562715f28ceb7621f0074"
concepts: [apache-iceberg, lakehouse-architecture, open-table-format, apache-hive, apache-parquet, apache-hudi, apache-xtable, schema-evolution, data-lake]
companies: [netflix, apache-software-foundation, cloudera, dremio, onehouse, qlik, amazon]
people: [dipankar-mazumdar]
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-28 10:18:53.594000"
tags: [story, source/devto]
---

## Summary
Apache Iceberg is a high-performance open table format for large analytic datasets, originally developed at Netflix to address reliability and scalability challenges in data lakes. Before Iceberg, data lakes relied on Apache Hive and Parquet but suffered from unreliable updates, brittle partitioning, and expensive metadata handling, especially on cloud object stores. Iceberg introduced a table abstraction over raw data files, combining data warehouse consistency with data lake flexibility. The project was open sourced and contributed to the Apache Software Foundation, where community collaboration drove its widespread adoption. Dipankar Mazumdar, Director of Developer Relations at Cloudera, discusses Iceberg's origins, its impact on modern lakehouse architectures, and the role of open collaboration in its growth.

## Key claims
- Apache Iceberg was originally developed at Netflix to handle massive datasets reliably while supporting evolving data requirements.
- Before Iceberg, data lakes relied on Apache Hive and Apache Parquet but faced unreliable updates, brittle partitioning, and expensive metadata handling on cloud object stores like Amazon S3.
- Iceberg introduces a table abstraction on top of raw data files, enabling multiple engines to safely read and write to the same datasets with strong consistency guarantees.
- Iceberg was open sourced and contributed to the Apache Software Foundation after Netflix recognized the challenges it solved were industry-wide.
- Dipankar Mazumdar is the author of 'Engineering Lakehouses with Open Table Formats' and a contributor to 'Apache Iceberg: The Definitive Guide'.
- Data warehouses abstracted storage complexity behind proprietary systems, leading to significant cost issues and vendor lock-in for organizations.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/theasf/asf-project-spotlight-apache-iceberg-fl5>

## Related
[[concepts/apache-iceberg|apache-iceberg]] · [[concepts/lakehouse-architecture|lakehouse-architecture]] · [[concepts/open-table-format|open-table-format]] · [[concepts/apache-hive|apache-hive]] · [[concepts/apache-parquet|apache-parquet]] · [[concepts/schema-evolution|schema-evolution]] · [[concepts/data-lake|data-lake]] · [[concepts/open-table-formats|open-table-formats]] · [[concepts/data-engineering|data-engineering]] · [[concepts/data-warehouses|data-warehouses]] · [[concepts/table-format|table-format]] · [[concepts/partitioning|partitioning]] · [[concepts/open-source|open-source]] · [[concepts/data-lakes|data-lakes]] · [[concepts/amazon-s3|amazon-s3]] · [[concepts/lakehouse|lakehouse]] · [[concepts/parquet|parquet]] · [[concepts/iceberg|iceberg]] · [[concepts/schema|schema]] · [[concepts/dremio|dremio]] · [[concepts/hadoop|hadoop]] · [[concepts/ai|ai]] · [[concepts/s3|s3]] · [[companies/netflix|Netflix]] · [[companies/apache-software-foundation|Apache Software Foundation]] · [[companies/cloudera|Cloudera]] · [[companies/dremio|Dremio]] · [[companies/onehouse|Onehouse]] · [[companies/qlik|Qlik]] · [[companies/amazon|Amazon]] · [[people/dipankar-mazumdar|Dipankar Mazumdar]] · [[episodes/2026-05-28|2026-05-28]]
