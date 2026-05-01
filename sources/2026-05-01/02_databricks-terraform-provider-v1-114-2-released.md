---
type: story
story_id: github_release_databricks_terraform-provider-databricks_315983586
episode_date: 2026-05-01
rank: 2
source: github_releases
url: "https://github.com/databricks/terraform-provider-databricks/releases/tag/v1.114.2"
title: Databricks Terraform Provider v1.114.2 released
quality_score: 0.711
content_hash: "sha256:8c12ab327e16fe02a8dfc89c6dc442fd4be15905dd5f709e7aa44619f0e7f2ff"
concepts: [terraform-provider, unity-catalog, databricks-postgres-branch, databricks-postgres-endpoint, databricks-external-location, terraform-drift]
companies: [databricks, hashicorp]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-01 10:19:07.240000"
tags: [story, source/github-releases]
---

## Summary
Databricks released version 1.114.2 of its Terraform Provider. The release adds support for adopting pre-existing databricks_postgres_branch and databricks_postgres_endpoint resources using a replace_existing true argument. An internal change marks the effective_file_event_queue field as computed with diff suppression in databricks_external_location to prevent Terraform drift caused by server-populated values returned by the Unity Catalog backend.

## Key claims
- Databricks Terraform Provider v1.114.2 was released.
- The release adds support for adopting pre-existing databricks_postgres_branch resources via a replace_existing true argument.
- The release adds support for adopting pre-existing databricks_postgres_endpoint resources via a replace_existing true argument.
- effective_file_event_queue is now marked as computed with diff suppression in databricks_external_location.
- The diff suppression change prevents Terraform drift when Unity Catalog backend returns the server-populated effective_file_event_queue field.

## Source
- **Origin:** github_releases
- **URL:** <https://github.com/databricks/terraform-provider-databricks/releases/tag/v1.114.2>

## Related
[[concepts/terraform-provider|terraform-provider]] · [[concepts/unity-catalog|unity-catalog]] · [[concepts/databricks-postgres-branch|databricks-postgres-branch]] · [[concepts/databricks-postgres-endpoint|databricks-postgres-endpoint]] · [[concepts/databricks-external-location|databricks-external-location]] · [[concepts/terraform-drift|terraform-drift]] · [[concepts/terraform|terraform]] · [[companies/databricks|Databricks]] · [[companies/hashicorp|HashiCorp]] · [[episodes/2026-05-01|2026-05-01]]
