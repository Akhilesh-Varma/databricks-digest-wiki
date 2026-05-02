---
type: story
story_id: github_release_databricks_terraform-provider-databricks_309702091
episode_date: 2026-04-16
rank: 2
source: github_releases
url: "https://github.com/databricks/terraform-provider-databricks/releases/tag/v1.113.0"
title: Databricks Terraform Provider v1.113.0 released
quality_score: 0.818
content_hash: "sha256:cf320429a28dcdb29aebbd543675b1005a3728a25fb39ad306811f5ed28cb636"
concepts: [databricks-terraform-provider, terraform, unity-catalog, databricks-postgres-catalog, databricks-postgres-synced-table, databricks-current-config, databricks-grant]
companies: [databricks]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:11:56.334000"
tags: [story, source/github-releases]
---

## Summary
Databricks released version 1.113.0 of its Terraform Provider, introducing several new resources and data sources. Key additions include support for PostgreSQL catalog and synced table resources, as well as workspace base environment resources. The release also adds an optional cloud argument to the databricks_current_config data source and an api field to dual account workspace resources to explicitly control API level. Bug fixes address import inconsistencies and provider configuration handling for grants.

## Key claims
- v1.113.0 adds resource and data source support for databricks_postgres_catalog and databricks_postgres_synced_table.
- New resources and data sources for databricks_environments_workspace_base_environment and databricks_environments_default_workspace_base_environment were introduced.
- An optional cloud argument was added to databricks_current_config to explicitly set the cloud type (aws, azure, gcp) instead of relying on host-based detection.
- An api field was added to numerous dual account workspace resources to explicitly control whether account-level or workspace-level APIs are used.
- The api field enables support for unified hosts like api.databricks.com where the API level cannot be inferred from the host.
- A bug causing Provider produced inconsistent final plan errors for force_destroy and schema-only fields during import was fixed.
- databricks_grant and databricks_grants were fixed to honor provider_config when using account-level providers.

## Source
- **Origin:** github_releases
- **URL:** <https://github.com/databricks/terraform-provider-databricks/releases/tag/v1.113.0>

## Related
[[concepts/databricks-terraform-provider|databricks-terraform-provider]] · [[concepts/terraform|terraform]] · [[concepts/databricks-postgres-catalog|databricks-postgres-catalog]] · [[concepts/databricks-postgres-synced-table|databricks-postgres-synced-table]] · [[concepts/databricks-current-config|databricks-current-config]] · [[concepts/databricks-grant|databricks-grant]] · [[concepts/databricks|databricks]] · [[concepts/workspace|workspace]] · [[concepts/azure|azure]] · [[concepts/aws|aws]] · [[concepts/api|api]] · [[companies/databricks|Databricks]] · [[episodes/2026-04-16|2026-04-16]]
