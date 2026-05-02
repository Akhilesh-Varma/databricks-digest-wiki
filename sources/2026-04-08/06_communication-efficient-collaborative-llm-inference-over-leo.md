---
type: story
story_id: rss_be13f140be7e
episode_date: 2026-04-08
rank: 6
source: rss_feed
url: "https://arxiv.org/abs/2604.04654"
title: Communication-Efficient Collaborative LLM Inference over LEO Satellite Networks
quality_score: 0.897
content_hash: "sha256:3913eb5765ed2a3953d4e2ea54bd6539c026fdcd6da4c84d82ad49c4ac5c1314"
concepts: [large-language-models-llms, leo-satellite-networks, collaborative-llm-inference, pipeline-parallelism, model-splitting, activation-compression, directed-acyclic-graph, a-search-algorithm, intermediate-activation-transmission]
companies: []
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:33:45.105000"
tags: [story, source/rss-feed]
---

## Summary
This paper proposes a communication-efficient collaborative LLM inference scheme designed for Low Earth Orbit (LEO) satellite networks, where limited onboard memory and high inference latency make single-satellite LLM deployment impractical. The approach splits a full LLM into sub-models distributed across multiple satellites, enabling collaborative inference by exchanging intermediate activations. Pipeline parallelism is used to overlap sub-model computation with activation transmission, reducing overall latency. An adaptive activation compression scheme mitigates cumulative errors from multi-stage model splitting. The optimization problem is formulated as a shortest-path search over a directed acyclic graph and solved with a modified A* algorithm, achieving up to 42% inference delay reduction and 71% communication overhead reduction with less than 1% accuracy loss.

## Key claims
- Limited onboard memory and excessive inference delay prevent practical deployment of LLMs on a single LEO satellite.
- The proposed scheme splits an LLM into multiple sub-models, each deployed on a separate satellite, enabling collaborative inference via intermediate activation exchange.
- Pipeline parallelism is leveraged to overlap sub-model inference with intermediate activation transmission, reducing end-to-end LLM inference delay.
- An adaptive activation compression scheme is designed to mitigate cumulative errors introduced by multi-stage model splitting while preserving inference accuracy.
- The inference delay minimization problem is transformed into a shortest-path search over a directed acyclic graph and solved using a modified A* algorithm.
- The proposed solution reduces inference delay by up to 42% and communication overhead by up to 71% compared to state-of-the-art benchmarks, with less than 1% accuracy loss.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2604.04654>

## Related
[[concepts/large-language-models-llms|large-language-models-llms]] · [[concepts/leo-satellite-networks|leo-satellite-networks]] · [[concepts/collaborative-llm-inference|collaborative-llm-inference]] · [[concepts/pipeline-parallelism|pipeline-parallelism]] · [[concepts/model-splitting|model-splitting]] · [[concepts/activation-compression|activation-compression]] · [[concepts/directed-acyclic-graph|directed-acyclic-graph]] · [[concepts/a-search-algorithm|a-search-algorithm]] · [[concepts/intermediate-activation-transmission|intermediate-activation-transmission]] · [[concepts/artificial-intelligence|artificial-intelligence]] · [[concepts/large-language-models|large-language-models]] · [[concepts/llm-inference|llm-inference]] · [[concepts/pipeline|pipeline]] · [[concepts/llms|llms]] · [[concepts/llm|llm]] · [[episodes/2026-04-08|2026-04-08]]
