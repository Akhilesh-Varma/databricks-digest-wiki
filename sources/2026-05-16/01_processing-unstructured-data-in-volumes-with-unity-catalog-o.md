---
type: story
story_id: community_f3a0c04a8123
episode_date: 2026-05-16
rank: 1
source: databricks_community
url: "https://community.databricks.com/t5/technical-blog/processing-unstructured-data-in-volumes-with-unity-catalog-open/ba-p/153360"
title: Processing Unstructured Data in Volumes with Unity Catalog Open APIs
quality_score: 0.78
content_hash: "sha256:1d882367ae05d4379998f98f74f344b5bea8561efb8a5116de1dba85ed84441e"
concepts: [unity-catalog, credential-vending, unity-catalog-volumes, unity-catalog-open-apis, files-api, rag-pipeline, daft, duckdb, ray, databricks-data-intelligence-platform]
companies: [databricks]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-16 10:18:31.585000"
tags: [story, source/databricks-community]
---

## Summary
Databricks has extended Unity Catalog's Open APIs to support credential vending for Volumes, enabling external tools and engines to securely access unstructured data without manual IAM management. The credential vending mechanism issues temporary, scoped cloud storage credentials based on existing Unity Catalog permissions, eliminating credential sprawl. Tools such as Daft, DuckDB, and Ray can now read directly from governed Unity Catalog Volumes without requiring native Databricks connectors. This brings unstructured data—images, videos, documents, sensor data—under the same unified governance model already applied to tables, models, and features. The capability is designed to support modern AI workloads including multimodal models, RAG pipelines, and IoT analytics.

## Key claims
- Unity Catalog now supports credential vending for Volumes, issuing temporary scoped cloud storage credentials to external engines based on UC permissions.
- External tools like Daft, DuckDB, and Ray can access Unity Catalog Volumes directly without native Databricks connector support.
- Credential vending eliminates the need to manually provision or maintain cloud IAM credentials outside of Unity Catalog.
- Unity Catalog Volumes bring unstructured data under the same governance model as tables, models, and features.
- The Files API remains available for Databricks-native tooling, while credential vending targets external engines that read directly from cloud storage.
- A Databricks admin defines privileges on a Volume for a principal, and Unity Catalog validates those permissions before issuing credentials.

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/technical-blog/processing-unstructured-data-in-volumes-with-unity-catalog-open/ba-p/153360>

## Related
[[concepts/unity-catalog|unity-catalog]] · [[concepts/credential-vending|credential-vending]] · [[concepts/unity-catalog-volumes|unity-catalog-volumes]] · [[concepts/unity-catalog-open-apis|unity-catalog-open-apis]] · [[concepts/files-api|files-api]] · [[concepts/daft|daft]] · [[concepts/duckdb|duckdb]] · [[concepts/ray|ray]] · [[concepts/databricks-unity-catalog|databricks-unity-catalog]] · [[concepts/distributed-computing|distributed-computing]] · [[concepts/unity-catalog-volume|unity-catalog-volume]] · [[concepts/lineage-tracking|lineage-tracking]] · [[concepts/open-sharing|open-sharing]] · [[concepts/open-source|open-source]] · [[concepts/governance|governance]] · [[concepts/databricks|databricks]] · [[concepts/open-apis|open-apis]] · [[concepts/analytics|analytics]] · [[concepts/lakehouse|lakehouse]] · [[concepts/api|api]] · [[concepts/iot|iot]] · [[concepts/rag|rag]] · [[concepts/ai|ai]] · [[concepts/uc|uc]] · [[companies/databricks|Databricks]] · [[episodes/2026-05-16|2026-05-16]]
