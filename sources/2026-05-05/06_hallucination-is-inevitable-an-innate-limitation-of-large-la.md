---
type: story
story_id: hn_48010033
episode_date: 2026-05-05
rank: 6
source: hacker_news
url: "https://arxiv.org/abs/2401.11817"
title: Hallucination Is Inevitable An Innate Limitation of Large Language Models
quality_score: 0.695
content_hash: "sha256:237880f6723454f774abda35bed58c152bf0302794d76fec83b2e6f7245c837b"
concepts: [large-language-models, hallucination-in-llms, learning-theory, computable-functions, time-complexity, hallucination-mitigation]
companies: [arxiv]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-05 10:21:38.911000"
tags: [story, source/hacker-news]
---

## Summary
This paper presents a formal theoretical argument that hallucination in large language models (LLMs) is not merely a practical limitation but an innate and unavoidable one. The authors define hallucination as inconsistencies between a computable LLM and a computable ground truth function, then use results from learning theory to prove that LLMs cannot learn all computable functions. Because the formal world they define is a subset of the real world, hallucinations are therefore also inevitable in real-world LLM deployments. The paper further characterizes hallucination-prone tasks under provable time complexity constraints and discusses the implications for existing mitigation strategies and safe LLM deployment.

## Key claims
- Hallucination in LLMs is formally proven to be impossible to completely eliminate.
- The authors define hallucination as inconsistencies between a computable LLM and a computable ground truth function.
- Using learning theory, the paper shows LLMs cannot learn all computable functions and will inevitably hallucinate when used as general problem solvers.
- Because the formal world is a subset of the real world, hallucinations are also inevitable for real-world LLMs.
- For real-world LLMs constrained by provable time complexity, specific hallucination-prone tasks can be identified and empirically validated.
- The formal framework is used to analyze the mechanisms and efficacy of existing hallucination mitigation approaches.

## Source
- **Origin:** hacker_news
- **URL:** <https://arxiv.org/abs/2401.11817>

## Related
[[concepts/large-language-models|large-language-models]] · [[concepts/hallucination-in-llms|hallucination-in-llms]] · [[concepts/learning-theory|learning-theory]] · [[concepts/computable-functions|computable-functions]] · [[concepts/hallucination-mitigation|hallucination-mitigation]] · [[concepts/llms|llms]] · [[concepts/html|html]] · [[concepts/llm|llm]] · [[companies/arxiv|arXiv]] · [[episodes/2026-05-05|2026-05-05]]
