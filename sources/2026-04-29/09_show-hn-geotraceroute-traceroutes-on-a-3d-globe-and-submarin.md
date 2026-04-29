---
type: story
story_id: hn_47943252
episode_date: 2026-04-29
rank: 9
source: hacker_news
url: "https://geotraceroute.com"
title: Show HN GeoTraceroute Traceroutes on a 3D globe and submarine cables
quality_score: 0.634
content_hash: "sha256:c3889d31563352a130d6697317ca4409e558c9ad33a57ff92ab70a81b767aad3"
concepts: [traceroute, icmp, geolocation, pathfinding]
companies: []
people: [salim]
extractor_model: gemini-2.5-flash-lite
extracted_at: "2026-04-29 10:21:13.856000"
tags: [story, source/hacker-news]
---

## Summary
GeoTraceroute v2.3 now infers submarine cable routes, a significant addition to its network tracing capabilities. The tool visualizes network paths on a 3D globe, 2D map, and topological view, featuring 320 community-contributed nodes across 50 countries. Standard traceroute struggles with underwater segments as cable routers don't respond to ICMP. GeoTraceroute overcomes this by detecting ocean crossings via geolocation deltas between hops and inferring cable paths using a graph of landing points and pathfinding algorithms. Coverage is currently strongest in the EU and US, with plans to expand to other regions.

## Key claims
- GeoTraceroute v2.3 has been released with submarine cable inference.
- The tool visualizes network paths on a 3D globe, 2D map, and topological mode.
- GeoTraceroute utilizes 320 community-contributed nodes across 50 countries.
- Submarine cable routing is inferred by detecting ocean crossings via geolocation deltas between hops.
- The tool infers cable paths using a geo graph of landing points and pathfinding.
- Coverage is currently better in the EU and US compared to Asia, Africa, and South America.

## Source
- **Origin:** hacker_news
- **URL:** <https://geotraceroute.com>

## Related
[[concepts/traceroute|traceroute]] · [[concepts/geolocation|geolocation]] · [[concepts/pathfinding|pathfinding]] · [[concepts/views|views]] · [[concepts/delta|delta]] · [[people/salim|Salim]] · [[episodes/2026-04-29|2026-04-29]]
