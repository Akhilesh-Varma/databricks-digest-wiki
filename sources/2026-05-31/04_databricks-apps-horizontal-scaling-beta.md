---
type: story
story_id: rss_079d8d7a8eba
episode_date: 2026-05-31
rank: 4
source: rss_feed
url: "https://docs.databricks.com/aws/en/release-notes/product/2026/may#databricks-apps-horizontal-scaling-beta"
title: Databricks Apps horizontal scaling Beta
quality_score: 0.766
content_hash: "sha256:3ee0e9807cfd244bfe627b1313aef667c12334f7ae8711dabfe1f2eae7a457da"
concepts: [databricks-apps, horizontal-scaling, session-affinity, zero-downtime-deployment]
companies: [databricks]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-31 10:17:15.563000"
tags: [story, source/rss-feed]
---

## Summary
Databricks has released a beta feature allowing Databricks Apps to run across multiple instances behind a single app URL. This horizontal scaling capability provides higher availability, zero-downtime deployments, and session affinity that routes each user's requests to the same instance. Existing standard apps can be converted to horizontally scaled apps, or the feature can be enabled during new app creation. Additionally, converted apps can opt out of pre-installed Python libraries to run on a clean base OS image.

## Key claims
- Databricks Apps can now run across multiple instances behind a single app URL in beta.
- Horizontal scaling for Databricks Apps provides higher availability and zero-downtime deployments.
- Session affinity routes every request from a given user to the same instance to preserve per-user data.
- Existing standard Databricks Apps can be converted to horizontally scaled apps.
- Horizontally scaled apps can opt out of pre-installed Python libraries to run on a clean base OS image.

## Source
- **Origin:** rss_feed
- **URL:** <https://docs.databricks.com/aws/en/release-notes/product/2026/may#databricks-apps-horizontal-scaling-beta>

## Related
[[concepts/databricks-apps|databricks-apps]] · [[concepts/horizontal-scaling|horizontal-scaling]] · [[concepts/session-affinity|session-affinity]] · [[concepts/zero-downtime-deployment|zero-downtime-deployment]] · [[concepts/databricks|databricks]] · [[concepts/python|python]] · [[companies/databricks|Databricks]] · [[episodes/2026-05-31|2026-05-31]]
