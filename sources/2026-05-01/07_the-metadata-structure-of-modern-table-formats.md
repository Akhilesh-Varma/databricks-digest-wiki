---
type: story
story_id: devto_3592586
episode_date: 2026-05-01
rank: 7
source: devto
url: "https://dev.to/alexmercedcoder/the-metadata-structure-of-modern-table-formats-i81"
title: The Metadata Structure of Modern Table Formats
quality_score: 0.829
content_hash: "sha256:f47e23d59de870b37877b725e1b98b3e77ae2a1cdd8b58bf752db53917006bf1"
concepts: [apache-iceberg, metadata-tree, manifest-list, manifest-file, snapshot, partition-evolution, hidden-partitioning, lakehouse-catalog, rest-catalog, hive-metastore, acid-transactions, time-travel, avro, apache-spark, s3-tables]
companies: [dremio, amazon-web-services, minio, apache-software-foundation]
people: [alex-merced]
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-01 10:20:11.266000"
tags: [story, source/devto]
---

## Summary
This article is Part 2 of a 15-part Apache Iceberg Masterclass and focuses on how modern table formats organize their metadata. It explains that metadata structure determines query planning speed, concurrent write handling, schema change propagation, and overhead accumulation. The article provides a detailed breakdown of Apache Iceberg's four-level metadata tree: catalog pointer, metadata file, manifest list, and manifest files. Each level progressively narrows the search space, enabling efficient pruning at query planning time. The piece also situates Iceberg within the broader landscape of lakehouse table formats that support ACID transactions and time travel.

## Key claims
- Apache Iceberg organizes metadata into a four-level tree: catalog pointer, metadata file (JSON), manifest list (Avro), and manifest files (Avro).
- The catalog stores a pointer to the current metadata file, serving as the single source of truth for the table's current state.
- Each snapshot in the metadata file is immutable and represents a complete version of the table; updates append a new snapshot rather than overwriting.
- Manifest lists contain partition-level summary statistics that allow the query planner to skip entire manifests not matching a query filter.
- Manifest files store per-file statistics (min, max, null count, NaN count, distinct count) enabling file-level pruning during query planning.
- Two table formats can both claim ACID support and time travel while having fundamentally different metadata mechanisms under the hood.
- For a petabyte-scale table, Iceberg's metadata tree can reduce query planning overhead to as few as three sequential reads before identifying relevant data files.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/alexmercedcoder/the-metadata-structure-of-modern-table-formats-i81>

## Related
[[concepts/apache-iceberg|apache-iceberg]] · [[concepts/metadata-tree|metadata-tree]] · [[concepts/manifest-list|manifest-list]] · [[concepts/manifest-file|manifest-file]] · [[concepts/snapshot|snapshot]] · [[concepts/partition-evolution|partition-evolution]] · [[concepts/hidden-partitioning|hidden-partitioning]] · [[concepts/lakehouse-catalog|lakehouse-catalog]] · [[concepts/rest-catalog|rest-catalog]] · [[concepts/hive-metastore|hive-metastore]] · [[concepts/acid-transactions|acid-transactions]] · [[concepts/time-travel|time-travel]] · [[concepts/avro|avro]] · [[concepts/streaming-data|streaming-data]] · [[concepts/lakehouse|lakehouse]] · [[concepts/aws-glue|aws-glue]] · [[concepts/iceberg|iceberg]] · [[concepts/python|python]] · [[concepts/spark|spark]] · [[concepts/aws|aws]] · [[concepts/ai|ai]] · [[concepts/s3|s3]] · [[companies/dremio|Dremio]] · [[companies/amazon-web-services|Amazon Web Services]] · [[companies/minio|MinIO]] · [[companies/apache-software-foundation|Apache Software Foundation]] · [[people/alex-merced|Alex Merced]] · [[episodes/2026-05-01|2026-05-01]]
