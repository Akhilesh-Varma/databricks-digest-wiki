---
type: story
story_id: hn_48100227
episode_date: 2026-05-12
rank: 4
source: hacker_news
url: "https://github.com/Mnexa-AI/e2a"
title: Show HN E2a Open-source email gateway for AI agents
quality_score: 0.65
content_hash: "sha256:102bded35db60280307394459199bc0d7739a3a52e0f4b82a8eb37a7d7842a17"
concepts: [e2a, email-gateway, human-in-the-loop, websocket, webhook, spf, dkim, dmarc, postgresql, soc-2, hipaa]
companies: [mnexa-ai]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-12 10:21:07.399000"
tags: [story, source/hacker-news]
---

## Summary
Mnexa-AI has open-sourced E2a, a standalone email gateway designed specifically for AI agents. The project originated from an internal need to use email as a trigger within an agent system. Key features include consistent email and conversation threading, human-in-the-loop review for outbound emails, fast onboarding of agent email addresses, and both WebSocket and webhook delivery mechanisms. The project currently supports SPF/DKIM but lacks DMARC, scoped API keys, high availability, and compliance certifications like SOC 2 or HIPAA.

## Key claims
- E2a is an open-source email gateway built specifically to serve as an email trigger and interface for AI agents.
- The project was extracted from an internal agent system built by Mnexa-AI and released as a standalone service.
- E2a maintains consistent threading between email threads and agent conversation threads.
- The gateway supports human-in-the-loop review for outbound emails, particularly useful during testing.
- E2a supports WebSocket connections for local agents and at-least-once webhook delivery for cloud agents.
- Current authentication supports SPF and DKIM but not yet DMARC.
- Planned but not yet implemented features include scoped API keys, multi-region high availability, app-layer email encryption, and SOC 2/HIPAA compliance.

## Source
- **Origin:** hacker_news
- **URL:** <https://github.com/Mnexa-AI/e2a>

## Related
[[concepts/e2a|e2a]] · [[concepts/email-gateway|email-gateway]] · [[concepts/human-in-the-loop|human-in-the-loop]] · [[concepts/websocket|websocket]] · [[concepts/webhook|webhook]] · [[concepts/spf|spf]] · [[concepts/dkim|dkim]] · [[concepts/postgres|postgres]] · [[concepts/cloud|cloud]] · [[concepts/api|api]] · [[concepts/ai|ai]] · [[companies/mnexa-ai|Mnexa-AI]] · [[episodes/2026-05-12|2026-05-12]]
