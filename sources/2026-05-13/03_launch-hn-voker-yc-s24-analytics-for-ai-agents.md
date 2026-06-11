---
type: story
story_id: hn_48109962
episode_date: 2026-05-13
rank: 3
source: hacker_news
url: "https://voker.ai"
title: Launch HN Voker YC S24 Analytics for AI Agents
quality_score: 0.737
content_hash: "sha256:7b5ec1105f3146a717eaa35370d12df85bf22c0b4225d808935f707b62d2d89d"
concepts: [agent-analytics, hierarchical-text-classification, llm-observability, llm-evals, conversational-intelligence, sdk, product-analytics]
companies: [voker-ai, y-combinator, openai, anthropic, google]
people: [alex, tyler]
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-13 10:21:31.859000"
tags: [story, source/hacker-news]
---

## Summary
Voker.ai is a YC S24 analytics platform for AI agent products, co-founded by Alex and Tyler. It provides a lightweight, LLM-stack-agnostic SDK that wraps LLM calls to surface structured analytics about agent performance in production. The platform introduces three core primitives—Intents, Corrections, and Resolutions—to describe conversational agent interactions and uses hierarchical text classification to generate dynamic usage categories. Unlike observability tools or eval frameworks, Voker targets AI product teams rather than just engineers, giving higher-level trend insights without requiring manual log review. A free tier is available at 2,000 events per month, with paid plans starting at $80/month.

## Key claims
- 90% of surveyed YC founders said the only way they know their agents are failing users is by receiving customer complaints.
- Voker introduces three agent analytics primitives: Intents, Corrections, and Resolutions, applicable to most conversational agents.
- Voker uses hierarchical text classification and LLMs to create dynamic categories from annotated conversations, avoiding LLMs for core statistical calculations.
- The Voker SDK is LLM-stack agnostic and supports OpenAI, Anthropic, and Gemini in Python and TypeScript.
- Existing observability tools are engineer-focused and suited for individual trace debugging, while eval tools only test known issues and miss unexpected trends.
- A common workaround teams use is uploading observability logs to Claude or ChatGPT for summary insights, which produces inconsistent and inaccurate statistics.
- Voker offers a free tier of 2,000 events per month and paid plans starting at $80/month with a 30-day free trial.

## Source
- **Origin:** hacker_news
- **URL:** <https://voker.ai>

## Related
[[concepts/agent-analytics|agent-analytics]] · [[concepts/hierarchical-text-classification|hierarchical-text-classification]] · [[concepts/llm-observability|llm-observability]] · [[concepts/llm-evals|llm-evals]] · [[concepts/conversational-intelligence|conversational-intelligence]] · [[concepts/product-analytics|product-analytics]] · [[concepts/data-engineering|data-engineering]] · [[concepts/observability|observability]] · [[concepts/data-science|data-science]] · [[concepts/typescript|typescript]] · [[concepts/analytics|analytics]] · [[concepts/chatgpt|chatgpt]] · [[concepts/claude|claude]] · [[concepts/having|having]] · [[concepts/python|python]] · [[concepts/llms|llms]] · [[concepts/llm|llm]] · [[concepts/ai|ai]] · [[companies/voker-ai|Voker.ai]] · [[companies/y-combinator|Y Combinator]] · [[companies/openai|OpenAI]] · [[companies/anthropic|Anthropic]] · [[companies/google|Google]] · [[people/alex|Alex]] · [[people/tyler|Tyler]] · [[episodes/2026-05-13|2026-05-13]]
