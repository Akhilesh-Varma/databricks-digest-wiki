---
type: story
story_id: github_release_databricks_databricks-sdk-java_321748990
episode_date: 2026-05-13
rank: 1
source: github_releases
url: "https://github.com/databricks/databricks-sdk-java/releases/tag/v0.108.0"
title: Databricks SDK Java v0.108.0 released
quality_score: 0.779
content_hash: "sha256:d17a3fe942bc554dba68d905dbad4339fee1ca7bb8587dc3b769ab157d684d0d"
concepts: [databricks-sdk-java, feature-engineering, served-model-workload-type, gpu-xlarge]
companies: [databricks]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-13 10:21:05.391000"
tags: [story, source/github-releases]
---

## Summary
Databricks released version 0.108.0 of its Java SDK, introducing several API changes across multiple services. New fields such as catalogName, createdAt, createdBy, name, and schemaName were added to the Feature class in the ML service. A GPU_XLARGE enum value was added to both ServedModelInputWorkloadType and ServingModelWorkloadType in the serving service. Breaking changes include a new required argument order for the listFeatures method and the removal of the unspecifiedResourceName field from RequestedResource in the postgres service.

## Key claims
- Databricks SDK Java v0.108.0 adds catalogName, createdAt, createdBy, name, and schemaName fields to com.databricks.sdk.service.ml.Feature.
- The release introduces a breaking change by adding catalogName and schemaName fields to com.databricks.sdk.service.ml.ListFeaturesRequest.
- GPU_XLARGE enum value is added to both ServedModelInputWorkloadType and ServingModelWorkloadType in the serving service.
- The listFeatures method for workspaceClient.featureEngineering has a breaking change with a new required argument order.
- The unspecifiedResourceName field is removed from com.databricks.sdk.service.postgres.RequestedResource as a breaking change.

## Source
- **Origin:** github_releases
- **URL:** <https://github.com/databricks/databricks-sdk-java/releases/tag/v0.108.0>

## Related
[[concepts/databricks-sdk-java|databricks-sdk-java]] · [[concepts/feature-engineering|feature-engineering]] · [[concepts/served-model-workload-type|served-model-workload-type]] · [[concepts/databricks|databricks]] · [[concepts/postgres|postgres]] · [[concepts/sdk|sdk]] · [[concepts/api|api]] · [[companies/databricks|Databricks]] · [[episodes/2026-05-13|2026-05-13]]
