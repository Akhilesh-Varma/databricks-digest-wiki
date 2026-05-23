---
type: story
story_id: devto_3718194
episode_date: 2026-05-22
rank: 8
source: devto
url: "https://dev.to/alexmercedcoder/writing-to-an-apache-iceberg-table-how-commits-and-acid-actually-work-59da"
title: Writing to an Apache Iceberg Table How Commits and ACID Actually Work
quality_score: 0.888
content_hash: "sha256:fffa888668e57704013e4e3b5bed6a10ad1d9beb02086fee084b06d57c655038"
concepts: [apache-iceberg, acid-transactions, manifest-file, manifest-list, snapshot, atomic-commit, compare-and-swap, lakehouse-catalog, partition-evolution, hidden-partitioning, parquet, orc, avro, object-storage, table-format]
companies: [amazon-web-services, microsoft, google, dremio, minio]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-22 10:21:36.947000"
tags: [story, source/devto]
---

## Summary
This article is Part 6 of a 15-part Apache Iceberg Masterclass and explains in detail how write operations work in Apache Iceberg tables. It describes the six-step write process: writing data files, creating manifest entries, creating or updating manifest files, creating a manifest list, creating a new metadata file, and performing an atomic commit via a catalog pointer swap. The article emphasizes that ACID guarantees in Iceberg are achieved entirely through the metadata layer rather than relying on any transactional capabilities of the underlying object storage (S3, ADLS, GCS). Concurrent writers are handled through a compare-and-swap operation at the catalog level. The piece is aimed at developers seeking a deep technical understanding of Iceberg's commit and ACID mechanics.

## Key claims
- Every write operation (INSERT, DELETE, UPDATE, MERGE) in Apache Iceberg follows the same six-step sequence.
- Newly written data files are invisible to readers until they are referenced by committed metadata.
- ACID guarantees in Iceberg live entirely in the metadata layer, not in the object storage layer.
- Object storage systems like S3, ADLS, and GCS have no built-in transaction support, making Iceberg's metadata-driven approach necessary.
- The atomic commit step uses a compare-and-swap operation on the catalog pointer to swap old metadata for new metadata.
- Manifest files are written in Avro format and contain file paths, row counts, partition values, and column-level statistics.
- Unchanged manifests from previous snapshots are carried forward by reference rather than being copied.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/alexmercedcoder/writing-to-an-apache-iceberg-table-how-commits-and-acid-actually-work-59da>

## Related
[[concepts/apache-iceberg|apache-iceberg]] · [[concepts/acid-transactions|acid-transactions]] · [[concepts/manifest-file|manifest-file]] · [[concepts/manifest-list|manifest-list]] · [[concepts/snapshot|snapshot]] · [[concepts/atomic-commit|atomic-commit]] · [[concepts/compare-and-swap|compare-and-swap]] · [[concepts/lakehouse-catalog|lakehouse-catalog]] · [[concepts/partition-evolution|partition-evolution]] · [[concepts/hidden-partitioning|hidden-partitioning]] · [[concepts/parquet|parquet]] · [[concepts/avro|avro]] · [[concepts/object-storage|object-storage]] · [[concepts/table-format|table-format]] · [[concepts/acid-guarantees|acid-guarantees]] · [[concepts/streaming-data|streaming-data]] · [[concepts/dremio-cloud|dremio-cloud]] · [[concepts/orphan-files|orphan-files]] · [[concepts/partitioning|partitioning]] · [[concepts/s3-tables|s3-tables]] · [[concepts/lakehouse|lakehouse]] · [[concepts/iceberg|iceberg]] · [[concepts/schema|schema]] · [[concepts/dremio|dremio]] · [[concepts/python|python]] · [[concepts/merge|merge]] · [[concepts/ai|ai]] · [[concepts/s3|s3]] · [[companies/amazon-web-services|Amazon Web Services]] · [[companies/microsoft|Microsoft]] · [[companies/google|Google]] · [[companies/dremio|Dremio]] · [[companies/minio|MinIO]] · [[episodes/2026-05-22|2026-05-22]]
