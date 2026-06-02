---
type: story
story_id: community_fa1f3cffde1e
episode_date: 2026-04-20
rank: 2
source: databricks_community
url: "https://community.databricks.com/t5/community-articles/lakeflow-spark-declarative-pipelines-now-decouples-pipeline-and/td-p/154287"
title: Lakeflow Spark Declarative Pipelines now decouples pipeline and tables lifecycle
quality_score: 0.78
content_hash: "sha256:f7a49f6ba9f3f3659768d05391a7c1fc0da27e32356886f82fc57c53476ea873"
concepts: [lakeflow-spark-declarative-pipelines, unity-catalog, materialized-views, streaming-tables, views]
companies: [databricks]
people: []
extractor_model: llama-3.3-70b-versatile
extracted_at: "2026-04-28 04:05:12.964000"
tags: [story, source/databricks-community]
---

## Summary
Databricks has introduced a beta feature for Lakeflow Spark Declarative Pipelines, allowing users to decouple pipelines from the tables they manage. This feature provides more flexibility for real-world scenarios, beyond strict CI/CD setups. With this update, deleting a pipeline no longer deletes its associated Materialized Views, Streaming Tables, and Views. The data remains fully queryable, and tables can be reattached to a pipeline anytime. This feature is available for Unity Catalog pipelines using the default publishing mode.

## Key claims
- Databricks has introduced a beta feature for Lakeflow Spark Declarative Pipelines to decouple pipelines from tables
- The feature allows deleting a pipeline without deleting its associated Materialized Views, Streaming Tables, and Views
- The data remains fully queryable even after a pipeline is deleted
- Tables can be reattached to a pipeline anytime and resume processing
- This feature is available for Unity Catalog pipelines using the default publishing mode

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/community-articles/lakeflow-spark-declarative-pipelines-now-decouples-pipeline-and/td-p/154287>

## Related
[[concepts/lakeflow-spark-declarative-pipelines|lakeflow-spark-declarative-pipelines]] · [[concepts/unity-catalog|unity-catalog]] · [[concepts/spark-declarative-pipelines|spark-declarative-pipelines]] · [[concepts/declarative-pipelines|declarative-pipelines]] · [[concepts/databricks|databricks]] · [[concepts/streaming|streaming]] · [[concepts/lakeflow|lakeflow]] · [[concepts/pipeline|pipeline]] · [[concepts/spark|spark]] · [[companies/databricks|Databricks]] · [[episodes/2026-04-20|2026-04-20]]
