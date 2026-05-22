---
type: story
story_id: rss_25576b9bedc7
episode_date: 2026-05-22
rank: 10
source: rss_feed
url: "https://arxiv.org/abs/2605.22811"
title: GS-QA A Benchmark for Geospatial Question Answering
quality_score: 0.836
content_hash: "sha256:dfd97294e318053dd5ae9524e6e69699519ad4817afe4401e5333afff679a812"
concepts: [gs-qa, geospatial-question-answering, large-language-models, retrieval-augmented-generation, text-to-sql, openstreetmap, spatial-database, gpt-4o, claude-sonnet, ministral-3]
companies: [openai, anthropic, mistral-ai, wikimedia-foundation]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-22 10:22:09.304000"
tags: [story, source/rss-feed]
---

## Summary
GS-QA is a new benchmark for evaluating geospatial question answering systems, comprising 2,800 question-answer pairs across 28 templates built on OpenStreetMap and Wikipedia data. It addresses limitations of prior benchmarks by covering a wide range of spatial predicates, answer types, and multi-source reasoning requirements. The benchmark includes a comprehensive evaluation methodology combining standard text-based QA measures with geospatial-specific metrics such as distance error and angular error. Nine LLM-based baselines were tested using GPT-4o, Claude Sonnet 4.6, and Ministral-3 with direct prompting, retrieval-augmented generation, and text-to-SQL approaches. Results show that while current LLMs handle simple spatial queries reasonably well, performance degrades significantly for complex predicates, numeric outputs, and multi-source reasoning.

## Key claims
- GS-QA contains 2,800 question-answer pairs across 28 templates derived from OpenStreetMap and Wikipedia data.
- The benchmark covers spatial predicates including directional and towards filtering, and answer types such as entity names, locations, distances, directions, counts, and aggregated areas/lengths.
- GS-QA requires multi-source reasoning by combining geospatial information from OpenStreetMap with factual information from Wikipedia.
- Evaluation methodology includes both text-based QA measures and geospatial-specific measures such as distance error and angular error.
- Nine LLM-based baselines were implemented using GPT-4o, Claude Sonnet 4.6, and Ministral-3 with combinations of direct prompting, retrieval-augmented generation, and text-to-SQL.
- Existing LLM solutions perform reasonably on simple spatial predicates with entity name outputs but degrade significantly for complex predicates, numeric outputs, and multi-source reasoning.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2605.22811>

## Related
[[concepts/gs-qa|gs-qa]] · [[concepts/geospatial-question-answering|geospatial-question-answering]] · [[concepts/large-language-models|large-language-models]] · [[concepts/retrieval-augmented-generation|retrieval-augmented-generation]] · [[concepts/text-to-sql|text-to-sql]] · [[concepts/openstreetmap|openstreetmap]] · [[concepts/llms|llms]] · [[concepts/sql|sql]] · [[concepts/llm|llm]] · [[companies/openai|OpenAI]] · [[companies/anthropic|Anthropic]] · [[companies/mistral-ai|Mistral AI]] · [[companies/wikimedia-foundation|Wikimedia Foundation]] · [[episodes/2026-05-22|2026-05-22]]
