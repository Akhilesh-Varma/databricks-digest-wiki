---
type: story
story_id: github_release_databricks_terraform-provider-databricks_315072156
episode_date: 2026-04-29
rank: 1
source: github_releases
url: "https://github.com/databricks/terraform-provider-databricks/releases/tag/v1.114.0"
title: Databricks Terraform Provider v1.114.0 released
quality_score: 0.779
content_hash: "sha256:e718adda93e0b57fa6558514803500c463bd833c0f2add959a146c5dd0d196b2"
concepts: [databricks-terraform-provider, unity-catalog, disaster-recovery-failover-group, disaster-recovery-stable-url, supervisor-agent, go-sdk, tls-1-3, terraform]
companies: [databricks]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-04-29 10:19:28.631000"
tags: [story, source/github-releases]
---

## Summary
Databricks released version 1.114.0 of its Terraform Provider, introducing several new resources and data sources. The update adds support for disaster recovery failover groups and stable URLs, supervisor agents and their tools, and a new Unity Catalog secret resource. It also enables adoption of pre-existing PostgreSQL branch and endpoint resources via a new argument. Internally, the release bumps the Go SDK to v0.128.0 and raises the minimum Go toolchain version to 1.25.7 to incorporate a TLS 1.3 session-resumption fix.

## Key claims
- Databricks Terraform Provider v1.114.0 adds resource and data sources for databricks_disaster_recovery_failover_group and databricks_disaster_recovery_stable_url.
- The release introduces resource and data sources for databricks_supervisor_agent and databricks_supervisor_agent_tool.
- A new databricks_secret_uc resource and data source is added for Unity Catalog secrets.
- Pre-existing databricks_postgres_branch and databricks_postgres_endpoint resources can now be adopted via a replace_existing true argument.
- The Go SDK dependency is updated to v0.128.0.
- The minimum Go toolchain is bumped from 1.24.0 to 1.25.7 to pick up a TLS 1.3 session-resumption fix.
- The provider now fails at plan time when the api field is not set for dual workspace/account resources configured against a unified host.

## Source
- **Origin:** github_releases
- **URL:** <https://github.com/databricks/terraform-provider-databricks/releases/tag/v1.114.0>

## Related
[[concepts/databricks-terraform-provider|databricks-terraform-provider]] · [[concepts/unity-catalog|unity-catalog]] · [[concepts/disaster-recovery-failover-group|disaster-recovery-failover-group]] · [[concepts/disaster-recovery-stable-url|disaster-recovery-stable-url]] · [[concepts/supervisor-agent|supervisor-agent]] · [[concepts/go-sdk|go-sdk]] · [[concepts/terraform|terraform]] · [[concepts/databricks-postgres-endpoint|databricks-postgres-endpoint]] · [[concepts/databricks-postgres-branch|databricks-postgres-branch]] · [[concepts/unified-host|unified-host]] · [[concepts/workspace|workspace]] · [[concepts/sdk|sdk]] · [[concepts/api|api]] · [[companies/databricks|Databricks]] · [[episodes/2026-04-29|2026-04-29]]
