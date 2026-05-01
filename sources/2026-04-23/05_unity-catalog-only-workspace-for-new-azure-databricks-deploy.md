---
type: story
story_id: community_7877b070de33
episode_date: 2026-04-23
rank: 5
source: databricks_community
url: "https://community.databricks.com/t5/community-articles/unity-catalog-only-workspace-for-new-azure-databricks/td-p/154609"
title: Unity Catalog-only workspace for new Azure Databricks deployments
quality_score: 0.7
content_hash: "sha256:efd51eea838007e4dc6a365b8aaeceb21d2e17b0b239c7b1c5eb87858fa17fa6"
concepts: [unity-catalog, dbfs, hive-metastore, mlflow]
companies: [databricks, microsoft-azure]
people: []
extractor_model: llama-3.3-70b-versatile
extracted_at: "2026-04-28 04:00:59.315000"
tags: [story, source/databricks-community]
---

## Summary
Starting September 30, 2026, all new Azure Databricks workspaces will be Unity Catalog only, eliminating DBFS root, Hive Metastore, and legacy runtimes below 13.3 LTS. This change aims to streamline the workspace experience. Existing features like volumes and system paths will continue to work as expected. The shift is part of a broader effort to modernize Azure Databricks deployments. Users will need to adapt to the new Unity Catalog-only environment.

## Key claims
- All new Azure Databricks workspaces will be Unity Catalog only starting September 30, 2026.
- DBFS root, Hive Metastore, and legacy runtimes below 13.3 LTS will be eliminated in new workspaces.
- Volumes will remain accessible via the dbfs Volumes prefix and POSIX-style Volumes path.
- System paths, including Databricks system paths and MLflow resource paths, will continue to work as expected.
- Internal workspace system data, such as notebook revisions and Spark logs, will still be accessible.

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/community-articles/unity-catalog-only-workspace-for-new-azure-databricks/td-p/154609>

## Related
[[concepts/unity-catalog|unity-catalog]] · [[concepts/dbfs|dbfs]] · [[concepts/hive-metastore|hive-metastore]] · [[concepts/databricks|databricks]] · [[concepts/workspace|workspace]] · [[concepts/azure|azure]] · [[concepts/spark|spark]] · [[companies/databricks|Databricks]] · [[companies/microsoft-azure|Microsoft Azure]] · [[episodes/2026-04-23|2026-04-23]]
