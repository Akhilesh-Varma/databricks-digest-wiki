---
type: story
story_id: github_release_databricks_databricks-sdk-java_324876054
episode_date: 2026-05-19
rank: 1
source: github_releases
url: "https://github.com/databricks/databricks-sdk-java/releases/tag/v0.110.0"
title: Databricks SDK Java v0.110.0 released
quality_score: 0.64
content_hash: "sha256:259633240ea81fcaa81c4ae2a80203d1fd4a67826621b1a363a9c7da054a5894"
concepts: [databricks-sdk-java, pipelineparams, pipelinetask]
companies: [databricks]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-19 10:19:48.446000"
tags: [story, source/github-releases]
---

## Summary
Databricks released version 0.110.0 of its Java SDK. The release introduces new fields for pipeline-related job parameters and tasks, including fullRefreshSelection, refreshFlowSelection, refreshSelection, and resetCheckpointSelection for both PipelineParams and PipelineTask classes. Additionally, two new email-related fields were added to the settings service.

## Key claims
- Databricks SDK Java v0.110.0 adds fullRefreshSelection, refreshFlowSelection, refreshSelection, and resetCheckpointSelection fields to com.databricks.sdk.service.jobs.PipelineParams.
- The same four new fields are also added to com.databricks.sdk.service.jobs.PipelineTask.
- Two new fields, effectiveOperationalEmailCustomRecipient and operationalEmailCustomRecipient, are added to com.databricks.sdk.service.settingsv2.Setting.

## Source
- **Origin:** github_releases
- **URL:** <https://github.com/databricks/databricks-sdk-java/releases/tag/v0.110.0>

## Related
[[concepts/databricks-sdk-java|databricks-sdk-java]] · [[concepts/pipelineparams|pipelineparams]] · [[concepts/pipelinetask|pipelinetask]] · [[concepts/databricks|databricks]] · [[concepts/sdk|sdk]] · [[concepts/api|api]] · [[companies/databricks|Databricks]] · [[episodes/2026-05-19|2026-05-19]]
