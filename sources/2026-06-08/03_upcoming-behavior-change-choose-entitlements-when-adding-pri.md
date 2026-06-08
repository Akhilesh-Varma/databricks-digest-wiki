---
type: story
story_id: rss_48ae48a75e17
episode_date: 2026-06-08
rank: 3
source: rss_feed
url: "https://docs.databricks.com/aws/en/release-notes/whats-coming#upcoming-behavior-change-choose-entitlements-when-adding-principals-to-workspaces"
title: Upcoming behavior change Choose entitlements when adding principals to workspaces
quality_score: 0.874
content_hash: "sha256:1b9558712034adb97e51fa93665047d9ab801be239e9668f1081d44e07e0b2ab"
concepts: [workspace-entitlements, scim, terraform, databricks-sql, workspace-scim-api, system-groups]
companies: [databricks]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-06-08 10:19:40.705000"
tags: [story, source/rss-feed]
---

## Summary
Databricks is changing how workspace entitlements are assigned to principals, moving from automatic inheritance via the 'users' system group to explicit entitlement grants. After the change, the 'users' system group will have no entitlements, and administrators must explicitly assign access levels when adding principals to a workspace. Databricks will automatically migrate existing entitlements to a new clone group named 'users-clone-<TIMESTAMP>'. Workspace administrators can opt in starting June 15, 2026, with the new behavior enforced for all workspaces on September 14, 2026. Organizations using automation such as Terraform or SCIM APIs must update their workflows to target standard account groups instead of system groups.

## Key claims
- Databricks is changing workspace entitlement assignment from automatic inheritance to explicit grants when adding principals.
- After the change, the 'users' system group will have no entitlements and the 'admins' group will have all workspace entitlements, with both groups locked.
- Workspace administrators can opt in to the new behavior starting June 15, 2026; it becomes enforced for all workspaces on September 14, 2026.
- Databricks will automatically migrate entitlements previously granted to 'users' into a new workspace-local clone group named 'users-clone-<TIMESTAMP>'.
- Automation workflows using Terraform, Workspace SCIM APIs, or custom scripts must be updated to target standard account groups, not system groups.
- Nesting 'users' or 'admins' as members of other groups will no longer be permitted under the new behavior.
- If a SCIM sync deletes unrecognized workspace groups, its configuration must be updated to preserve the migration clone group to avoid principals losing entitlements.

## Source
- **Origin:** rss_feed
- **URL:** <https://docs.databricks.com/aws/en/release-notes/whats-coming#upcoming-behavior-change-choose-entitlements-when-adding-principals-to-workspaces>

## Related
[[concepts/workspace-entitlements|workspace-entitlements]] · [[concepts/scim|scim]] · [[concepts/workspace-scim-api|workspace-scim-api]] · [[concepts/system-groups|system-groups]] · [[concepts/access-control|access-control]] · [[concepts/genie-spaces|genie-spaces]] · [[concepts/databricks|databricks]] · [[concepts/workflows|workflows]] · [[concepts/workspace|workspace]] · [[concepts/genie|genie]] · [[concepts/sql|sql]] · [[companies/databricks|Databricks]] · [[episodes/2026-06-08|2026-06-08]]
