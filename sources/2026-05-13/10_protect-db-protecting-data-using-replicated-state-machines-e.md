---
type: story
story_id: rss_25fdf80a5863
episode_date: 2026-05-13
rank: 10
source: rss_feed
url: "https://arxiv.org/abs/2605.11953"
title: PROTECT-DB Protecting Data using Replicated State Machines Efficient Corruption Detection Recovery
quality_score: 0.756
content_hash: "sha256:3abd803e4100e9286640ea3912f8ec182e9de1e7b67a8a985296a8a45dd1fd65"
concepts: [byzantine-fault-tolerant-replicated-state-machine, postgresql, blockchain, deterministic-database-execution, corruption-detection, shared-log]
companies: []
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-13 10:23:01.854000"
tags: [story, source/rss-feed]
---

## Summary
The paper PROTECT-DB proposes a system for protecting database integrity against Byzantine attacks using Byzantine-fault tolerant (BFT) replicated state machines built on a deterministic extension of PostgreSQL. Each replica deterministically executes transactions recorded in a shared blockchain-based log, ensuring consistency across nodes. The system is designed for efficient and rapid detection of data corruption as well as concurrent repair during normal transaction execution. A performance study is presented to demonstrate the practicality and efficiency of the approach. The authors argue this work establishes a foundation for practical BFT replicated state machine use in database systems.

## Key claims
- PROTECT-DB uses Byzantine-fault tolerant replicated state machines to protect databases against corruption attacks.
- The system is built on top of a deterministic extension of PostgreSQL.
- Each replica deterministically executes transactions recorded in a shared log blockchain.
- The design prioritizes efficient and quick detection of corruption concurrent with transaction execution.
- The system supports quick repair of corrupted state without halting transaction processing.
- A performance study demonstrates the efficiency and practicality of the proposed approach.
- The authors claim this work lays the foundation for practical BFT replicated state machine use in databases.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2605.11953>

## Related
[[concepts/byzantine-fault-tolerant-replicated-state-machine|byzantine-fault-tolerant-replicated-state-machine]] · [[concepts/postgresql|postgresql]] · [[concepts/blockchain|blockchain]] · [[concepts/deterministic-database-execution|deterministic-database-execution]] · [[concepts/corruption-detection|corruption-detection]] · [[episodes/2026-05-13|2026-05-13]]
