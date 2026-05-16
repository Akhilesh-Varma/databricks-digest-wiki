---
type: story
story_id: rss_d95125dac3d5
episode_date: 2026-05-16
rank: 9
source: rss_feed
url: "https://arxiv.org/abs/2605.14376"
title: Fast Gossip-based Rumor Spreading using Small Messages
quality_score: 0.716
content_hash: "sha256:752a4c99ce779914a242c1779c82bca2d100599e599b0682b46f11d3f0fdbe9e"
concepts: [gossip-algorithms, rumor-spreading, graph-sketches, weak-conductance, minimum-spanning-tree, distributed-computing]
companies: []
people: [kook-jin-ahn, sudipto-guha, andrew-mcgregor]
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-16 10:20:33.544000"
tags: [story, source/rss-feed]
---

## Summary
This paper studies gossip algorithms for the rumor spreading problem, where a rumor must be disseminated from a source node to all nodes in an arbitrary and unknown graph. The authors address the limitation of existing fast gossip algorithms that require large messages (up to linear in network size n), undermining the lightweight communication advantage of gossip. They present two new gossip algorithms that achieve fast rumor spreading using only polylogarithmic message sizes. The first algorithm runs in O(c log n / Φ_c) rounds based on weak conductance, which is essentially optimal. The second algorithm runs in Õ(D√n) rounds depending on network diameter and can also output a minimum spanning tree in the same round complexity.

## Key claims
- Existing fast gossip algorithms for rumor spreading typically require message sizes linear in the network size n, undermining their lightweight communication advantage.
- The authors present two gossip algorithms that achieve fast rumor spreading using messages of only polylog n size.
- The first algorithm runs in O(c log n / Φ_c) rounds for every c ≥ 1, where Φ_c is the weak conductance, and this bound is essentially optimal.
- The second algorithm runs in Õ(D√n) rounds with high probability and is independent of the graph's conductance.
- The second algorithm can be modified to output a minimum spanning tree (MST) in the same number of rounds, which is essentially round-optimal even for non-gossip algorithms.
- The algorithms use graph sketches (Ahn, Guha, McGregor, SODA 2012) in a novel way to overcome communication bottlenecks.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2605.14376>

## Related
[[concepts/gossip-algorithms|gossip-algorithms]] · [[concepts/rumor-spreading|rumor-spreading]] · [[concepts/graph-sketches|graph-sketches]] · [[concepts/weak-conductance|weak-conductance]] · [[concepts/minimum-spanning-tree|minimum-spanning-tree]] · [[concepts/linear|linear]] · [[concepts/soda|soda]] · [[people/kook-jin-ahn|Kook Jin Ahn]] · [[people/sudipto-guha|Sudipto Guha]] · [[people/andrew-mcgregor|Andrew McGregor]] · [[episodes/2026-05-16|2026-05-16]]
