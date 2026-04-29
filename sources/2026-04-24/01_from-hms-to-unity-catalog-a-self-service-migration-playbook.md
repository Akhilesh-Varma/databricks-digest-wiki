---
type: story
story_id: community_9d4706ee347d
episode_date: 2026-04-24
rank: 1
source: databricks_community
url: "https://community.databricks.com/t5/technical-blog/from-hms-to-unity-catalog-a-self-service-migration-playbook/ba-p/155116"
title: From HMS to Unity Catalog A Self-Service Migration Playbook
quality_score: 0.78
content_hash: "sha256:8c77c752f5806bb79c61ef9fdbcb44252bc6ea11d76fc2fb28986b00718731ae"
concepts: [unity-catalog, hive-metastore, ucx, catalog-explorer, genie-code]
companies: [databricks]
people: []
extractor_model: llama-3.3-70b-versatile
extracted_at: "2026-04-28 03:34:28.736000"
tags: [story, source/databricks-community]
---

## Summary
Databricks' Unity Catalog is a centralized governance layer that addresses the limitations of Hive Metastore, providing fine-grained access control, data lineage, and centralized auditing. This guide provides a self-service migration playbook for data engineers and platform administrators to migrate from Hive Metastore to Unity Catalog. The migration process involves moving away from the legacy workspace-level Hive Metastore and adopting a centralized governance structure. Unity Catalog provides a unified governance layer across the entire Databricks estate, unlocking features such as centralized governance, data discovery, and fine-grained access control.

## Key claims
- Unity Catalog provides a centralized governance layer across all workspaces, addressing the limitations of Hive Metastore.
- Migrating to Unity Catalog involves moving away from the legacy workspace-level Hive Metastore and adopting a centralized governance structure.
- Unity Catalog unlocks features such as centralized governance, data discovery, fine-grained access control, and automatic lineage.
- Staying on Hive Metastore poses an active risk, including loss of visibility into who has access to what and increased compliance efforts.
- Databricks will provision all new workspaces as Unity Catalog-only starting September 30, 2026.

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/technical-blog/from-hms-to-unity-catalog-a-self-service-migration-playbook/ba-p/155116>

## Related
[[concepts/unity-catalog|unity-catalog]] · [[concepts/hive-metastore|hive-metastore]] · [[concepts/lakeflow-connect|lakeflow-connect]] · [[concepts/data-discovery|data-discovery]] · [[concepts/access-control|access-control]] · [[concepts/vector-search|vector-search]] · [[concepts/data-lineage|data-lineage]] · [[concepts/databricks|databricks]] · [[concepts/governance|governance]] · [[concepts/workspace|workspace]] · [[concepts/lakeflow|lakeflow]] · [[concepts/lakebase|lakebase]] · [[concepts/pipeline|pipeline]] · [[concepts/genie|genie]] · [[concepts/dbfs|dbfs]] · [[concepts/ai|ai]] · [[companies/databricks|Databricks]] · [[episodes/2026-04-24|2026-04-24]]
