---
type: story
story_id: rss_c4814b5a9d54
episode_date: 2026-04-27
rank: 7
source: rss_feed
url: "https://medium.com/@karumajji/inside-lakebase-the-architecture-that-makes-serverless-postgres-actually-work-f05ae2a9c103?source=rss------databricks-5"
title: Inside Lakebase The Architecture that makes Serverless Postgres actually work
quality_score: 0.733
content_hash: "sha256:4ed307401cf7a35c88e9848b5b74dc0772aedffc290cd835ee9ec58c7c6256aa"
concepts: [postgres, compute-storage-separation, wal-quorum, pageserver, stateless-compute, zero-downtime-patching]
companies: [databricks]
people: []
extractor_model: gemini-2.5-flash-lite
extracted_at: "2026-04-28 03:21:40.495000"
tags: [story, source/rss-feed]
---

## Summary
Lakebase is an architecture designed to enable serverless Postgres functionality. It achieves this through compute-storage separation, a WAL quorum mechanism, and the internal workings of its pageserver. The stateless compute layer is key to enabling zero-downtime patching, making the system highly available and maintainable.

## Key claims
- Lakebase is an architecture that enables serverless Postgres.
- The architecture relies on compute-storage separation.
- WAL quorum is a critical component of Lakebase.
- Pageserver internals are part of the Lakebase design.
- Stateless compute allows for zero-downtime patching.

## Source
- **Origin:** rss_feed
- **URL:** <https://medium.com/@karumajji/inside-lakebase-the-architecture-that-makes-serverless-postgres-actually-work-f05ae2a9c103?source=rss------databricks-5>

## Related
[[concepts/postgres|postgres]] · [[concepts/compute-storage-separation|compute-storage-separation]] · [[concepts/wal-quorum|wal-quorum]] · [[concepts/pageserver|pageserver]] · [[concepts/stateless-compute|stateless-compute]] · [[concepts/zero-downtime-patching|zero-downtime-patching]] · [[companies/databricks|Databricks]] · [[episodes/2026-04-27|2026-04-27]]
