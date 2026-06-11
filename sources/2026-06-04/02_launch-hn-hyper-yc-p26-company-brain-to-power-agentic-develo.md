---
type: story
story_id: hn_48387095
episode_date: 2026-06-04
rank: 2
source: hacker_news
url: "https://news.ycombinator.com/item?id=48387095"
title: Launch HN Hyper YC P26 Company brain to power agentic development
quality_score: 0.816
content_hash: "sha256:84e9afbfd8cc32870c43e684eb7c0e1b109766c4d0ac52c6342595176c287954"
concepts: [knowledge-graph, model-context-protocol-mcp, retrieval-augmented-generation, reciprocal-rank-fusion, semantic-search, second-brain, agentic-ai, postgres-full-text-search, webhook, obsidian, roam-research, notion, anki, claude-code, cursor, codex, granola]
companies: [hyper, y-combinator, anthropic, openai]
people: [shalin, kanyes]
extractor_model: claude-sonnet-4-6
extracted_at: "2026-06-04 10:21:23.210000"
tags: [story, source/hacker-news]
---

## Summary
Hyper is a YC W26 startup building a 'shared company brain' that ingests information from tools like Slack, Docs, Email, and Calendar to improve AI agents and automations. The system synthesizes ingested data into a hybrid memory architecture combining a knowledge graph of subject-predicate-object facts with semantic embeddings and Postgres full-text search. Facts carry provenance, access-control tags, and timestamps for when they were introduced or invalidated, allowing the graph to stay current and handle contradictions gracefully. Agents interact with Hyper via lifecycle hooks in tools like Claude Code, Cursor, and Codex, as well as standard MCP tool calls. The founders, longtime friends Shalin and Kanyes, were inspired by the tools-for-thought movement and believe the main bottleneck for capable AI models is lack of company-specific context.

## Key claims
- Hyper ingests company information from Slack, Docs, Email, Calendar, and Granola and synthesizes it into a knowledge graph with semantic embeddings.
- The memory system uses a hybrid approach with two modalities: raw source 'Episodes' and extracted 'Facts' stored as subject-predicate-object records.
- Facts carry provenance back to their source and access-control tags, so two people on the same team can ask the same question and receive different answers.
- When a fact is contradicted, the new fact supersedes the old one but the old version is retained so users can audit how a decision was reached.
- Agents read and write to Hyper via lifecycle hooks in tools like Claude Code, Cowork, Codex, and Cursor, as well as plain MCP tool calls.
- Hyper is positioned as solving limitations of MCP, including session-scoped context loss, incomplete information gathering, and lack of meta-reasoning.
- Hyper is a YC P26 (W26) company offering a 3-day free trial.

## Source
- **Origin:** hacker_news
- **URL:** <https://news.ycombinator.com/item?id=48387095>

## Related
[[concepts/knowledge-graph|knowledge-graph]] · [[concepts/model-context-protocol-mcp|model-context-protocol-mcp]] · [[concepts/reciprocal-rank-fusion|reciprocal-rank-fusion]] · [[concepts/semantic-search|semantic-search]] · [[concepts/second-brain|second-brain]] · [[concepts/agentic-ai|agentic-ai]] · [[concepts/full-text-search|full-text-search]] · [[concepts/embeddings|embeddings]] · [[concepts/ai-agents|ai-agents]] · [[concepts/postgres|postgres]] · [[concepts/claude|claude]] · [[concepts/rest|rest]] · [[concepts/mcp|mcp]] · [[concepts/ai|ai]] · [[companies/hyper|Hyper]] · [[companies/y-combinator|Y Combinator]] · [[companies/anthropic|Anthropic]] · [[companies/openai|OpenAI]] · [[people/shalin|Shalin]] · [[people/kanyes|Kanyes]] · [[episodes/2026-06-04|2026-06-04]]
