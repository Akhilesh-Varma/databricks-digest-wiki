---
type: story
story_id: rss_6818bda45f3d
episode_date: 2026-04-10
rank: 6
source: rss_feed
url: "https://arxiv.org/abs/2604.07609"
title: Blink CPU-Free LLM Inference by Delegating the Serving Stack to GPU and SmartNIC
quality_score: 0.876
content_hash: "sha256:46c72dab4293869e268d125b2168edcf6f68b534edd67882b2c1f987d34a2552"
concepts: [blink, llm-inference, smartnic, rdma, kv-cache-management, persistent-gpu-kernel, tensorrt-llm, vllm, sglang, cpu-free-inference]
companies: []
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:29:08.539000"
tags: [story, source/rss-feed]
---

## Summary
Blink is a new end-to-end LLM inference serving architecture that removes the host CPU from the steady-state inference path by redistributing work to a SmartNIC and a GPU. The SmartNIC handles request ingestion and delivers inputs directly into GPU memory via RDMA, while a persistent GPU kernel manages batching, scheduling, and KV-cache without CPU involvement. Benchmarked against TensorRT-LLM, vLLM, and SGLang, Blink reduces P99 TTFT by up to 8.47x, P99 TPOT by up to 3.40x, and energy per token by up to 48.6%. Under CPU interference conditions where existing systems degrade by up to two orders of magnitude, Blink maintains stable performance, enabling better application colocation in datacenters.

## Key claims
- Blink removes the host CPU from the steady-state LLM inference path by offloading orchestration to a SmartNIC and GPU.
- The SmartNIC delivers inputs directly into GPU memory via RDMA, bypassing the host CPU.
- A persistent GPU kernel in Blink handles batching, scheduling, and KV-cache management without CPU involvement.
- Blink reduces pre-saturation P99 TTFT by up to 8.47x and P99 TPOT by up to 3.40x compared to baselines.
- Blink improves decode throughput by up to 2.1x and reduces energy per token by up to 48.6%.
- Under CPU interference, existing serving systems degrade by up to two orders of magnitude while Blink remains stable.
- Current LLM serving stacks force operators to reserve CPU headroom, leaving substantial datacenter capacity unutilized.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2604.07609>

## Related
[[concepts/blink|blink]] · [[concepts/llm-inference|llm-inference]] · [[concepts/smartnic|smartnic]] · [[concepts/rdma|rdma]] · [[concepts/kv-cache-management|kv-cache-management]] · [[concepts/persistent-gpu-kernel|persistent-gpu-kernel]] · [[concepts/tensorrt-llm|tensorrt-llm]] · [[concepts/vllm|vllm]] · [[concepts/sglang|sglang]] · [[concepts/cpu-free-inference|cpu-free-inference]] · [[concepts/large-language-model|large-language-model]] · [[concepts/language-model|language-model]] · [[concepts/llm|llm]] · [[episodes/2026-04-10|2026-04-10]]
