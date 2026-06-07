---
type: story
story_id: devto_3839392
episode_date: 2026-06-07
rank: 7
source: devto
url: "https://dev.to/hajirufai/i-built-a-mini-columnar-storage-engine-in-pure-python-and-finally-understood-why-parquet-is-so-l70"
title: I built a mini columnar storage engine in pure Python and finally understood why Parquet is so fast
quality_score: 0.778
content_hash: "sha256:57075e52b39b78ffca3374b9fa52ef9cd56f964af964f9a791287d921c9fa77b"
concepts: [parquet, columnar-storage, apache-arrow, dictionary-encoding, run-length-encoding, delta-encoding, row-store, bit-packing]
companies: []
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-06-07 10:19:29.771000"
tags: [story, source/devto]
---

## Summary
The author describes building a minimal columnar storage engine in pure Python after experiencing a slow 40-second reporting query that read 90 columns when only 3 were needed. Through this weekend project, they explored the core ideas behind Parquet and Apache Arrow: storing data column-by-column on disk, writing a footer at the end of the file to enable random column access, and applying per-column encodings such as dictionary encoding, run-length encoding, and delta encoding. The article explains how each encoding targets a specific data pattern to reduce storage size before any general-purpose compression is applied. The author concludes that columnar storage's speed comes from the combination of reading only relevant columns and exploiting type homogeneity within columns for cheap, effective compression.

## Key claims
- A row store forces reading all columns even when a query touches only a few, wasting I/O on irrelevant bytes.
- Columnar storage places each column's values contiguously on disk, allowing queries to read only the needed columns.
- The footer-at-the-end pattern used in Parquet lets a reader seek directly to column locations without scanning the entire file.
- Dictionary encoding converts low-cardinality string columns into compact integer codes plus a small dictionary, dramatically reducing storage.
- Run-length encoding compresses sorted or repetitive column data into (value, count) pairs, making time-partitioned data compress extremely well.
- Delta encoding stores differences between consecutive monotonic integers rather than absolute values, keeping numbers small for further bit-packing.
- Each column independently selects its best encoding, which is why a single Parquet file can mix encoding strategies across columns.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/hajirufai/i-built-a-mini-columnar-storage-engine-in-pure-python-and-finally-understood-why-parquet-is-so-l70>

## Related
[[concepts/parquet|parquet]] · [[concepts/columnar-storage|columnar-storage]] · [[concepts/apache-arrow|apache-arrow]] · [[concepts/dictionary-encoding|dictionary-encoding]] · [[concepts/run-length-encoding|run-length-encoding]] · [[concepts/delta-encoding|delta-encoding]] · [[concepts/row-store|row-store]] · [[concepts/streaming|streaming]] · [[concepts/metadata|metadata]] · [[concepts/pyarrow|pyarrow]] · [[concepts/pandas|pandas]] · [[concepts/python|python]] · [[concepts/delta|delta]] · [[concepts/rest|rest]] · [[episodes/2026-06-07|2026-06-07]]
