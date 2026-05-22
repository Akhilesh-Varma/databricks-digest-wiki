---
type: story
story_id: devto_3506857
episode_date: 2026-04-16
rank: 9
source: devto
url: "https://dev.to/alexmercedcoder/apache-data-lakehouse-weekly-april-9-15-2026-51c7"
title: "Apache Data Lakehouse Weekly April 9 15, 2026"
quality_score: 0.831
content_hash: "sha256:b9d7ac514cf139143148f8b1406b8116e6148316dae938d824d73fbaf9f1b535"
concepts: [apache-iceberg, apache-polaris, apache-parquet, apache-arrow, data-lakehouse, v4-metadata-json, one-file-commits, manifest-delete-vectors, alp-encoding, iceberg-summit, apache-software-foundation-pmc]
companies: [apache-software-foundation, dremio]
people: [anton-okolnychyi, yufei-gu, shawn-chang, steven-wu, russell-spitzer, amogh-jahagirdar, peter-vary, holden-karau, kevin-liu, steve-loughran, sung-yun, jean-baptiste-onofre]
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:14:29.701000"
tags: [story, source/devto]
---

## Summary
The week of April 9–15, 2026 saw post-Iceberg Summit momentum translate into concrete proposals across several Apache projects. Key Apache Iceberg discussions included V4 metadata.json optionality, one-file commits replacing manifest lists, efficient column updates for AI/ML workloads, and an AI contribution policy. Apache Polaris, one month past its graduation as a top-level Apache project, published its first board report under PMC governance. Apache Parquet's ALP encoding vote closed, and Apache Arrow's community addressed Java baseline and AI tooling policy decisions.

## Key claims
- The Iceberg Summit in San Francisco produced alignment on V4 metadata.json optionality, favoring catalog-managed metadata as a first-class supported mode with explicit opt-in portability semantics.
- Russell Spitzer and Amogh Jahagirdar's one-file commits design replaces manifest lists with root manifests and uses manifest delete vectors to enable single-file commits, reducing commit latency and metadata storage footprint.
- Péter Váry proposed efficient column updates for AI/ML workloads, allowing Iceberg to write only updated columns to separate files and merge at read time, targeting wide tables like feature stores.
- An AI contribution policy covering disclosure requirements and code provenance standards for AI-generated contributions was expected to be published on the Apache Iceberg dev list following the summit.
- Apache Polaris graduated as a top-level Apache project on February 18, 2026, and Jean-Baptiste Onofré filed its first board report covering the March 26 ASF board meeting.
- Apache Parquet's ALP encoding vote closed during the week, and Polaris 1.4.0 planning accelerated post-summit.
- Apache Arrow's engineering community addressed two linked decisions about its future Java baseline and AI tooling policy.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/alexmercedcoder/apache-data-lakehouse-weekly-april-9-15-2026-51c7>

## Related
[[concepts/apache-iceberg|apache-iceberg]] · [[concepts/apache-polaris|apache-polaris]] · [[concepts/apache-parquet|apache-parquet]] · [[concepts/apache-arrow|apache-arrow]] · [[concepts/data-lakehouse|data-lakehouse]] · [[concepts/v4-metadata-json|v4-metadata-json]] · [[concepts/one-file-commits|one-file-commits]] · [[concepts/manifest-delete-vectors|manifest-delete-vectors]] · [[concepts/alp-encoding|alp-encoding]] · [[concepts/iceberg-summit|iceberg-summit]] · [[concepts/apache-software-foundation-pmc|apache-software-foundation-pmc]] · [[concepts/feature-stores|feature-stores]] · [[concepts/governance|governance]] · [[concepts/parquet|parquet]] · [[concepts/iceberg|iceberg]] · [[concepts/dremio|dremio]] · [[concepts/merge|merge]] · [[concepts/json|json]] · [[concepts/ai|ai]] · [[companies/apache-software-foundation|Apache Software Foundation]] · [[companies/dremio|Dremio]] · [[people/anton-okolnychyi|Anton Okolnychyi]] · [[people/yufei-gu|Yufei Gu]] · [[people/shawn-chang|Shawn Chang]] · [[people/steven-wu|Steven Wu]] · [[people/russell-spitzer|Russell Spitzer]] · [[people/amogh-jahagirdar|Amogh Jahagirdar]] · [[people/peter-vary|Péter Váry]] · [[people/holden-karau|Holden Karau]] · [[people/kevin-liu|Kevin Liu]] · [[people/steve-loughran|Steve Loughran]] · [[people/sung-yun|Sung Yun]] · [[people/jean-baptiste-onofre|Jean-Baptiste Onofré]] · [[episodes/2026-04-16|2026-04-16]]
