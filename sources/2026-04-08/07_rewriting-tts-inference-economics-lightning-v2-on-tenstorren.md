---
type: story
story_id: rss_ba0566b42831
episode_date: 2026-04-08
rank: 7
source: rss_feed
url: "https://arxiv.org/abs/2604.03279"
title: Rewriting TTS Inference Economics Lightning V2 on Tenstorrent Achieves 4x Lower Cost Than NVIDIA L40S
quality_score: 0.897
content_hash: "sha256:e63b056be90dc6c79f42b2d0a1a715323a13bb2ad581a583b8921261ebdf72b4"
concepts: [lightning-v2, text-to-speech-tts, blockfloat8-bfp8, lofi-compute, hardware-software-co-optimization, network-on-chip-noc, low-precision-inference, large-language-models-llms]
companies: [tenstorrent, nvidia]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:34:04.903000"
tags: [story, source/rss-feed]
---

## Summary
Researchers present Lightning V2, a production-grade Text-to-Speech model co-optimized for Tenstorrent hardware. The paper addresses the numerical fragility of TTS models compared to LLMs, noting that aggressive precision reduction techniques like BlockFloat8 and LoFi compute cause audible artifacts in speech synthesis. Through precision-aware architectural design and hardware-software co-optimization leveraging Tenstorrent's Network-on-Chip, distributed SRAM, and deterministic execution model, Lightning V2 achieves over 95% LoFi computational fidelity and more than 80% BlockFloat8 deployment without measurable audio quality degradation. The system achieves approximately 4x lower on-premises accelerator cost compared to an NVIDIA L40S baseline at equivalent throughput.

## Key claims
- TTS models are significantly more numerically fragile than LLMs due to continuous waveform generation and perceptual sensitivity to small numerical perturbations.
- Applying BlockFloat8 and LoFi compute techniques to TTS systems often results in audible artifacts, phase instability, and spectral distortion.
- Lightning V2 achieves over 95% LoFi computational fidelity without measurable degradation in audio quality.
- Lightning V2 enables more than 80% BlockFloat8 deployment while maintaining production audio fidelity.
- Lightning V2 achieves approximately 4x lower on-premises accelerator cost compared to an NVIDIA L40S at equivalent throughput.
- Tenstorrent's Network-on-Chip, distributed SRAM, and deterministic execution model reduce memory movement and redundant weight fetches for efficient low-precision inference.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2604.03279>

## Related
[[concepts/lightning-v2|lightning-v2]] · [[concepts/text-to-speech-tts|text-to-speech-tts]] · [[concepts/blockfloat8-bfp8|blockfloat8-bfp8]] · [[concepts/lofi-compute|lofi-compute]] · [[concepts/hardware-software-co-optimization|hardware-software-co-optimization]] · [[concepts/network-on-chip-noc|network-on-chip-noc]] · [[concepts/low-precision-inference|low-precision-inference]] · [[concepts/large-language-models|large-language-models]] · [[concepts/llms|llms]] · [[companies/tenstorrent|Tenstorrent]] · [[companies/nvidia|NVIDIA]] · [[episodes/2026-04-08|2026-04-08]]
