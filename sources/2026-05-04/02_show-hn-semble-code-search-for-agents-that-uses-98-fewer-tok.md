---
type: story
story_id: hn_47997629
episode_date: 2026-05-04
rank: 2
source: hacker_news
url: "https://github.com/MinishLab/semble"
title: Show HN Semble Code search for agents that uses 98 fewer tokens than grep
quality_score: 0.654
content_hash: "sha256:6f9a77275136a16cf7543bd264994f7d205373f613c3982a66ca064cc1313fec"
concepts: [model2vec, bm25, reciprocal-rank-fusion, mcp-server, potion-code-16m, ndcg, static-embeddings, semble]
companies: [minishlab, anthropic, cursor, hugging-face]
people: [stephan, thomas]
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-04 10:20:10.998000"
tags: [story, source/hacker-news]
---

## Summary
Semble is an open-source code search tool built by Stephan and Thomas of MinishLab, designed to help AI coding agents find relevant code without falling back to token-expensive grep or full-file reads. It combines static Model2Vec embeddings (potion-code-16M), BM25 retrieval, Reciprocal Rank Fusion, and code-aware reranking, running entirely on CPU with no API keys or GPU required. On a benchmark of 1,250 query/document pairs across 63 repositories and 19 languages, Semble uses 98% fewer tokens than grep-based approaches and achieves 99% of the retrieval quality of a 137M-parameter transformer model. It ships as an MCP server compatible with Claude Code, Cursor, Codex, and OpenCode, and can index a typical repository in about 250ms with query latency of 1.5ms.

## Key claims
- Semble uses 98% fewer tokens than grep-based code reading approaches.
- It achieves 99% of the retrieval quality of a 137M-parameter code-trained transformer model.
- Semble indexes a typical repository in approximately 250ms and answers queries in 1.5ms on CPU.
- The tool requires no API keys, no GPU, and no external services.
- It combines Model2Vec static embeddings, BM25, Reciprocal Rank Fusion, and code-aware reranking.
- Benchmarks cover 1,250 query/document pairs across 63 repositories and 19 programming languages.
- Semble ships as an MCP server compatible with Claude Code, Cursor, Codex, and OpenCode.

## Source
- **Origin:** hacker_news
- **URL:** <https://github.com/MinishLab/semble>

## Related
[[concepts/model2vec|model2vec]] · [[concepts/bm25|bm25]] · [[concepts/reciprocal-rank-fusion|reciprocal-rank-fusion]] · [[concepts/mcp-server|mcp-server]] · [[concepts/potion-code-16m|potion-code-16m]] · [[concepts/ndcg|ndcg]] · [[concepts/static-embeddings|static-embeddings]] · [[concepts/semble|semble]] · [[concepts/claude-code|claude-code]] · [[concepts/cursor|cursor]] · [[concepts/codex|codex]] · [[concepts/api|api]] · [[concepts/mcp|mcp]] · [[companies/minishlab|MinishLab]] · [[companies/anthropic|Anthropic]] · [[companies/cursor|Cursor]] · [[companies/hugging-face|Hugging Face]] · [[people/stephan|Stephan]] · [[people/thomas|Thomas]] · [[episodes/2026-05-04|2026-05-04]]
