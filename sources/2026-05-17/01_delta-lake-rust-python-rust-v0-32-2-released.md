---
type: story
story_id: github_release_delta-io_delta-rs_323759919
episode_date: 2026-05-17
rank: 1
source: github_releases
url: "https://github.com/delta-io/delta-rs/releases/tag/rust-v0.32.2"
title: Delta Lake Rust Python rust-v0.32.2 released
quality_score: 0.771
content_hash: "sha256:e30f95d5dde0caab83b35d987a8591ffa319bc16ebd0f635a1f47d47c3d6dad7"
concepts: [delta-lake, delta-rs, dynamodb-locking, commitproperties, deltascan, delta-kernel]
companies: [delta-io]
people: [ethan-tyler, r-tyler]
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-17 10:19:26.750000"
tags: [story, source/github-releases]
---

## Summary
The delta-rs project released rust-v0.32.2 on 2026-05-15, a maintenance release for the Delta Lake Rust and Python library. The release closes several bug reports including a DynamoDB setup documentation issue, a MERGE regression causing higher memory usage in Python 1.5.1 compared to 1.5.0, and a crash on Linux kernels with 64KB page sizes. It also adds a feature to support passing non-string datatypes in custom metadata via CommitProperties from Python. Several pull requests were merged covering refactoring, documentation updates, bug fixes, and test consolidation.

## Key claims
- delta-rs rust-v0.32.2 was released on 2026-05-15.
- A regression in Python 1.5.1 caused MERGE operations with small source batches to use substantially more RSS memory than version 1.5.0.
- A bug was fixed where importing deltalake in Python crashed on Linux kernels with 64KB page sizes.
- The release adds support for passing non-string datatypes in custom _metadata within CommitProperties from Python.
- DynamoDB locking setup documentation was updated as part of this release.
- The release includes a refactor to deprecate the legacy DeltaScan codec surface.

## Source
- **Origin:** github_releases
- **URL:** <https://github.com/delta-io/delta-rs/releases/tag/rust-v0.32.2>

## Related
[[concepts/delta-lake|delta-lake]] · [[concepts/delta-rs|delta-rs]] · [[concepts/dynamodb-locking|dynamodb-locking]] · [[concepts/commitproperties|commitproperties]] · [[concepts/python|python]] · [[concepts/merge|merge]] · [[companies/delta-io|delta-io]] · [[people/ethan-tyler|Ethan Tyler]] · [[people/r-tyler|R Tyler]] · [[episodes/2026-05-17|2026-05-17]]
