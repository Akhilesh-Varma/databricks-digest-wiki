---
type: story
story_id: hn_48169874
episode_date: 2026-05-18
rank: 3
source: hacker_news
url: "https://github.com/MinishLab/semble"
title: Show HN Semble Code search for agents that uses 98 fewer tokens than grep
quality_score: 0.761
content_hash: "sha256:b19e21b5d9bc5a32a86f0da67bd935d89ec54d78e393f9e0be2623b8bbbb0654"
concepts: [semble, model2vec, potion-code-16m, bm25, reciprocal-rank-fusion, mcp-server, ndcg, claude-code, static-embeddings]
companies: [minishlab, anthropic, cursor, openai, hugging-face]
people: [stephan, thomas]
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-18 10:19:25.037000"
tags: [story, source/hacker-news]
---

## Summary
Semble is an open-source code search tool designed for AI coding agents that combines static Model2Vec embeddings with BM25, fused via Reciprocal Rank Fusion (RRF) and reranked with code-aware signals. It was built by Stephan and Thomas of MinishLab to address the token-heavy fallback behavior of agents like Claude Code when searching large codebases. Semble runs entirely on CPU with no API keys or GPU required, indexing a typical repo in 250ms and querying in 1.5ms. On a benchmark of 1,250 query/document pairs across 63 repos and 19 languages, it uses 98% fewer tokens than grep-based approaches while achieving 99% of the retrieval quality of a 137M-parameter transformer model. It ships as an MCP server compatible with Claude Code, Cursor, Codex, and OpenCode.

## Key claims
- Semble uses 98% fewer tokens than grep-based code reading for AI agent code search.
- Semble achieves 0.854 NDCG@10, representing 99% of the retrieval quality of a 137M-parameter code-trained transformer.
- Semble indexes a typical repository in approximately 250ms and answers queries in 1.5ms on CPU.
- The tool requires no API keys, no GPU, and no external services, running entirely on CPU.
- Semble combines Model2Vec static embeddings (potion-code-16M) with BM25, fused via RRF and reranked with code-aware signals.
- Semble is available as an MCP server drop-in for Claude Code, Cursor, Codex, and OpenCode.
- The benchmark covers 1,250 query/document pairs across 63 repositories and 19 programming languages.

## Source
- **Origin:** hacker_news
- **URL:** <https://github.com/MinishLab/semble>

## Related
[[concepts/semble|semble]] · [[concepts/model2vec|model2vec]] · [[concepts/potion-code-16m|potion-code-16m]] · [[concepts/bm25|bm25]] · [[concepts/reciprocal-rank-fusion|reciprocal-rank-fusion]] · [[concepts/mcp-server|mcp-server]] · [[concepts/ndcg|ndcg]] · [[concepts/claude-code|claude-code]] · [[concepts/static-embeddings|static-embeddings]] · [[concepts/embeddings|embeddings]] · [[concepts/claude|claude]] · [[concepts/cursor|cursor]] · [[concepts/codex|codex]] · [[concepts/api|api]] · [[concepts/mcp|mcp]] · [[companies/minishlab|MinishLab]] · [[companies/anthropic|Anthropic]] · [[companies/cursor|Cursor]] · [[companies/openai|OpenAI]] · [[companies/hugging-face|Hugging Face]] · [[people/stephan|Stephan]] · [[people/thomas|Thomas]] · [[episodes/2026-05-18|2026-05-18]]
