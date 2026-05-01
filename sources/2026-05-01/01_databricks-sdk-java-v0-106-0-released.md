---
type: story
story_id: github_release_databricks_databricks-sdk-java_315827389
episode_date: 2026-05-01
rank: 1
source: github_releases
url: "https://github.com/databricks/databricks-sdk-java/releases/tag/v0.106.0"
title: Databricks SDK Java v0.106.0 released
quality_score: 0.808
content_hash: "sha256:1c790bfec96683a9522143eb8b98e054734dc10285193ae98c222cb9f35df56a"
concepts: [databricks-java-sdk, unity-catalog, delta-lake, databricks-pipelines, supervisor-agents, disaster-recovery, knowledge-assistants, confidential-compute]
companies: [databricks, confluent, atlassian, google, smartsheet, microsoft]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-01 10:18:50.959000"
tags: [story, source/github-releases]
---

## Summary
Databricks released version 0.106.0 of its Java SDK, introducing a range of API changes. The release adds a new `disasterrecovery` package and associated account-level service, as well as a `temporaryVolumeCredentials` workspace service. New methods were added to the `knowledgeAssistants` and `postgres` services, and several new fields were introduced across compute, ML, pipelines, and supervisor-agent service classes. A breaking change was also included, making the `description` field on `SupervisorAgent` no longer required.

## Key claims
- Databricks SDK Java v0.106.0 adds a new com.databricks.sdk.service.disasterrecovery package.
- The release introduces accountClient.disasterRecovery and workspaceClient.temporaryVolumeCredentials services.
- New CRUD and permission methods were added to the workspaceClient.knowledgeAssistants service.
- An undeleteProject method was added to the workspaceClient.postgres service.
- Confluence, Jira, Outlook, and Smartsheet options were added to pipelines.ConnectorOptions.
- A breaking change makes the description field on SupervisorAgent no longer required.
- A CONFLUENCE enum value was added to both ConnectionType and IngestionSourceType.

## Source
- **Origin:** github_releases
- **URL:** <https://github.com/databricks/databricks-sdk-java/releases/tag/v0.106.0>

## Related
[[concepts/databricks-java-sdk|databricks-java-sdk]] · [[concepts/databricks-pipelines|databricks-pipelines]] · [[concepts/supervisor-agents|supervisor-agents]] · [[concepts/disaster-recovery|disaster-recovery]] · [[concepts/knowledge-assistants|knowledge-assistants]] · [[concepts/databricks|databricks]] · [[concepts/postgres|postgres]] · [[concepts/sdk|sdk]] · [[concepts/api|api]] · [[companies/databricks|Databricks]] · [[companies/confluent|Confluent]] · [[companies/atlassian|Atlassian]] · [[companies/google|Google]] · [[companies/smartsheet|Smartsheet]] · [[companies/microsoft|Microsoft]] · [[episodes/2026-05-01|2026-05-01]]
