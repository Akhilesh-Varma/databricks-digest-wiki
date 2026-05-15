---
type: story
story_id: github_release_databricks_cli_318865157
episode_date: 2026-05-08
rank: 1
source: github_releases
url: "https://github.com/databricks/cli/releases/tag/v0.299.1"
title: Databricks CLI v0.299.1 released
quality_score: 0.766
content_hash: "sha256:f2a8d9b29ea524f0b1f08748ba4de01e5414834b5a4d9a182d1ecb7721dff2d5"
concepts: [databricks-cli, databricks-bundles, spog-url-convention, unified-hosts, pgx]
companies: [databricks]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-08 10:21:21.198000"
tags: [story, source/github-releases]
---

## Summary
Databricks CLI version 0.299.1 introduces several improvements to the `databricks api` command, including support for unified hosts, new flags for account and workspace scoping, and recognition of the SPOG URL convention used by the Databricks UI. JSON output formatting has been standardized for single objects. Bundle handling received fixes including validation that resource keys do not contain variable references, a fix for broken deployment state after a failed recreate, and a nil-entry guard in the `bundle debug list-targets` command. A new experimental Postgres command was added along with its dependency `github.com/jackc/pgx/v5`.

## Key claims
- databricks api command now works against unified hosts in CLI v0.299.1.
- New --account and --workspace-id flags allow per-call scoping to account API and workspace routing.
- The ?o query parameter from SPOG URLs is now recognized as a per-call workspace override.
- JSON output for single objects now uses standard key-value spacing consistent with list output.
- Bundle validation now rejects resource keys that contain variable references.
- A fix prevents broken deployment state with an invalid empty ID after a failed bundle recreate.
- An experimental Postgres command was added, introducing github.com/jackc/pgx/v5 as a new dependency.

## Source
- **Origin:** github_releases
- **URL:** <https://github.com/databricks/cli/releases/tag/v0.299.1>

## Related
[[concepts/databricks-cli|databricks-cli]] · [[concepts/databricks-bundles|databricks-bundles]] · [[concepts/spog-url-convention|spog-url-convention]] · [[concepts/unified-hosts|unified-hosts]] · [[concepts/databricks|databricks]] · [[concepts/workspace|workspace]] · [[concepts/postgres|postgres]] · [[concepts/spog|spog]] · [[concepts/json|json]] · [[concepts/cli|cli]] · [[concepts/api|api]] · [[companies/databricks|Databricks]] · [[episodes/2026-05-08|2026-05-08]]
