---
type: story
story_id: hn_48415709
episode_date: 2026-06-06
rank: 2
source: hacker_news
url: "https://mimicscribe.app/"
title: "Show HN On-device transcriber that's 97 accurate at identifying speakers"
quality_score: 0.688
content_hash: "sha256:3f32c9028875758ff7ca3c0d354ed9430bb6867b46e558d0a2e87feb42824331"
concepts: [speaker-diarization, pyannote, parakeet-stt, fluidaudio, on-device-inference, push-to-talk-dictation, llm-cleanup, bring-your-own-key]
companies: []
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-06-06 10:18:15.014000"
tags: [story, source/hacker-news]
---

## Summary
MimicScribe is a macOS menu bar application built over seven months that performs on-device speaker identification with claimed 97% accuracy during meeting transcription. It uses a port of Pyannote's community-1 diarization model combined with Parakeet STT grammar cues to improve speaker segmentation by masking audio at sentence boundaries. The app offers real-time talking points for discovery calls, a keyboard- and voice-driven interface, and post-meeting voice commands for transcript correction. It supports both a fully on-device free mode and a cloud-augmented mode with bring-your-own-key options to address privacy concerns. The developer targets technical users and is seeking feedback, particularly around the privacy story.

## Key claims
- MimicScribe claims 97% accuracy in on-device speaker identification during meetings.
- The speaker diarization system is built on a port of Pyannote's community-1 model via the FluidAudio project.
- Grammar structure cues from Parakeet STT are used to mask audio by sentence for improved speaker cluster assignment.
- The system intentionally oversegments speakers because merging is easier than untangling incorrect merges.
- A fully on-device mode is available for free with no cloud dependency, while cloud models add features like context-aware speaker merging and action item attribution.
- Recording is controlled via a keyboard shortcut rather than calendar integration to preserve privacy and reduce transcript clutter.
- Post-meeting transcript corrections can be made using natural voice commands such as 'merge this speaker with that speaker'.

## Source
- **Origin:** hacker_news
- **URL:** <https://mimicscribe.app/>

## Related
[[concepts/speaker-diarization|speaker-diarization]] · [[concepts/pyannote|pyannote]] · [[concepts/parakeet-stt|parakeet-stt]] · [[concepts/fluidaudio|fluidaudio]] · [[concepts/on-device-inference|on-device-inference]] · [[concepts/llm-cleanup|llm-cleanup]] · [[concepts/bring-your-own-key|bring-your-own-key]] · [[concepts/cloud|cloud]] · [[concepts/merge|merge]] · [[concepts/llm|llm]] · [[concepts/ai|ai]] · [[episodes/2026-06-06|2026-06-06]]
