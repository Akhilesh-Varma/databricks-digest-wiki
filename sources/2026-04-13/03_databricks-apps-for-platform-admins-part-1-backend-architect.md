---
type: story
story_id: community_5deaad498779
episode_date: 2026-04-13
rank: 3
source: databricks_community
url: "https://community.databricks.com/t5/technical-blog/databricks-apps-for-platform-admins-part-1-backend-architecture/ba-p/152208"
title: Databricks Apps for Platform Admins Part 1 Backend Architecture and Access Control
quality_score: 0.78
content_hash: "sha256:b3ca127c9af190f2f5c72d41a5201ee6483a59a514caaff8173e3d4a4949e0ba"
concepts: [databricks-apps, unity-catalog, serverless-compute, service-principal, streamlit, dash, gradio, flask, react, row-level-security, column-masking, sso]
companies: [databricks, github, gitlab, bitbucket]
people: [peyman-nasirifard]
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:22:07.112000"
tags: [story, source/databricks-community]
---

## Summary
This article is the first part of a multi-part blog series aimed at platform admins governing Databricks Apps. It explains the execution model, where apps run on serverless compute with no cluster management, and are deployed as Python or Node.js applications with a unique URL. The post details a two-level workspace permission model (CAN MANAGE and CAN USE) and a dual authorization framework combining app-level service principal authentication and user-level identity passthrough. Key governance concepts such as billing states, SSO enforcement, Unity Catalog policy integration, and authorization scopes are covered to help admins safely roll out Apps in their organizations.

## Key claims
- Databricks Apps run on serverless compute, requiring no cluster configuration, and are accessible via a unique URL on the databricksapps.com domain.
- Supported frameworks for Databricks Apps include Streamlit, Dash, Gradio, Flask, and React, with source code hosted in workspace folders or Git repositories.
- Apps are only billed when in the Running state; Stopped, Deploying, and Crashed states incur no charges.
- The workspace-level permission model has two levels: CAN MANAGE (edit, delete, configure) and CAN USE (run and interact only), assignable to users, groups, or service principals.
- Every Databricks App automatically receives a dedicated service principal, with credentials injected as environment variables for machine-to-machine authorization.
- User Authorization mode (Public Preview as of March 25, 2026) allows the app to act with the calling user's identity, enforcing Unity Catalog row-level filters, column masks, and table ACLs.
- Apps must declare authorization scopes to limit API access; if none are selected, Databricks assigns default scopes for basic user identity retrieval.

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/technical-blog/databricks-apps-for-platform-admins-part-1-backend-architecture/ba-p/152208>

## Related
[[concepts/databricks-apps|databricks-apps]] · [[concepts/unity-catalog|unity-catalog]] · [[concepts/serverless-compute|serverless-compute]] · [[concepts/service-principal|service-principal]] · [[concepts/databricks-serverless-compute|databricks-serverless-compute]] · [[concepts/databricks-workspace|databricks-workspace]] · [[concepts/app-authorization|app-authorization]] · [[concepts/access-control|access-control]] · [[concepts/sql-warehouse|sql-warehouse]] · [[concepts/genie-space|genie-space]] · [[concepts/databricks|databricks]] · [[concepts/governance|governance]] · [[concepts/workspace|workspace]] · [[concepts/snapshot|snapshot]] · [[concepts/node-js|node-js]] · [[concepts/python|python]] · [[concepts/genie|genie]] · [[concepts/sql|sql]] · [[concepts/api|api]] · [[concepts/git|git]] · [[concepts/ai|ai]] · [[companies/databricks|Databricks]] · [[companies/github|GitHub]] · [[companies/gitlab|GitLab]] · [[companies/bitbucket|Bitbucket]] · [[people/peyman-nasirifard|Peyman Nasirifard]] · [[episodes/2026-04-13|2026-04-13]]
