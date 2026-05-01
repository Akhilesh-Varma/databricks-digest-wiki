---
type: story
story_id: github_release_databricks_databricks-sdk-java_312638599
episode_date: 2026-04-23
rank: 2
source: github_releases
url: "https://github.com/databricks/databricks-sdk-java/releases/tag/v0.105.0"
title: Databricks SDK Java v0.105.0 released
quality_score: 0.78
content_hash: "sha256:9f83d74ac0c42b96720039df7a7f12e0365b9bea999942b988f75129d313b031"
concepts: [databricks-sdk-java, agent-standard]
companies: [databricks]
people: []
extractor_model: llama-3.3-70b-versatile
extracted_at: "2026-04-28 04:00:31.718000"
tags: [story, source/github-releases]
---

## Summary
Databricks SDK Java v0.105.0 has been released with new features and improvements, including automatic detection of AI coding agents and honors the AGENT standard. The SDK now appends the agent to HTTP request headers when running inside a known AI agent environment. Breaking changes include the removal of the experimentalIsUnifiedHost field and the DATABRICKS_EXPERIMENTAL_IS_UNIFIED_HOST environment variable. Bug fixes include adding the X-Databricks-Org-Id header to SharesExtImpl.list for SPOG host compatibility.

## Key claims
- Databricks SDK Java v0.105.0 has been released with new features and improvements.
- The SDK now automatically detects AI coding agents and appends the agent to HTTP request headers.
- The SDK honors the AGENT standard when AGENT is set to a known product name.
- The experimentalIsUnifiedHost field and the DATABRICKS_EXPERIMENTAL_IS_UNIFIED_HOST environment variable have been removed.
- A bug fix adds the X-Databricks-Org-Id header to SharesExtImpl.list for SPOG host compatibility.

## Source
- **Origin:** github_releases
- **URL:** <https://github.com/databricks/databricks-sdk-java/releases/tag/v0.105.0>

## Related
[[concepts/databricks-sdk-java|databricks-sdk-java]] · [[concepts/agent-standard|agent-standard]] · [[concepts/ai-coding-agents|ai-coding-agents]] · [[concepts/coding-agents|coding-agents]] · [[concepts/unified-host|unified-host]] · [[concepts/claude-code|claude-code]] · [[concepts/databricks|databricks]] · [[concepts/openclaw|openclaw]] · [[concepts/codex|codex]] · [[concepts/oauth|oauth]] · [[concepts/spog|spog]] · [[concepts/sdk|sdk]] · [[concepts/cli|cli]] · [[concepts/ai|ai]] · [[companies/databricks|Databricks]] · [[episodes/2026-04-23|2026-04-23]]
