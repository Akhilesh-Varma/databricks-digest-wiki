---
type: story
story_id: rss_615b79ee60f7
episode_date: 2026-06-12
rank: 5
source: rss_feed
url: "https://docs.databricks.com/aws/en/release-notes/product/2026/june#abac-grant-policies-for-models-beta"
title: ABAC GRANT policies for models Beta
quality_score: 0.806
content_hash: "sha256:de780438f9b3505099d5778951ed0a29efa707ccb24d8cfb5778c35641fc4198"
concepts: [abac-grant-policies, unity-catalog, attribute-based-access-control, mlflow]
companies: [databricks]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-06-12 10:17:28.874000"
tags: [story, source/rss-feed]
---

## Summary
Databricks has released ABAC GRANT policies in Beta, extending attribute-based access control to Unity Catalog. These policies dynamically grant privileges to securable objects whose governed tags match a defined condition, eliminating the need to grant privileges on each object individually. In the Beta release, GRANT policies can assign the EXECUTE privilege on models, attached at the catalog or schema level. Both customer-registered MLflow models and Databricks-hosted foundation models in system.ai are supported.

## Key claims
- ABAC GRANT policies are now in Beta on Databricks.
- GRANT policies extend attribute-based access control to dynamically grant Unity Catalog privileges based on governed tag conditions.
- Privileges are granted to securable objects whose tags match a condition, rather than being granted on each object individually.
- In Beta, GRANT policies can grant the EXECUTE privilege on models at the catalog or schema level.
- Both customer-registered MLflow models and Databricks-hosted foundation models in system.ai are supported.

## Source
- **Origin:** rss_feed
- **URL:** <https://docs.databricks.com/aws/en/release-notes/product/2026/june#abac-grant-policies-for-models-beta>

## Related
[[concepts/abac-grant-policies|abac-grant-policies]] · [[concepts/unity-catalog|unity-catalog]] · [[concepts/attribute-based-access-control|attribute-based-access-control]] · [[concepts/foundation-models|foundation-models]] · [[concepts/access-control|access-control]] · [[concepts/governed-tags|governed-tags]] · [[concepts/databricks|databricks]] · [[concepts/schema|schema]] · [[concepts/abac|abac]] · [[concepts/ai|ai]] · [[companies/databricks|Databricks]] · [[episodes/2026-06-12|2026-06-12]]
