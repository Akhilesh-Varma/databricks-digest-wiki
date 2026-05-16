---
type: story
story_id: rss_5fc4d7f0cb82
episode_date: 2026-05-16
rank: 5
source: rss_feed
url: "https://medium.com/towards-data-engineering/what-happens-if-two-jobs-run-a-delta-merge-on-the-same-partition-concurrency-deep-dive-e151da6a5c20?source=rss------databricks-5"
title: "What Happens If Two Jobs Run a Delta MERGE on the Same Partition? Concurrency Deep Dive"
quality_score: 0.698
content_hash: "sha256:b2b470d9502013e8975c5ca42be06ba0d4605a4186ffd704505f4631b78056fb"
concepts: [delta-lake, merge, optimistic-concurrency-control, etl, transaction-log, transaction-isolation]
companies: [databricks]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-16 10:19:35.881000"
tags: [story, source/rss-feed]
---

## Summary
The article explores what happens when two concurrent ETL jobs perform MERGE operations on the same partition of a Delta Lake table. It dives into Delta Lake's concurrency control mechanisms to explain how conflicts are detected and resolved. The piece examines the optimistic concurrency model used by Delta Lake and the conditions under which one or both jobs may fail or succeed. It is aimed at data engineers who need to understand transaction isolation and conflict resolution in Delta Lake environments.

## Key claims
- Delta Lake uses optimistic concurrency control to manage simultaneous write operations.
- Two concurrent MERGE operations targeting the same Delta Lake partition can result in a transaction conflict.
- Delta Lake's transaction log is central to detecting and resolving write conflicts between concurrent jobs.
- When a conflict is detected, one of the concurrent MERGE jobs will fail and may need to be retried.
- Understanding Delta Lake's concurrency model is critical for designing reliable ETL pipelines with overlapping write patterns.

## Source
- **Origin:** rss_feed
- **URL:** <https://medium.com/towards-data-engineering/what-happens-if-two-jobs-run-a-delta-merge-on-the-same-partition-concurrency-deep-dive-e151da6a5c20?source=rss------databricks-5>

## Related
[[concepts/delta-lake|delta-lake]] · [[concepts/merge|merge]] · [[concepts/optimistic-concurrency-control|optimistic-concurrency-control]] · [[concepts/etl|etl]] · [[concepts/transaction-log|transaction-log]] · [[concepts/transaction-isolation|transaction-isolation]] · [[concepts/data-engineering|data-engineering]] · [[concepts/delta|delta]] · [[companies/databricks|Databricks]] · [[episodes/2026-05-16|2026-05-16]]
