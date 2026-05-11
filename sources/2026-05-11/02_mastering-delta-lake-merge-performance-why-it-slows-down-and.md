---
type: story
story_id: community_5c2c0914fe5d
episode_date: 2026-05-11
rank: 2
source: databricks_community
url: "https://community.databricks.com/t5/technical-blog/mastering-delta-lake-merge-performance-why-it-slows-down-and-how/ba-p/156305"
title: Mastering Delta Lake MERGE Performance Why It Slows Down and How to Fix It
quality_score: 0.62
content_hash: "sha256:bdfcf4e21298482d5c1bfa370fbd86fb0c858021b243980e2e203a2814e5564d"
concepts: [delta-lake-merge, delta-lake, literal-value-injection, copy-on-write, deletion-vectors, broadcasthashjoin, sortmergejoin, shuffledhashjoin, delta-transaction-log, cluster-by, predicate-pushdown]
companies: [databricks, apache-software-foundation]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-11 10:19:24.714000"
tags: [story, source/databricks-community]
---

## Summary
Delta Lake MERGE operations can degrade from seconds to minutes or hours as tables grow because, by default, Phase 2 of MERGE execution scans all files rather than pruning based on the source DataFrame's values. The root cause is that at query-planning time Spark cannot evaluate the source DataFrame, so join conditions referencing source columns cannot be pushed down as predicates. The solution is to pre-scan the source data, extract concrete literal values, and inject them into the MERGE condition so Spark can perform file pruning at plan time. This technique applies to both streaming and batch workloads and is especially impactful on large, clustered or partitioned tables. Additional optimizations such as Deletion Vectors can further reduce write amplification caused by Copy-on-Write file rewrites.

## Key claims
- By default, Delta Lake MERGE scans all files in the target table during Phase 2, regardless of clustering or partitioning keys.
- Spark cannot push down join conditions referencing an unevaluated source DataFrame as predicates at query-planning time.
- Pre-scanning the source batch to extract literal values and injecting them into the MERGE condition enables file pruning that is otherwise impossible.
- Delta Lake MERGE executes in five phases: transaction log analysis, file selection, join execution, Copy-on-Write file rewrite, and transaction commit.
- Copy-on-Write means every affected file is fully rewritten even if only one row is updated, causing write amplification.
- Deletion Vectors allow Delta Lake to mark rows as deleted without full file rewrites, reducing write amplification.
- The literal value injection optimization benefits both streaming micro-batch and batch MERGE workloads.

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/technical-blog/mastering-delta-lake-merge-performance-why-it-slows-down-and-how/ba-p/156305>

## Related
[[concepts/delta-lake-merge|delta-lake-merge]] · [[concepts/delta-lake|delta-lake]] · [[concepts/literal-value-injection|literal-value-injection]] · [[concepts/copy-on-write|copy-on-write]] · [[concepts/deletion-vectors|deletion-vectors]] · [[concepts/delta-transaction-log|delta-transaction-log]] · [[concepts/cluster-by|cluster-by]] · [[concepts/predicate-pushdown|predicate-pushdown]] · [[concepts/transaction-log|transaction-log]] · [[concepts/dataframe|dataframe]] · [[concepts/merge|merge]] · [[concepts/delta|delta]] · [[concepts/spark|spark]] · [[companies/databricks|Databricks]] · [[companies/apache-software-foundation|Apache Software Foundation]] · [[episodes/2026-05-11|2026-05-11]]
