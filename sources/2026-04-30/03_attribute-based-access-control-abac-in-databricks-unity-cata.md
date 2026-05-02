---
type: story
story_id: community_4f6e7cb22e62
episode_date: 2026-04-30
rank: 3
source: databricks_community
url: "https://community.databricks.com/t5/community-articles/attribute-based-access-control-abac-in-databricks-unity-catalog/td-p/126465"
title: Attribute-Based Access Control ABAC in Databricks Unity Catalog
quality_score: 0.74
content_hash: "sha256:6898721ed06e3fe087e74f00fb7f5ffc00ee0716512c3ddac60372a5787a5b53"
concepts: [attribute-based-access-control, abac, databricks-unity-catalog, uc, row-level-security, rls, column-level-filtering, column-level-masking, clm, sql-user-defined-functions, udfs, rbac, pii]
companies: [databricks]
people: []
extractor_model: gemini-2.5-flash-lite
extracted_at: "2026-04-30 10:17:20.219000"
tags: [story, source/databricks-community]
---

## Summary
Databricks Unity Catalog now offers Attribute-Based Access Control (ABAC), a new data governance model that complements its existing security features. ABAC provides fine-grained, dynamic, and scalable access control for data, AI assets, and files by using attributes of users, data, and the environment, rather than just static roles. This allows for policies that adapt automatically to changing contexts and simplifies management through attribute-based rules and inheritance. ABAC supports features like row-level security and column-level masking, enhancing compliance and scalability for enterprise data management.

## Key claims
- Attribute-Based Access Control (ABAC) is a new data governance model available in Databricks Unity Catalog.
- ABAC offers fine-grained, dynamic, and scalable access control for data, AI assets, and files.
- Access in ABAC is governed by attributes of users, data, and the environment, not just static roles.
- ABAC policies can adapt automatically as attributes or business contexts change.
- Tags are key-value metadata pairs that are central to ABAC enforcement in Databricks.
- ABAC supports Row-Level Security (RLS) and Column-Level Masking (CLM) policies.
- Policies and tags in ABAC can inherit downward through the object hierarchy (catalog, schema, table).

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/community-articles/attribute-based-access-control-abac-in-databricks-unity-catalog/td-p/126465>

## Related
[[concepts/attribute-based-access-control|attribute-based-access-control]] · [[concepts/abac|abac]] · [[concepts/databricks-unity-catalog|databricks-unity-catalog]] · [[concepts/uc|uc]] · [[concepts/row-level-security|row-level-security]] · [[concepts/rls|rls]] · [[concepts/column-level-filtering|column-level-filtering]] · [[concepts/column-level-masking|column-level-masking]] · [[concepts/clm|clm]] · [[concepts/user-defined-functions|user-defined-functions]] · [[concepts/data-governance|data-governance]] · [[concepts/access-control|access-control]] · [[concepts/column-masking|column-masking]] · [[concepts/unity-catalog|unity-catalog]] · [[concepts/databricks|databricks]] · [[concepts/governance|governance]] · [[concepts/azure|azure]] · [[concepts/aws|aws]] · [[concepts/sql|sql]] · [[concepts/ai|ai]] · [[companies/databricks|Databricks]] · [[episodes/2026-04-30|2026-04-30]]
