---
type: story
story_id: github_release_databricks_cli_306478567
episode_date: 2026-04-08
rank: 1
source: github_releases
url: "https://github.com/databricks/cli/releases/tag/v0.296.0"
title: Databricks CLI v0.296.0 released
quality_score: 0.764
content_hash: "sha256:ac60184d6127ca0d7531a39e7d857ca6f6387ee5ed69b2e994a0646c39d67460"
concepts: [databricks-cli, databricks-asset-bundles, direct-deployment-engine, terraform]
companies: [databricks]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:32:08.222000"
tags: [story, source/github-releases]
---

## Summary
Databricks CLI version 0.296.0 introduces the Direct deployment engine for DABs (Databricks Asset Bundles) as a Public Preview feature. Several CLI authentication improvements were made, including error handling when conflicting --profile and --host flags are used, and a new --force-refresh flag for token management. The release also includes multiple bug fixes for the Direct engine, addressing issues with grants, secret scopes, resource binding, and principal deployment. Bundle-level fixes include deduplication of grant entries and improved remote state handling during deployment.

## Key claims
- The Direct deployment engine for DABs is now in Public Preview as of CLI v0.296.0.
- CLI Auth commands now return an error when --profile and --host flags conflict.
- A new --force-refresh flag was added to the databricks auth token command to force token refresh even when a cached token is still valid.
- Bundle deployment bind now always pulls remote state before modifying.
- The Direct engine fixes include resolving drift in grants due to privilege reordering and a 400 error when deploying grants with ALL_PRIVILEGES.
- Secret scope permissions migration from Terraform to the Direct engine was fixed.
- Duplicate grant entries with duplicate principals or privileges are now deduplicated during initialization.

## Source
- **Origin:** github_releases
- **URL:** <https://github.com/databricks/cli/releases/tag/v0.296.0>

## Related
[[concepts/databricks-cli|databricks-cli]] · [[concepts/databricks-asset-bundles|databricks-asset-bundles]] · [[concepts/direct-deployment-engine|direct-deployment-engine]] · [[concepts/deployment-bind|deployment-bind]] · [[concepts/databricks|databricks]] · [[concepts/cli|cli]] · [[companies/databricks|Databricks]] · [[episodes/2026-04-08|2026-04-08]]
