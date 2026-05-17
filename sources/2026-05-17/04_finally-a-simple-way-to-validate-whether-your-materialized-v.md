---
type: story
story_id: community_b5cc02e492bb
episode_date: 2026-05-17
rank: 4
source: databricks_community
url: "https://community.databricks.com/t5/community-articles/finally-a-simple-way-to-validate-whether-your-materialized-view/td-p/156557"
title: "Finally! A simple way to validate whether your Materialized View can actually refresh incrementally"
quality_score: 0.62
content_hash: "sha256:9baa96fa68ab1ddf54f2facf5d848dd4d5fa64685cf77d63d1ad5ccac1a82be8"
concepts: [materialized-view, incremental-refresh, explain-create-materialized-view, auto-refresh-policy, event-log]
companies: [databricks]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-17 10:20:15.924000"
tags: [story, source/databricks-community]
---

## Summary
Databricks has introduced a way to validate whether a Materialized View is eligible for incremental refresh before running a pipeline, using the EXPLAIN CREATE MATERIALIZED VIEW command. Previously, users had to run the pipeline and query the event log to verify incremental refresh behavior. The command provides a clear explanation when incremental refresh is not possible, such as when non-deterministic functions like current_timestamp are used. Notably, eligibility for incremental refresh only guarantees incremental execution under the AUTO refresh policy if the optimizer deems it cheaper; users must use the incremental refresh policy to enforce it. Open questions remain about support for non-algebraic functions like median and how Databricks handles late-arriving data in this context.

## Key claims
- The EXPLAIN CREATE MATERIALIZED VIEW command can now be used to check incremental refresh eligibility without running a pipeline.
- Previously, verifying incremental refresh required running the pipeline and querying the event log.
- Using non-deterministic functions like current_timestamp prevents a Materialized View from being eligible for incremental refresh.
- When incremental refresh is not possible, the command returns a precise explanation of the reason.
- Under the AUTO refresh policy, the optimizer may still choose full recompute even if incremental refresh is eligible.
- Users must explicitly use the incremental refresh policy to enforce incremental execution.

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/community-articles/finally-a-simple-way-to-validate-whether-your-materialized-view/td-p/156557>

## Related
[[concepts/materialized-view|materialized-view]] · [[concepts/incremental-refresh|incremental-refresh]] · [[concepts/explain-create-materialized-view|explain-create-materialized-view]] · [[concepts/auto-refresh-policy|auto-refresh-policy]] · [[concepts/materialized-views|materialized-views]] · [[concepts/databricks|databricks]] · [[concepts/pipeline|pipeline]] · [[concepts/explain|explain]] · [[concepts/views|views]] · [[companies/databricks|Databricks]] · [[episodes/2026-05-17|2026-05-17]]
