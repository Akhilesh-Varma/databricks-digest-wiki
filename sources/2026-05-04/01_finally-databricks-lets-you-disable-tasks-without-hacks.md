---
type: story
story_id: community_536463b40ec3
episode_date: 2026-05-04
rank: 1
source: databricks_community
url: "https://community.databricks.com/t5/community-articles/finally-databricks-lets-you-disable-tasks-without-hacks/td-p/156052"
title: "Finally! Databricks lets you disable tasks without hacks"
quality_score: 0.66
content_hash: "sha256:3b0a1395977b4ded6b3c2c86f8882b4e107eff3b40581cb2235e75322103bf1a"
concepts: [lakeflow-jobs, databricks-workflows, task-disabling, private-preview]
companies: [databricks, microsoft-azure]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-04 10:19:55"
tags: [story, source/databricks-community]
---

## Summary
Databricks has introduced the ability to disable individual tasks within Lakeflow Jobs without removing them from the workflow. Previously, users had to rely on workarounds such as custom flags or conditional logic to skip tasks, which cluttered code and increased maintenance burden. A disabled task is skipped at runtime but retains its configuration and run history, allowing it to be re-enabled without rebuilding. The feature is currently in private preview and must be manually enabled via the Previews settings toggle.

## Key claims
- Databricks now allows users to disable individual tasks in Lakeflow Jobs without deleting them.
- Previously, skipping a task required workarounds such as custom flags or if-else logic blocks.
- A disabled task is skipped at runtime while retaining its full configuration and run history.
- Disabled tasks can be re-enabled later without any rebuilding required.
- The task-disabling feature is currently in private preview and must be toggled on in Previews settings.

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/community-articles/finally-databricks-lets-you-disable-tasks-without-hacks/td-p/156052>

## Related
[[concepts/lakeflow-jobs|lakeflow-jobs]] · [[concepts/databricks-workflows|databricks-workflows]] · [[concepts/task-disabling|task-disabling]] · [[concepts/databricks-lakeflow|databricks-lakeflow]] · [[concepts/azure-databricks|azure-databricks]] · [[concepts/databricks|databricks]] · [[concepts/lakeflow|lakeflow]] · [[concepts/azure|azure]] · [[companies/databricks|Databricks]] · [[companies/microsoft-azure|Microsoft Azure]] · [[episodes/2026-05-04|2026-05-04]]
