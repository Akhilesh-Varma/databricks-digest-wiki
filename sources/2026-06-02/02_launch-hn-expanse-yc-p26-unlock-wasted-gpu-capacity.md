---
type: story
story_id: hn_48356312
episode_date: 2026-06-02
rank: 2
source: hacker_news
url: "https://news.ycombinator.com/item?id=48356312"
title: Launch HN Expanse YC P26 Unlock Wasted GPU Capacity
quality_score: 0.845
content_hash: "sha256:452ed0b61fd74b6628344ef29af179e3db272f23128bdf85b3172c0c8a80d246"
concepts: [slurm, kubernetes, hpc-resource-prediction, dcgm, cupti, cgroups, gpu-cluster-observability, multimodal-deep-learning, stack-profiling, llm-coding-agents]
companies: [expanse, y-combinator, epcc-edinburgh-parallel-computing-centre, google-deepmind, anthropic, openai]
people: [ismaeel-bashir, adrian-jackson]
extractor_model: claude-sonnet-4-6
extracted_at: "2026-06-02 10:19:29.908000"
tags: [story, source/hacker-news]
---

## Summary
Expanse is a YC W26 startup building software to reduce wasted GPU and HPC cluster capacity by predicting actual resource needs before job submission. The system installs on every node, hooks into SLURM or Kubernetes schedulers, and uses deep learning models trained on source code, job submission scripts, and live hardware telemetry to generate accurate resource recommendations. The founders measured a national-scale HPC cluster and found 59% of compute was wasted across 122,000 jobs, equivalent to roughly $8.5M in one month at on-demand cloud rates. Expanse also provides live observability dashboards and failure diagnosis with code-level fix suggestions. The company claims its models outperform frontier LLMs like GPT-5.5, Claude Opus 4.8, and Gemini on resource prediction tasks by approximately 8x.

## Key claims
- Datacenters run at roughly 30–40% effective utilization due to users over-requesting resources by two to three times.
- A one-month measurement of a national-scale HPC cluster found 59% of compute wasted across 122,000 jobs, worth ~$8.5M at on-demand cloud rates.
- Expanse's multimodal HPC resource predictor scored 34% better than any baseline on EPCC's clusters and outperformed frontier LLMs on the same prediction task by roughly 8x.
- The system hooks into SLURM and Kubernetes scheduler lifecycles without requiring changes to how users submit jobs.
- Expanse fine-tunes cluster-specific models that improve over time as more workloads run, making it adaptive to new hardware and workload patterns.
- Benchmarks against Gemini 3.5 Pro, Claude Opus 4.8, GPT-5.5, and Codex 5.3 showed no correlation between model size or iteration and accuracy improvement on this task.
- Expanse provides uncertainty estimates and p90 values so users can choose their own risk tolerance for resource provisioning.

## Source
- **Origin:** hacker_news
- **URL:** <https://news.ycombinator.com/item?id=48356312>

## Related
[[concepts/slurm|slurm]] · [[concepts/kubernetes|kubernetes]] · [[concepts/hpc-resource-prediction|hpc-resource-prediction]] · [[concepts/dcgm|dcgm]] · [[concepts/cupti|cupti]] · [[concepts/gpu-cluster-observability|gpu-cluster-observability]] · [[concepts/multimodal-deep-learning|multimodal-deep-learning]] · [[concepts/stack-profiling|stack-profiling]] · [[concepts/llm-coding-agents|llm-coding-agents]] · [[concepts/claude-opus-4-8|claude-opus-4-8]] · [[concepts/coding-agents|coding-agents]] · [[concepts/observability|observability]] · [[concepts/telemetry|telemetry]] · [[concepts/metadata|metadata]] · [[concepts/gpt-5-5|gpt-5-5]] · [[concepts/vacuum|vacuum]] · [[concepts/cloud|cloud]] · [[concepts/codex|codex]] · [[concepts/llms|llms]] · [[concepts/cli|cli]] · [[concepts/llm|llm]] · [[concepts/ai|ai]] · [[companies/expanse|Expanse]] · [[companies/y-combinator|Y Combinator]] · [[companies/epcc-edinburgh-parallel-computing-centre|EPCC (Edinburgh Parallel Computing Centre)]] · [[companies/google-deepmind|Google DeepMind]] · [[companies/anthropic|Anthropic]] · [[companies/openai|OpenAI]] · [[people/ismaeel-bashir|Ismaeel Bashir]] · [[people/adrian-jackson|Adrian Jackson]] · [[episodes/2026-06-02|2026-06-02]]
