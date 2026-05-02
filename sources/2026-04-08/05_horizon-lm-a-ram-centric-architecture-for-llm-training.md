---
type: story
story_id: rss_57c9a1f38f7a
episode_date: 2026-04-08
rank: 5
source: rss_feed
url: "https://arxiv.org/abs/2602.04816"
title: Horizon-LM A RAM-Centric Architecture for LLM Training
quality_score: 0.911
content_hash: "sha256:2f99d100b7b55ae8ca8e03f5a4e302b4ae41419b5f655397f10a64c832d641b2"
concepts: [horizon-lm, large-language-model-training, cpu-offloading, deepspeed-zero-3, autograd, gradient-checkpointing-recomputation, double-buffering, distributed-parallelism, instruction-tuning, reinforcement-learning-from-human-feedback]
companies: []
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:33:25.427000"
tags: [story, source/rss-feed]
---

## Summary
Horizon-LM is a RAM-centric training architecture for large language models that repositions host CPU memory as the authoritative parameter store while using GPUs only as transient compute engines. The system eliminates persistent GPU-resident modules and autograd graphs, instead relying on explicit recomputation and manual gradient propagation. A pipelined double-buffered execution engine enables training of models up to 120B parameters on a single H200 GPU with 1.5 TB of host RAM. On a standard single A100 machine, Horizon-LM achieves up to 12.2× higher training throughput than DeepSpeed ZeRO-3 with CPU offloading. The work argues that host memory, not GPU memory, defines the true feasibility boundary for node-scale large-model training.

## Key claims
- Horizon-LM treats host RAM as the authoritative parameter store and GPUs as transient compute engines via a CPU-master, GPU-template execution model.
- The system eliminates persistent GPU-resident modules and autograd graphs, using explicit recomputation and manual gradient propagation instead.
- A pipelined double-buffered execution engine decouples model scale from GPU count and bounds memory usage to the theoretical parameter footprint.
- On a single H200 GPU with 1.5 TB host RAM, Horizon-LM reliably trains models up to 120B parameters.
- On a single A100 machine, Horizon-LM achieves up to 12.2× higher training throughput than DeepSpeed ZeRO-3 with CPU offloading.
- Horizon-LM sustains high device utilization and predictable memory growth across platforms and scales.
- Host memory, not GPU memory, defines the true feasibility boundary for node-scale large-model training according to the authors.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2602.04816>

## Related
[[concepts/horizon-lm|horizon-lm]] · [[concepts/large-language-model-training|large-language-model-training]] · [[concepts/cpu-offloading|cpu-offloading]] · [[concepts/deepspeed-zero-3|deepspeed-zero-3]] · [[concepts/autograd|autograd]] · [[concepts/gradient-checkpointing-recomputation|gradient-checkpointing-recomputation]] · [[concepts/double-buffering|double-buffering]] · [[concepts/large-language-models|large-language-models]] · [[concepts/llms|llms]] · [[episodes/2026-04-08|2026-04-08]]
