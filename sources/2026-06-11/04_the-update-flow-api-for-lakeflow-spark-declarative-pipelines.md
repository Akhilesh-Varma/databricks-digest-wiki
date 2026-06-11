---
type: story
story_id: rss_a3c3f2c7a202
episode_date: 2026-06-11
rank: 4
source: rss_feed
url: "https://docs.databricks.com/aws/en/release-notes/product/2026/june#the-update_flow-api-for-lakeflow-spark-declarative-pipelines-is-generally-available"
title: The update_flow API for Lakeflow Spark Declarative Pipelines is generally available
quality_score: 0.806
content_hash: "sha256:fe692f389d57784d8e1f8b994e164bb979673f41b9c96b2e3a222ddba08393b1"
concepts: [lakeflow-spark-declarative-pipelines, update-flow, update-output-mode, stateful-aggregations, append-flows, watermark]
companies: [databricks]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-06-11 10:17:28.311000"
tags: [story, source/rss-feed]
---

## Summary
Databricks has announced the general availability of the update_flow API for Lakeflow Spark Declarative Pipelines. The dp.update_flow decorator allows users to add an update flow that writes to a sink in update output mode, emitting only the rows that change in each batch. A key differentiator from append flows is that update flows support stateful aggregations without requiring a watermark.

## Key claims
- The dp.update_flow decorator is now generally available in Lakeflow Spark Declarative Pipelines.
- Update flows write to a sink in update output mode, emitting only changed rows in each batch.
- Unlike append flows, update flows support stateful aggregations without requiring a watermark.

## Source
- **Origin:** rss_feed
- **URL:** <https://docs.databricks.com/aws/en/release-notes/product/2026/june#the-update_flow-api-for-lakeflow-spark-declarative-pipelines-is-generally-available>

## Related
[[concepts/lakeflow-spark-declarative-pipelines|lakeflow-spark-declarative-pipelines]] · [[concepts/update-flow|update-flow]] · [[concepts/update-output-mode|update-output-mode]] · [[concepts/stateful-aggregations|stateful-aggregations]] · [[concepts/append-flows|append-flows]] · [[concepts/spark-declarative-pipelines|spark-declarative-pipelines]] · [[concepts/declarative-pipelines|declarative-pipelines]] · [[concepts/lakeflow|lakeflow]] · [[concepts/spark|spark]] · [[companies/databricks|Databricks]] · [[episodes/2026-06-11|2026-06-11]]
