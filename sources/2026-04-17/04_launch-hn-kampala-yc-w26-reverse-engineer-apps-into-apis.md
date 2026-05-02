---
type: story
story_id: hn_47794514
episode_date: 2026-04-17
rank: 4
source: hacker_news
url: "https://www.zatanna.ai/kampala"
title: Launch HN Kampala YC W26 Reverse-Engineer Apps into APIs
quality_score: 0.741
content_hash: "sha256:e63b16c76ea91dd5a77bcbe618f204c994fe244fabec8d8eba490667d8f6f6a5"
concepts: [man-in-the-middle-proxy, model-context-protocol-mcp, browser-automation, tls-fingerprinting, http2-fingerprinting, computer-use-agents, anti-bot-detection, session-token-reuse, workflow-replay, yardi]
companies: [zatanna, y-combinator]
people: [alex, tarun]
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:08:59.782000"
tags: [story, source/hacker-news]
---

## Summary
Kampala, built by Alex and Tarun under their company Zatanna, is a man-in-the-middle (MITM) proxy tool that reverse-engineers existing web, mobile, and desktop application workflows into reusable APIs and scripts. Unlike browser automation or computer-use agents, Kampala operates at the HTTP request layer, leveraging existing session tokens and anti-bot cookies to automate workflows deterministically. The tool addresses shortcomings of existing MITM proxies, including TLS/HTTP2 fingerprint manipulation and poor MCP implementations. Users can either use an agent harness that auto-generates scripts via prompting or manually record a workflow once and use an MCP-compatible coding agent to replicate it. The founders originally built the tooling while working in dental tech to integrate with insurance payer dashboards and legacy practice management systems.

## Key claims
- Kampala is a MITM-style proxy that reverse-engineers app workflows into APIs without browser automation or computer-use agents.
- It works across websites, mobile apps, and desktop apps by operating at the HTTP request layer.
- Existing MITM tools failed due to TLS/HTTP2 fingerprint manipulation detectable by anti-bot systems and poor MCP feature exposure.
- Kampala leverages existing session tokens and anti-bot cookies to automate workflows deterministically in seconds.
- Users can generate scripts via an agent harness or by manually performing a workflow once and prompting a coding agent via MCP.
- The tool was originally developed internally at Zatanna while building integrations for dental insurance payer dashboards and legacy dental practice systems.
- Kampala can host generated scripts/APIs on behalf of users or allow export and self-hosting.

## Source
- **Origin:** hacker_news
- **URL:** <https://www.zatanna.ai/kampala>

## Related
[[concepts/man-in-the-middle-proxy|man-in-the-middle-proxy]] · [[concepts/model-context-protocol-mcp|model-context-protocol-mcp]] · [[concepts/browser-automation|browser-automation]] · [[concepts/tls-fingerprinting|tls-fingerprinting]] · [[concepts/http2-fingerprinting|http2-fingerprinting]] · [[concepts/computer-use-agents|computer-use-agents]] · [[concepts/anti-bot-detection|anti-bot-detection]] · [[concepts/session-token-reuse|session-token-reuse]] · [[concepts/workflow-replay|workflow-replay]] · [[concepts/workflows|workflows]] · [[concepts/llms|llms]] · [[concepts/api|api]] · [[concepts/ai|ai]] · [[companies/zatanna|Zatanna]] · [[companies/y-combinator|Y Combinator]] · [[people/alex|Alex]] · [[people/tarun|Tarun]] · [[episodes/2026-04-17|2026-04-17]]
