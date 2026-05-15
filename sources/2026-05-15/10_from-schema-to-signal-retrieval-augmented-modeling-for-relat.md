---
type: story
story_id: rss_a78eea866fd0
episode_date: 2026-05-15
rank: 10
source: rss_feed
url: "https://arxiv.org/abs/2605.14464"
title: From Schema to Signal Retrieval-Augmented Modeling for Relational Data Analytics
quality_score: 0.756
content_hash: "sha256:2933d4a8224a040623e4c62de722fa24fe1fc96943363eb1525b5e641574b741"
concepts: [retrieval-augmented-modeling-ram, relational-database-management-system-rdbms, graph-neural-networks, contrastive-learning, random-walks, information-retrieval, intra-table-retrieval-augmentation-atra, extra-table-retrieval-augmentation-etra, deep-neural-networks, representation-learning]
companies: []
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-15 10:22:34.669000"
tags: [story, source/rss-feed]
---

## Summary
This paper introduces Retrieval-Augmented Modeling (RAM), a framework designed to improve deep learning on relational databases stored in RDBMS. Unlike existing methods that rely solely on schema-defined graphs, RAM treats tuple attributes as tokens and uses random walks to build contextual documents, enabling information retrieval techniques to capture semantic relevance between tuples. The framework introduces two retrieval-based augmentations—ATRA for intra-table contrastive learning and ETRA for cross-table semantic linking—alongside a layer-wise architecture for representation learning. Experiments on five real-world relational databases show RAM consistently outperforms existing baselines across diverse prediction tasks.

## Key claims
- RAM combines graph structure with attribute semantics to address limitations of schema-defined graph approaches for relational data analytics.
- Tuple attributes are treated as tokens and random walks are used to construct contextual documents for information retrieval.
- ATRA leverages intra-table semantic relevance for contrastive learning to improve tuple representations.
- ETRA links semantically related tuples across tables to enhance graph connectivity beyond schema-defined edges.
- RAM uses a layer-wise architecture comprising attribute embedding, feature integration, and graph aggregation layers.
- Experiments on five real-world relational databases demonstrate RAM achieves state-of-the-art performance on diverse prediction tasks.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2605.14464>

## Related
[[concepts/retrieval-augmented-modeling-ram|retrieval-augmented-modeling-ram]] · [[concepts/relational-database-management-system-rdbms|relational-database-management-system-rdbms]] · [[concepts/graph-neural-networks|graph-neural-networks]] · [[concepts/contrastive-learning|contrastive-learning]] · [[concepts/random-walks|random-walks]] · [[concepts/information-retrieval|information-retrieval]] · [[concepts/intra-table-retrieval-augmentation-atra|intra-table-retrieval-augmentation-atra]] · [[concepts/extra-table-retrieval-augmentation-etra|extra-table-retrieval-augmentation-etra]] · [[concepts/relational-databases|relational-databases]] · [[concepts/data-analytics|data-analytics]] · [[concepts/analytics|analytics]] · [[concepts/schema|schema]] · [[episodes/2026-05-15|2026-05-15]]
