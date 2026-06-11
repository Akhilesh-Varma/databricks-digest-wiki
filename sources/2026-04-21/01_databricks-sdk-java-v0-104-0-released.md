---
type: story
story_id: github_release_databricks_databricks-sdk-java_311121577
episode_date: 2026-04-21
rank: 1
source: github_releases
url: "https://github.com/databricks/databricks-sdk-java/releases/tag/v0.104.0"
title: Databricks SDK Java v0.104.0 released
quality_score: 0.766
content_hash: "sha256:89f00790cfad0d2f55dc5835f38242d0b9bb2a6eafb7c36eecacac9d98396646"
concepts: [databricks-sdk-java, azure-managed-service-identity, ai-coding-agents]
companies: [databricks]
people: []
extractor_model: llama-3.3-70b-versatile
extracted_at: "2026-04-28 04:03:26.296000"
tags: [story, source/github-releases]
---

## Summary
Databricks SDK Java v0.104.0 has been released with new features and improvements, including support for authentication through Azure Managed Service Identity and automatic detection of AI coding agents. The SDK also includes bug fixes, such as handling non-JSON error responses and detecting scope mismatches in cached tokens. Additionally, internal changes have been made to introduce a logging abstraction and improve token federation.

## Key claims
- Databricks SDK Java v0.104.0 supports authentication through Azure Managed Service Identity via the new azure-msi credential provider.
- The SDK automatically detects AI coding agents in the user-agent string and appends agent to HTTP request headers.
- The SDK now raises an error when the cached token's scopes don't match the SDK's configured scopes, instead of silently ignoring the mismatch.
- The release includes bug fixes for handling non-JSON error responses and adds a logging abstraction to decouple the SDK from a specific logging backend.

## Source
- **Origin:** github_releases
- **URL:** <https://github.com/databricks/databricks-sdk-java/releases/tag/v0.104.0>

## Related
[[concepts/databricks-sdk-java|databricks-sdk-java]] · [[concepts/azure-managed-service-identity|azure-managed-service-identity]] · [[concepts/deserialization|deserialization]] · [[concepts/databricks-cli|databricks-cli]] · [[concepts/coding-agents|coding-agents]] · [[concepts/claude-code|claude-code]] · [[concepts/databricks|databricks]] · [[concepts/gemini-cli|gemini-cli]] · [[concepts/workspace|workspace]] · [[concepts/ai-agent|ai-agent]] · [[concepts/metadata|metadata]] · [[concepts/claude|claude]] · [[concepts/cursor|cursor]] · [[concepts/azure|azure]] · [[concepts/codex|codex]] · [[concepts/scim|scim]] · [[concepts/spog|spog]] · [[concepts/json|json]] · [[concepts/sdk|sdk]] · [[concepts/cli|cli]] · [[concepts/ai|ai]] · [[companies/databricks|Databricks]] · [[episodes/2026-04-21|2026-04-21]]
