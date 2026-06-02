---
type: story
story_id: community_962b0f6120f4
episode_date: 2026-04-24
rank: 2
source: databricks_community
url: "https://community.databricks.com/t5/announcements/take-control-customer-managed-keys-for-lakebase-postgres/td-p/155338"
title: Take Control Customer-Managed Keys for Lakebase Postgres
quality_score: 0.74
content_hash: "sha256:0169b5b8663b67ae494e5294c0b797e6d1cf692bb1fa5dd692691caeea83c515"
concepts: [lakebase-postgres, customer-managed-keys, envelope-encryption]
companies: [databricks]
people: []
extractor_model: llama-3.3-70b-versatile
extracted_at: "2026-04-28 03:37:13.966000"
tags: [story, source/databricks-community]
---

## Summary
Databricks' Lakebase Postgres now supports customer-managed keys, allowing security teams to keep encryption keys in their own cloud KMS. This feature provides end-to-end protection, a cryptographic kill switch, and envelope encryption at scale. The customer-managed keys can be used to meet stricter data sovereignty and compliance requirements for Postgres workloads. The feature combines Lakebase's decoupled storage and compute architecture with customer-owned keys. Account admins can register the CMK once and bind it to a workspace, and all Lakebase projects in that workspace will inherit it.

## Key claims
- Lakebase Postgres now supports customer-managed keys (CMK) for encryption
- Customer-managed keys can be stored in cloud KMS such as AWS KMS, Azure Key Vault, or Google Cloud KMS
- The CMK can be used as a cryptographic kill switch to make Lakebase data inaccessible
- Lakebase uses a CMK-KEK-DEK hierarchy for envelope encryption at scale
- Account admins can register the CMK once and bind it to a workspace for all Lakebase projects

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/announcements/take-control-customer-managed-keys-for-lakebase-postgres/td-p/155338>

## Related
[[concepts/lakebase-postgres|lakebase-postgres]] · [[concepts/customer-managed-keys|customer-managed-keys]] · [[concepts/data-sovereignty|data-sovereignty]] · [[concepts/google-cloud|google-cloud]] · [[concepts/databricks|databricks]] · [[concepts/workspace|workspace]] · [[concepts/lakebase|lakebase]] · [[concepts/postgres|postgres]] · [[concepts/azure|azure]] · [[concepts/cloud|cloud]] · [[concepts/aws|aws]] · [[companies/databricks|Databricks]] · [[episodes/2026-04-24|2026-04-24]]
