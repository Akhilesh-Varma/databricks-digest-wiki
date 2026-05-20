---
type: story
story_id: hn_48192383
episode_date: 2026-05-20
rank: 4
source: hacker_news
url: "https://github.com/antoinezambelli/forge"
title: Show HN Forge Guardrails take an 8B model from 53 to 99 on agentic tasks
quality_score: 0.892
content_hash: "sha256:3f0e3ba5279438af60ece2a15ebba8e6c01cc19fa03ffe90642f175808347f9a"
concepts: [forge, llm-tool-calling, agentic-workflows, guardrails, retry-nudges, toolresolutionerror, context-compaction, vram-aware-context-management, ollama, llamafile, llama-server, mcnemar-s-test, ministral-8b, mistral-nemo-12b]
companies: [texas-instruments, anthropic, acm, mistral-ai]
people: [antoine-zambelli]
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-20 10:22:11.419000"
tags: [story, source/hacker-news]
---

## Summary
Antoine Zambelli, AI Director at Texas Instruments, built Forge, an open-source reliability layer for self-hosted LLM tool-calling on consumer hardware. Forge adds domain-agnostic guardrails—retry nudges, step enforcement, error recovery, and VRAM-aware context management—around local models without modifying the models themselves. The system improves an 8B model's performance on multi-step agentic workflows from 53% to 99.3%, narrowing the gap with frontier APIs like Claude Sonnet to under one percentage point. A key finding is that the serving backend alone can cause a 75-point accuracy swing with identical model weights, and that error recovery scores zero for all models tested without an explicit retry mechanism. The paper has been accepted to ACM CAIS 2026.

## Key claims
- Forge improves a Ministral 8B model from 53% to 99.3% on multi-step agentic workflows without changing the model weights.
- A local 8B model with Forge (99.3%) outperforms Claude Sonnet without guardrails (87.2%), beating frontier API results.
- Error recovery scores 0% for every model tested—local and frontier—without an explicit retry mechanism, indicating an architectural absence rather than a capability gap.
- The same Mistral-Nemo 12B weights produce 7% accuracy on llama-server with native function calling versus 83% on Llamafile in prompt mode—a 75-point swing from infrastructure alone.
- Retry nudges account for 24–49 point accuracy drops when disabled, making them the highest-impact guardrail layer per ablation study.
- Ollama and Llamafile silently fall back to CPU when VRAM is exceeded; Forge queries nvidia-smi at startup to derive a token budget preventing this.
- Forge introduces a new ToolResolutionError exception class to distinguish between a tool returning data and a tool finding nothing, preventing silent bad-data propagation.

## Source
- **Origin:** hacker_news
- **URL:** <https://github.com/antoinezambelli/forge>

## Related
[[concepts/forge|forge]] · [[concepts/llm-tool-calling|llm-tool-calling]] · [[concepts/agentic-workflows|agentic-workflows]] · [[concepts/guardrails|guardrails]] · [[concepts/retry-nudges|retry-nudges]] · [[concepts/toolresolutionerror|toolresolutionerror]] · [[concepts/context-compaction|context-compaction]] · [[concepts/vram-aware-context-management|vram-aware-context-management]] · [[concepts/ollama|ollama]] · [[concepts/llamafile|llamafile]] · [[concepts/ministral-8b|ministral-8b]] · [[concepts/mistral-nemo-12b|mistral-nemo-12b]] · [[concepts/workflows|workflows]] · [[concepts/optimize|optimize]] · [[concepts/api|api]] · [[concepts/llm|llm]] · [[concepts/ai|ai]] · [[companies/texas-instruments|Texas Instruments]] · [[companies/anthropic|Anthropic]] · [[companies/acm|ACM]] · [[companies/mistral-ai|Mistral AI]] · [[people/antoine-zambelli|Antoine Zambelli]] · [[episodes/2026-05-20|2026-05-20]]
