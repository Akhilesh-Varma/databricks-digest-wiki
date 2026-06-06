---
type: story
story_id: hn_48410522
episode_date: 2026-06-06
rank: 6
source: hacker_news
url: "https://news.ycombinator.com/item?id=48410522"
title: "Ask HN Is Azure capacity this constraind or am I doing it wrong?"
quality_score: 0.655
content_hash: "sha256:da21dcc185ec286a2d01f6071708e70e1b18d7d03d92423ab75a38ccdbc20016"
concepts: [azure-kubernetes-service, postgres-flexible-server, vcpu-quota, standard-dasv7-family, cloud-agnostic-infrastructure]
companies: [microsoft-azure, amazon-web-services]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-06-06 10:19:12.233000"
tags: [story, source/hacker-news]
---

## Summary
A developer with extensive AWS experience is attempting to deploy cloud-agnostic infrastructure on Azure and is encountering severe capacity constraints. After being redirected from US East to US East 2 due to Postgres Flexible Server availability issues, they are now blocked by vCPU quota limits for the Standard Dasv5 family on AKS. Azure support has responded with a boilerplate message indicating the quota request has been backlogged with no ETA. The developer is asking the Hacker News community for Azure regions and instance types that are less capacity-constrained.

## Key claims
- The developer was redirected from US East to US East 2 by Azure support due to Postgres Flexible Server capacity issues.
- After moving to US East 2, the developer hit a vCPU quota limit of 100 for the Standard Dasv7 Family when deploying AKS.
- Azure support responded with a templated message stating the quota request was backlogged with no ETA.
- The developer has been waiting more than one day with no substantive response from Azure support.
- The developer is considering abandoning Azure due to capacity and support responsiveness issues.
- The article highlights a contrast in experience between AWS and Azure for infrastructure provisioning.

## Source
- **Origin:** hacker_news
- **URL:** <https://news.ycombinator.com/item?id=48410522>

## Related
[[concepts/azure-kubernetes-service|azure-kubernetes-service]] · [[concepts/postgres-flexible-server|postgres-flexible-server]] · [[concepts/vcpu-quota|vcpu-quota]] · [[concepts/standard-dasv7-family|standard-dasv7-family]] · [[concepts/cloud-agnostic-infrastructure|cloud-agnostic-infrastructure]] · [[concepts/postgres|postgres]] · [[concepts/azure|azure]] · [[concepts/cloud|cloud]] · [[concepts/aws|aws]] · [[companies/microsoft-azure|Microsoft Azure]] · [[companies/amazon-web-services|Amazon Web Services]] · [[episodes/2026-06-06|2026-06-06]]
