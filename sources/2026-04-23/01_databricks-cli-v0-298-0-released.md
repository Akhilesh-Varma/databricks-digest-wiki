---
type: story
story_id: github_release_databricks_cli_312213931
episode_date: 2026-04-23
rank: 1
source: github_releases
url: "https://github.com/databricks/cli/releases/tag/v0.298.0"
title: Databricks CLI v0.298.0 released
quality_score: 0.887
content_hash: "sha256:77c746a0db7143f9b4b6cda82830af4ec7675290bf66b10c91d86a9e86c75df8"
concepts: [databricks-cli, lakebase, vector-search-endpoints, pydabs]
companies: [databricks]
people: []
extractor_model: llama-3.3-70b-versatile
extracted_at: "2026-04-28 04:00:22.452000"
tags: [story, source/github-releases]
---

## Summary
Databricks has released version 0.298.0 of its CLI, which includes several updates and improvements. The --limit flag has been added to all paginated list commands for client-side result capping. The former API page-size flag has been renamed to --page-size and is now hidden to avoid collision. The CLI also now caches .well-known databricks-config lookups under .cache databricks host-metadata. Additionally, the auth env has been deprecated and will be removed in a future release.

## Key claims
- Databricks CLI v0.298.0 has been released with several updates and improvements.
- The --limit flag has been added to all paginated list commands for client-side result capping.
- The former API page-size flag has been renamed to --page-size and is now hidden.
- The CLI now caches .well-known databricks-config lookups under .cache databricks host-metadata.
- The auth env has been deprecated and will be removed in a future release.

## Source
- **Origin:** github_releases
- **URL:** <https://github.com/databricks/cli/releases/tag/v0.298.0>

## Related
[[concepts/databricks-cli|databricks-cli]] · [[concepts/vector-search|vector-search]] · [[concepts/databricks|databricks]] · [[concepts/postgres|postgres]] · [[concepts/metadata|metadata]] · [[concepts/cli|cli]] · [[concepts/api|api]] · [[companies/databricks|Databricks]] · [[episodes/2026-04-23|2026-04-23]]
