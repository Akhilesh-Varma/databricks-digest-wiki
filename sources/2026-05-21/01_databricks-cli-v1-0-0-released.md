---
type: story
story_id: github_release_databricks_cli_326685849
episode_date: 2026-05-21
rank: 1
source: github_releases
url: "https://github.com/databricks/cli/releases/tag/v1.0.0"
title: Databricks CLI v1.0.0 released
quality_score: 0.859
content_hash: "sha256:d467a204eb3f4cfa067cb9f2367ef7c7d1cb5bd9709940f359487caea6205258"
concepts: [databricks-cli, semantic-versioning, oauth, os-native-secure-store, immutable-release-tags, supply-chain-attack-mitigation, databricks-asset-bundles, d-bus, databricks-aitools, claude-code, cursor, github-copilot, codex-cli]
companies: [databricks, anthropic, github, openai]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-21 10:20:19.551000"
tags: [story, source/github-releases]
---

## Summary
Databricks has released CLI v1.0.0 as the first major generally available release of its command-line interface. Starting with this version, the CLI adopts semantic versioning and uses immutable release tags to improve security against supply chain attacks. A notable breaking change moves OAuth token storage from a plain JSON file to the OS-native secure store (Keychain on macOS, Credential Manager on Windows, Secret Service on Linux) by default. The 0.299.x line will continue to receive security-critical patches through May 20, 2027. A new `databricks aitools` command group is introduced for installing Databricks skills into coding agents such as Claude Code, Cursor, and GitHub Copilot.

## Key claims
- Databricks CLI v1.0.0 is the first major generally available release and adopts semantic versioning.
- Starting with v1.0.0, the CLI uses immutable release tags to increase security against supply chain attacks.
- OAuth tokens for interactive logins are now stored in the OS-native secure store by default instead of a plain JSON file.
- Users must run 'databricks auth login' once per profile after upgrading because cached tokens from older versions are not migrated.
- The 0.299.x release line will receive security-critical patches through May 20, 2027.
- A new 'databricks aitools' command group allows installing Databricks skills into coding agents including Claude Code, Cursor, Codex CLI, and GitHub Copilot.
- On systems where the OS keyring is unreachable, the CLI transparently falls back to the file-based token cache.

## Source
- **Origin:** github_releases
- **URL:** <https://github.com/databricks/cli/releases/tag/v1.0.0>

## Related
[[concepts/databricks-cli|databricks-cli]] · [[concepts/semantic-versioning|semantic-versioning]] · [[concepts/oauth|oauth]] · [[concepts/os-native-secure-store|os-native-secure-store]] · [[concepts/immutable-release-tags|immutable-release-tags]] · [[concepts/supply-chain-attack-mitigation|supply-chain-attack-mitigation]] · [[concepts/databricks-aitools|databricks-aitools]] · [[concepts/coding-agents|coding-agents]] · [[concepts/databricks|databricks]] · [[concepts/versioning|versioning]] · [[concepts/claude|claude]] · [[concepts/codex|codex]] · [[concepts/dabs|dabs]] · [[concepts/json|json]] · [[concepts/cli|cli]] · [[companies/databricks|Databricks]] · [[companies/anthropic|Anthropic]] · [[companies/github|GitHub]] · [[companies/openai|OpenAI]] · [[episodes/2026-05-21|2026-05-21]]
