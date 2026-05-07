---
type: story
story_id: github_release_databricks_cli_315656703
episode_date: 2026-04-30
rank: 1
source: github_releases
url: "https://github.com/databricks/cli/releases/tag/v0.299.0"
title: Databricks CLI v0.299.0 released
quality_score: 0.779
content_hash: "sha256:874bbe1035ce24175cb31fa0153720a67913c1ec60562c00cfd20dd6abcd86e5"
concepts: [oauth, token-cache, unified-host, interactive-pagination, secure-token-storage]
companies: [databricks]
people: []
extractor_model: gemini-2.5-flash-lite
extracted_at: "2026-04-30 10:17:02.020000"
tags: [story, source/github-releases]
---

## Summary
Databricks CLI version 0.299.0 has been released, introducing several key changes. The CLI now solely manages its file-based OAuth token cache, moving this responsibility from the SDK. Experimental flags related to unified hosts have been removed, with unified host detection now relying exclusively on .well-known discovery. Interactive pagination has been added to list commands for improved user experience, and an opt-in feature for OS-native secure token storage is now available. Additionally, a fix has been implemented for a panic in the `update-default-warehouse-override` command.

## Key claims
- Databricks CLI v0.299.0 has been released.
- File-based OAuth token cache management has been moved from the SDK to the CLI.
- Experimental flags for unified hosts have been removed, with discovery now using .well-known endpoints.
- Interactive pagination is now available for list commands.
- An opt-in feature for OS-native secure token storage has been added.
- A bug causing a panic in `update-default-warehouse-override` has been fixed.

## Source
- **Origin:** github_releases
- **URL:** <https://github.com/databricks/cli/releases/tag/v0.299.0>

## Related
[[concepts/token-cache|token-cache]] · [[concepts/unified-host|unified-host]] · [[concepts/interactive-pagination|interactive-pagination]] · [[concepts/secure-token-storage|secure-token-storage]] · [[concepts/oauth-token|oauth-token]] · [[concepts/databricks|databricks]] · [[concepts/schema|schema]] · [[concepts/sdk|sdk]] · [[concepts/cli|cli]] · [[companies/databricks|Databricks]] · [[episodes/2026-04-30|2026-04-30]]
