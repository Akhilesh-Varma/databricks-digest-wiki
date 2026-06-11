---
type: story
story_id: hn_48248801
episode_date: 2026-05-24
rank: 2
source: hacker_news
url: "https://news.ycombinator.com/item?id=48248801"
title: Show HN I built a RAG and knowledge graph agent that runs locally
quality_score: 0.763
content_hash: "sha256:84880cac31d185d65a3269e21f9f594dade95aeb2e8b299fe6b8d4503772ec85"
concepts: [rag-retrieval-augmented-generation, knowledge-graph, local-llm, vector-store, docker-execution, vision-llm, ai-agent, homebrew]
companies: [anthropic, openai, cursor]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-24 14:08:01.617000"
tags: [story, source/hacker-news]
---

## Summary
Claw-Coder is a locally-running AI coding agent designed to address privacy and performance concerns associated with cloud-based coding assistants like Codex, Cursor, and Claude. It keeps all code, RAG indexes, and knowledge graph data on the user's machine, avoiding the need to share codebases with cloud providers. To compensate for the limited capabilities of small local LLMs, it equips them with a knowledge graph, a vector-store-backed RAG system, a web search tool, and Docker-based code execution across multiple languages. The Docker execution environment includes a vision LLM to evaluate rendered HTML/CSS output, allowing the agent to validate its own generated code. The project is currently closed-source and in testing, distributed via Homebrew.

## Key claims
- Claw-Coder runs entirely locally, keeping all code, RAG data, and knowledge graph information on the user's machine to preserve privacy.
- Cloud-based coding agents like Codex and Cursor send user codebases to cloud providers, which Claw-Coder aims to avoid.
- Small local LLMs (e.g., 8B, 13B parameter models) lack the capability of cloud models, so Claw-Coder compensates by providing them with specialized tools.
- A knowledge graph is used to represent relationships between code entities in a codebase, improving reasoning and coding performance of local LLMs.
- RAG with a vector store allows the agent to handle large codebases that would exceed the context window of local LLMs.
- Docker containers are used to execute and validate generated code across multiple languages, and a vision LLM evaluates rendered browser output for HTML/CSS.
- Claw-Coder is currently closed-source and distributed via Homebrew for testing and feedback.

## Source
- **Origin:** hacker_news
- **URL:** <https://news.ycombinator.com/item?id=48248801>

## Related
[[concepts/rag-retrieval-augmented-generation|rag-retrieval-augmented-generation]] · [[concepts/knowledge-graph|knowledge-graph]] · [[concepts/local-llm|local-llm]] · [[concepts/vector-store|vector-store]] · [[concepts/docker-execution|docker-execution]] · [[concepts/vision-llm|vision-llm]] · [[concepts/ai-agent|ai-agent]] · [[concepts/context-window|context-window]] · [[concepts/workspace|workspace]] · [[concepts/explain|explain]] · [[concepts/claude|claude]] · [[concepts/docker|docker]] · [[concepts/cursor|cursor]] · [[concepts/cloud|cloud]] · [[concepts/codex|codex]] · [[concepts/llms|llms]] · [[concepts/html|html]] · [[concepts/rag|rag]] · [[concepts/llm|llm]] · [[concepts/ai|ai]] · [[companies/anthropic|Anthropic]] · [[companies/openai|OpenAI]] · [[companies/cursor|Cursor]] · [[episodes/2026-05-24|2026-05-24]]
