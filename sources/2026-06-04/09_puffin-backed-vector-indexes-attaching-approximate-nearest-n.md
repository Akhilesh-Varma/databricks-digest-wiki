---
type: story
story_id: rss_16812b36c1cd
episode_date: 2026-06-04
rank: 9
source: rss_feed
url: "https://arxiv.org/abs/2606.04196"
title: Puffin-Backed Vector Indexes Attaching Approximate Nearest Neighbor Indexes to Apache Iceberg Snapshots for Compute-Disaggregated Query Engines
quality_score: 0.836
content_hash: "sha256:8d9d365346b24ae21f55917d6592c959c54790b9636946642eae1ff47e291044"
concepts: [apache-iceberg, puffin-file-format, approximate-nearest-neighbor-index, vamana-graph, diskann, compute-disaggregated-architecture, vector-similarity-search, iceberg-rest-catalog, flockdb, duckdb, optimistic-concurrency-control, massively-parallel-processing-engine, deletion-vectors]
companies: []
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-06-04 10:23:14.778000"
tags: [story, source/rss-feed]
---

## Summary
This paper describes a design pattern and implementation for embedding distributed approximate nearest neighbor (ANN) indexes inside the Apache Iceberg table format. The authors use the Puffin sidecar file as a storage container and the snapshot summary as a binding mechanism, enabling vector similarity search within compute-disaggregated query engines without a dedicated index storage layer. The approach stores full Vamana/DiskANN graphs at billion-vector scale inside Puffin blobs, linking them through existing Iceberg snapshot operations to inherit atomicity, time travel, and multi-engine readability at no extra implementation cost. A tiered probe strategy places small centroid indexes on the coordinator and large DiskANN graphs on executor SSDs. The implementation is demonstrated through FlockDB, a distributed MPP engine built on DuckDB.

## Key claims
- The Puffin sidecar file format is sufficient to carry full Vamana graphs at billion-vector scale inside Apache Iceberg tables.
- Linking ANN index blobs through the Iceberg snapshot summary property reduces index management to standard Iceberg snapshot operations.
- The design inherits atomicity, time travel, multi-engine readability, and orphan file garbage collection from the Iceberg table format at zero implementation cost.
- A tiered probe strategy places small centroid indexes on the coordinator and large DiskANN graphs on executor SSDs.
- The pattern avoids breaking the compute-disaggregation invariant by eliminating the need for a dedicated index storage layer with its own lifecycle and consistency model.
- The implementation extends FlockDB, a distributed MPP engine built on DuckDB.
- The paper presents a coordinator-executor protocol for distributed index build, probe, and incremental refresh integrated into the Iceberg REST catalog's optimistic-concurrency commit path.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2606.04196>

## Related
[[concepts/apache-iceberg|apache-iceberg]] · [[concepts/puffin-file-format|puffin-file-format]] · [[concepts/approximate-nearest-neighbor-index|approximate-nearest-neighbor-index]] · [[concepts/vamana-graph|vamana-graph]] · [[concepts/diskann|diskann]] · [[concepts/compute-disaggregated-architecture|compute-disaggregated-architecture]] · [[concepts/vector-similarity-search|vector-similarity-search]] · [[concepts/iceberg-rest-catalog|iceberg-rest-catalog]] · [[concepts/flockdb|flockdb]] · [[concepts/duckdb|duckdb]] · [[concepts/optimistic-concurrency-control|optimistic-concurrency-control]] · [[concepts/massively-parallel-processing-engine|massively-parallel-processing-engine]] · [[concepts/disaggregated-architecture|disaggregated-architecture]] · [[concepts/incremental-refresh|incremental-refresh]] · [[concepts/object-storage|object-storage]] · [[concepts/table-format|table-format]] · [[concepts/iceberg-rest|iceberg-rest]] · [[concepts/rest-catalog|rest-catalog]] · [[concepts/time-travel|time-travel]] · [[concepts/snapshot|snapshot]] · [[concepts/iceberg|iceberg]] · [[concepts/rest|rest]] · [[episodes/2026-06-04|2026-06-04]]
