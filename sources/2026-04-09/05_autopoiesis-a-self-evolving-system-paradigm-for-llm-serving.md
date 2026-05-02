---
type: story
story_id: rss_5b60a8969c46
episode_date: 2026-04-09
rank: 5
source: rss_feed
url: "https://arxiv.org/abs/2604.07144"
title: Autopoiesis A Self-Evolving System Paradigm for LLM Serving Under Runtime Dynamics
quality_score: 0.916
content_hash: "sha256:92ab14ae3c00e453c1c35eae77ab642caaa03743a1a82b661e5a9a3375bac798"
concepts: [autopoiesis, llm-serving, program-synthesis, online-policy-evolution, cluster-autoscaling, scheduling-algorithms, large-language-models]
companies: []
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:31:29.415000"
tags: [story, source/rss-feed]
---

## Summary
Autopoiesis is a novel self-evolving system paradigm for Large Language Model serving that addresses the limitations of static, human-engineered serving policies in volatile runtime environments. The system introduces an LLM-driven program synthesis workflow that continuously rewrites serving policy code in response to real-time observed dynamics such as workload fluctuations and elastic cluster autoscaling. Rather than deploying fixed scheduling and rescheduling strategies, Autopoiesis treats policy design as an ongoing system component that autonomously adapts to shifting runtime trade-offs. Evaluations across diverse runtime dynamics show up to 53% and on average 34% improvements over state-of-the-art LLM serving systems.

## Key claims
- Traditional LLM serving systems rely on static, human-engineered policies that cannot adapt to continuously shifting runtime trade-offs.
- Autopoiesis introduces an LLM-driven program synthesis workflow that evolves serving policies based on real-time observed system dynamics.
- The system enables continuous online policy evolution during serving, transforming policy design from a one-time offline task into an ongoing component.
- Autopoiesis treats serving policies as living code that LLMs continuously rewrite throughout deployment rather than static pre-deployment artifacts.
- Evaluation shows Autopoiesis achieves up to 53% and on average 34% improvements over state-of-the-art LLM serving systems across diverse runtime dynamics.
- Key runtime trade-offs addressed include scheduling overhead vs. execution efficiency and rescheduling frequency vs. reconfiguration overhead.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2604.07144>

## Related
[[concepts/autopoiesis|autopoiesis]] · [[concepts/llm-serving|llm-serving]] · [[concepts/program-synthesis|program-synthesis]] · [[concepts/online-policy-evolution|online-policy-evolution]] · [[concepts/large-language-models|large-language-models]] · [[concepts/large-language-model|large-language-model]] · [[concepts/language-model|language-model]] · [[concepts/llms|llms]] · [[concepts/llm|llm]] · [[episodes/2026-04-09|2026-04-09]]
