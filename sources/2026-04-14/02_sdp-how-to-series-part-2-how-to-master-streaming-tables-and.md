---
type: story
story_id: community_7664885c07a0
episode_date: 2026-04-14
rank: 2
source: databricks_community
url: "https://community.databricks.com/t5/technical-blog/sdp-how-to-series-part-2-how-to-master-streaming-tables-and/ba-p/151728"
title: SDP How-To Series. Part 2 How to Master Streaming Tables and Materialized Views
quality_score: 0.78
content_hash: "sha256:6f1bf62f6885613654c06b599b734aae1f6ad59e39fcda1ec0be5cebad94d811"
concepts: [lakeflow-spark-declarative-pipelines, streaming-tables, materialized-views, dp-temporary-view, dp-table, dp-materialized-view, append-flow, spark-structured-streaming, unity-catalog, medallion-architecture, apache-kafka]
companies: [databricks]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:18:07.874000"
tags: [story, source/databricks-community]
---

## Summary
This article is the second installment in the Lakeflow Spark Declarative Pipelines (SDP) How-To Series on Databricks Community. It explains the core building blocks of SDP pipelines: temporary views, streaming tables, and materialized views, and guides readers on when to use each. The concept of a 'flow' is introduced as a stateful, incremental computation that defines how data moves from source to destination. The article contrasts imperative Spark Structured Streaming code with the declarative SDP decorator-based approach, showing how the latter automates persistence, checkpoints, and state management. Practical examples using dp.temporary_view and dp.table decorators illustrate Bronze-layer ingestion patterns.

## Key claims
- In SDP, a 'flow' is a stateful, incremental computation that tracks processed data and defines both the query and the landing mode (Append, Upsert, or Replace).
- dp.temporary_view creates ephemeral, storage-free views scoped to the pipeline, useful for modular transformation logic without creating physical tables.
- dp.table is the primary target for an Append Flow and is the declarative equivalent of Spark Structured Streaming's writeStream API with outputMode append.
- SDP implicitly creates an Append Flow when the dp.table decorator is used, eliminating the need for explicit .save or writeStream calls.
- Flows can be defined implicitly via decorators or explicitly for more complex pipeline logic.
- Each flow's destination is either a physical table in Unity Catalog or a sink to an external system.
- Streaming Tables are recommended for Bronze-layer ingestion of sources like Kafka topics or raw JSON file directories.

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/technical-blog/sdp-how-to-series-part-2-how-to-master-streaming-tables-and/ba-p/151728>

## Related
[[concepts/lakeflow-spark-declarative-pipelines|lakeflow-spark-declarative-pipelines]] · [[concepts/streaming-tables|streaming-tables]] · [[concepts/materialized-views|materialized-views]] · [[concepts/dp-temporary-view|dp-temporary-view]] · [[concepts/dp-table|dp-table]] · [[concepts/dp-materialized-view|dp-materialized-view]] · [[concepts/append-flow|append-flow]] · [[concepts/spark-structured-streaming|spark-structured-streaming]] · [[concepts/unity-catalog|unity-catalog]] · [[concepts/spark-declarative-pipelines|spark-declarative-pipelines]] · [[concepts/declarative-pipelines|declarative-pipelines]] · [[concepts/structured-streaming|structured-streaming]] · [[concepts/dataframe|dataframe]] · [[concepts/lakeflow|lakeflow]] · [[concepts/pipeline|pipeline]] · [[concepts/upsert|upsert]] · [[concepts/views|views]] · [[concepts/kafka|kafka]] · [[concepts/spark|spark]] · [[concepts/api|api]] · [[concepts/uc|uc]] · [[companies/databricks|Databricks]] · [[episodes/2026-04-14|2026-04-14]]
