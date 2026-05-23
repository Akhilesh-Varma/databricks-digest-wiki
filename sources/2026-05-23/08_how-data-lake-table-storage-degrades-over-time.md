---
type: story
story_id: devto_3726607
episode_date: 2026-05-23
rank: 8
source: devto
url: "https://dev.to/alexmercedcoder/how-data-lake-table-storage-degrades-over-time-47i5"
title: How Data Lake Table Storage Degrades Over Time
quality_score: 0.789
content_hash: "sha256:854df8537c07fa2e7a7473870e5e080d3faaa39d2a92bef99bbefad78f94e680"
concepts: [apache-iceberg, small-file-problem, orphan-files, metadata-bloat, iceberg-snapshots, iceberg-manifest, compaction, partition-evolution, hidden-partitioning, lakehouse-catalog, s3-tables, minio-ai-storage, dremio-cloud]
companies: [dremio, minio, amazon-web-services]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-23 10:20:04.366000"
tags: [story, source/devto]
---

## Summary
This article is Part 9 of a 15-part Apache Iceberg Masterclass and explains how Iceberg table storage degrades over time without proper maintenance. It identifies five types of degradation: the small file problem, orphan files, and metadata bloat (among others). The small file problem arises from frequent small commits, causing thousands of manifest entries that slow query planning. Orphan files accumulate from failed writes, expired snapshots, and compaction, wasting storage and increasing costs. Metadata bloat occurs as every commit adds a new snapshot, causing the metadata file to grow unboundedly.

## Key claims
- An Iceberg table that performs well on day one will degrade significantly by day 365 without periodic maintenance.
- Files smaller than 32 MB are considered problematic; a table with 10,000 small files requires the query planner to evaluate 10,000 manifest entries versus 40 for properly-sized 256 MB files.
- A streaming pipeline committing every 30 seconds can produce approximately 5,000 files per day.
- Orphan files accumulate from failed writes, expired snapshots, and compaction operations, and can cost thousands of dollars annually in storage fees.
- A daily batch pipeline writing 50 GB per day with weekly compaction can produce 350 GB of orphan files every week.
- Every commit creates a new snapshot, causing metadata files to grow over time and contributing to metadata bloat.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/alexmercedcoder/how-data-lake-table-storage-degrades-over-time-47i5>

## Related
[[concepts/apache-iceberg|apache-iceberg]] · [[concepts/small-file-problem|small-file-problem]] · [[concepts/orphan-files|orphan-files]] · [[concepts/metadata-bloat|metadata-bloat]] · [[concepts/iceberg-snapshots|iceberg-snapshots]] · [[concepts/iceberg-manifest|iceberg-manifest]] · [[concepts/compaction|compaction]] · [[concepts/streaming-pipeline|streaming-pipeline]] · [[concepts/streaming-data|streaming-data]] · [[concepts/batch-pipeline|batch-pipeline]] · [[concepts/partitioning|partitioning]] · [[concepts/lakehouse|lakehouse]] · [[concepts/snapshot|snapshot]] · [[concepts/pipeline|pipeline]] · [[concepts/iceberg|iceberg]] · [[concepts/dremio|dremio]] · [[concepts/python|python]] · [[concepts/ai|ai]] · [[concepts/s3|s3]] · [[companies/dremio|Dremio]] · [[companies/minio|MinIO]] · [[companies/amazon-web-services|Amazon Web Services]] · [[episodes/2026-05-23|2026-05-23]]
