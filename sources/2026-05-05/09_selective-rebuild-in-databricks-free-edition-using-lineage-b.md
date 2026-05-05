---
type: story
story_id: rss_d95777787011
episode_date: 2026-05-05
rank: 9
source: rss_feed
url: "https://medium.com/@jr.vera.ma/selective-rebuild-in-databricks-free-edition-using-lineage-bfs-596ab06a77f6?source=rss------databricks-5"
title: Selective Rebuild In Databricks Free Edition Using Lineage BFS
quality_score: 0.691
content_hash: "sha256:2a10ca847a3f4b198f64434ba602d653a8940757a863469b856cf81a4923d59c"
concepts: [databricks-free-edition, breadth-first-search, data-lineage, selective-rebuild]
companies: [databricks, medium]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-05 10:22:14.048000"
tags: [story, source/rss-feed]
---

## Summary
The article describes a proof-of-concept built on Databricks Free Edition that addresses a practical data engineering challenge using lineage-based Breadth-First Search (BFS). The author implements a selective rebuild strategy, meaning only the affected downstream tables or assets are reprocessed when an upstream change occurs. The approach leverages data lineage graphs traversed via BFS to determine the minimal set of objects requiring rebuilding. The POC is designed to work within the constraints of the Databricks Free Edition environment.

## Key claims
- The author built a POC on Databricks Free Edition to solve a selective rebuild problem in data engineering.
- Breadth-First Search (BFS) is applied to a data lineage graph to identify downstream dependencies.
- Selective rebuild ensures only affected downstream assets are reprocessed after an upstream change.
- The solution is constrained to work within the Databricks Free Edition tier.

## Source
- **Origin:** rss_feed
- **URL:** <https://medium.com/@jr.vera.ma/selective-rebuild-in-databricks-free-edition-using-lineage-bfs-596ab06a77f6?source=rss------databricks-5>

## Related
[[concepts/databricks-free-edition|databricks-free-edition]] · [[concepts/breadth-first-search|breadth-first-search]] · [[concepts/data-lineage|data-lineage]] · [[concepts/selective-rebuild|selective-rebuild]] · [[concepts/data-engineering|data-engineering]] · [[concepts/databricks|databricks]] · [[companies/databricks|Databricks]] · [[companies/medium|Medium]] · [[episodes/2026-05-05|2026-05-05]]
