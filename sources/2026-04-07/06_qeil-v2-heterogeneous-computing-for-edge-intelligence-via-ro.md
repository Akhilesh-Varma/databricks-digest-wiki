---
type: story
story_id: rss_fadd6376bbff
episode_date: 2026-04-07
rank: 6
source: rss_feed
url: "https://arxiv.org/abs/2602.06057"
title: QEIL v2 Heterogeneous Computing for Edge Intelligence via Roofline-Derived Pareto-Optimal Energy Modeling and Multi-Objective Orchestration
quality_score: 0.906
content_hash: "sha256:200c78ae44e5b21fc858b1f3fefe71bd614fe8b8f55bd3e30fca501249fff508"
concepts: [qeil-v2, roofline-model, pareto-guided-simulated-annealing-with-momentum-pgsam, dasi, cpq, phi-thermal-yield, eac-arde-selection-cascade, csvet-early-stopping, large-language-models-llms, heterogeneous-edge-computing, llama-3-1-8b, 4-bit-quantization, multi-objective-optimization, cmos-leakage-physics]
companies: []
people: [kumar-jha]
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:36:58.965000"
tags: [story, source/rss-feed]
---

## Summary
QEIL v2 is a framework for deploying large language models on heterogeneous edge devices, replacing static heuristics with physics-grounded, runtime-adaptive models. It introduces three device-workload metrics—DASI, CPQ, and Phi—derived from semiconductor physics to form a unified energy equation. Optimization is handled by PGSAM (Pareto-Guided Simulated Annealing with Momentum), which simultaneously minimizes energy, latency, and device underutilization. At inference time, an EAC ARDE selection cascade with CSVET early stopping provides progressive verification. Evaluated across seven model families on WikiText-103, GSM8K, and ARC-Challenge, QEIL v2 achieves a 2.86x IPW improvement over standard inference and is the first edge orchestration system to surpass the IPW 1.0 empirical reference mark.

## Key claims
- QEIL v2 replaces all static heuristics from QEIL v1 with physics-grounded, runtime-adaptive models derived from semiconductor physics.
- Three new device-workload metrics—DASI (roofline-derived compute utilization), CPQ (memory pressure), and Phi (thermal yield)—form a unified energy equation.
- PGSAM (Pareto-Guided Simulated Annealing with Momentum) simultaneously optimizes energy, latency, and device underutilization.
- QEIL v2 achieves 75.7% pass@k at 63.8W with IPW 0.9749, a 2.86x improvement over standard inference.
- Applied to a 4-bit Llama-3.1-8B, QEIL v2 achieves IPW 1.024 at 54.8W, the first edge orchestration system to surpass the IPW 1.0 empirical reference mark.
- Total energy drops 75.6% versus standard inference, with 38.3% latency reduction, zero thermal throttling, and 100% fault recovery across all benchmarks.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2602.06057>

## Related
[[concepts/qeil-v2|qeil-v2]] · [[concepts/roofline-model|roofline-model]] · [[concepts/pareto-guided-simulated-annealing-with-momentum-pgsam|pareto-guided-simulated-annealing-with-momentum-pgsam]] · [[concepts/dasi|dasi]] · [[concepts/cpq|cpq]] · [[concepts/phi-thermal-yield|phi-thermal-yield]] · [[concepts/eac-arde-selection-cascade|eac-arde-selection-cascade]] · [[concepts/csvet-early-stopping|csvet-early-stopping]] · [[concepts/large-language-models-llms|large-language-models-llms]] · [[concepts/heterogeneous-edge-computing|heterogeneous-edge-computing]] · [[concepts/multi-objective-optimization|multi-objective-optimization]] · [[concepts/large-language-models|large-language-models]] · [[concepts/early-stopping|early-stopping]] · [[concepts/llms|llms]] · [[people/kumar-jha|Kumar Jha]] · [[episodes/2026-04-07|2026-04-07]]
