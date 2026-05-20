---
type: story
story_id: hn_47827486
episode_date: 2026-04-20
rank: 4
source: hacker_news
url: "https://news.ycombinator.com/item?id=47827486"
title: "Ask HN Is giving AI agents DB access the new BI-tool problem?"
quality_score: 0.781
content_hash: "sha256:c119a97099aa33c421efc55da98ef877f5645a3538dbfb2ac08bdd8342fa4612"
concepts: [bi-tools, postgres, read-replica, row-level-security, lakehouse, iceberg, delta]
companies: [snowflake, bigquery, redshift]
people: []
extractor_model: llama-3.3-70b-versatile
extracted_at: "2026-04-28 04:05:32.745000"
tags: [story, source/hacker-news]
---

## Summary
The article discusses the challenge of giving AI/ML teams access to production database data, and how it differs from providing access to BI teams. The author is seeking advice on how to handle this situation, including where the AI agent should connect and what considerations should be taken into account. The author is looking for experiences from people who have faced similar challenges. The goal is to understand the differences between giving AI/ML teams and BI teams access to database data. The author wants to know if this is a new problem or the same problem with new challenges.

## Key claims
- AI/ML teams are requesting access to production database data, which poses a new challenge.
- The challenge of giving AI/ML teams access to database data differs from giving BI teams access.
- There are various options for where the AI agent can connect, including primary with RLS, read replica, warehouse, lakehouse, or something else.
- Compliance, cost, and bad experiences are potential concerns when giving AI/ML teams access to database data.
- The author is seeking advice from people who have faced similar challenges.

## Source
- **Origin:** hacker_news
- **URL:** <https://news.ycombinator.com/item?id=47827486>

## Related
[[concepts/postgres|postgres]] · [[concepts/read-replica|read-replica]] · [[concepts/warehouse|warehouse]] · [[concepts/snowflake|snowflake]] · [[concepts/bigquery|bigquery]] · [[concepts/redshift|redshift]] · [[concepts/rls|rls]] · [[concepts/pii|pii]] · [[concepts/ai|ai]] · [[concepts/s3|s3]] · [[companies/snowflake|Snowflake]] · [[companies/bigquery|BigQuery]] · [[companies/redshift|Redshift]] · [[episodes/2026-04-20|2026-04-20]]
