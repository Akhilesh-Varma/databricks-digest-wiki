---
type: story
story_id: hn_48144670
episode_date: 2026-05-15
rank: 4
source: hacker_news
url: "https://github.com/GlycemicGPT/GlycemicGPT"
title: Show HN GlycemicGPT Open-source AI-powered diabetes management
quality_score: 0.818
content_hash: "sha256:f691bda00e21a4f4c3451e0bd8bfa23944379352ef205b88b2f1d0263b7cff35"
concepts: [glycemicgpt, nightscout, retrieval-augmented-generation-rag, ollama, continuous-glucose-monitor, bluetooth-low-energy-ble, fastapi, next-js, jetpack-compose, wear-os, docker, kubernetes, gpl-3-0]
companies: [dexcom, tandem-diabetes-care, anthropic, openai]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-15 10:21:15.569000"
tags: [story, source/hacker-news]
---

## Summary
GlycemicGPT is an open-source, self-hosted AI-powered diabetes management platform created by a Type 1 diabetic software engineer who lacked clinical oversight between endocrinologist appointments. It connects continuous glucose monitors, insulin pumps, and Nightscout instances to an AI analysis layer running entirely on the user's own infrastructure. The platform provides daily summaries, meal response analysis, conversational chat with RAG-backed clinical knowledge, and predictive alerting, but explicitly does not control insulin delivery or act as a closed-loop system. Users can run AI inference locally via Ollama or connect to hosted providers like Claude or OpenAI, with no data routed through any centralized project service. The project is licensed under GPL-3.0 and is seeking contributors, especially those with BLE and Android experience.

## Key claims
- GlycemicGPT is a self-hosted, open-source platform licensed under GPL-3.0 with no subscriptions or vendor lock-in.
- The platform supports Dexcom G7 via cloud API, Tandem t:slim X2 and Mobi pumps via direct BLE, and existing Nightscout instances.
- The AI layer provides daily briefs, meal response analysis, conversational chat with RAG-backed clinical knowledge, and predictive alerting with caregiver escalation.
- GlycemicGPT is explicitly a monitoring and analysis tool only — it does not deliver insulin or control pumps.
- Users can run AI inference fully locally using Ollama or connect to hosted providers such as Claude or OpenAI.
- The stack includes FastAPI, PostgreSQL 16, Redis 7, Next.js 15, React 19, and a Kotlin-based Android app with Wear OS support.
- The project includes a sandboxed Plugin SDK with Kotlin interfaces to allow contributors to add support for new devices.

## Source
- **Origin:** hacker_news
- **URL:** <https://github.com/GlycemicGPT/GlycemicGPT>

## Related
[[concepts/glycemicgpt|glycemicgpt]] · [[concepts/nightscout|nightscout]] · [[concepts/retrieval-augmented-generation-rag|retrieval-augmented-generation-rag]] · [[concepts/ollama|ollama]] · [[concepts/continuous-glucose-monitor|continuous-glucose-monitor]] · [[concepts/bluetooth-low-energy-ble|bluetooth-low-energy-ble]] · [[concepts/typescript|typescript]] · [[concepts/postgresql|postgresql]] · [[concepts/tailwind|tailwind]] · [[concepts/python|python]] · [[concepts/cloud|cloud]] · [[concepts/redis|redis]] · [[concepts/react|react]] · [[concepts/sdk|sdk]] · [[concepts/api|api]] · [[concepts/rag|rag]] · [[concepts/ai|ai]] · [[companies/dexcom|Dexcom]] · [[companies/tandem-diabetes-care|Tandem Diabetes Care]] · [[companies/anthropic|Anthropic]] · [[companies/openai|OpenAI]] · [[episodes/2026-05-15|2026-05-15]]
