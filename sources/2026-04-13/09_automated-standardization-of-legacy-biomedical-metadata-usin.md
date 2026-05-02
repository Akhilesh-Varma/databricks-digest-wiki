---
type: story
story_id: rss_6802522cea23
episode_date: 2026-04-13
rank: 9
source: rss_feed
url: "https://arxiv.org/abs/2604.08552"
title: Automated Standardization of Legacy Biomedical Metadata Using an Ontology-Constrained LLM Agent
quality_score: 0.75
content_hash: "sha256:954f73b0a1b20c6b464b7d5856a5733e1614680136e75dc7953aae90be986281"
concepts: [llm-agent, ontology-constrained-metadata-standardization, fair-data-principles, retrieval-augmented-generation, biomedical-terminology-services, hubmap, machine-actionable-metadata-templates]
companies: []
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:24:06.924000"
tags: [story, source/rss-feed]
---

## Summary
This paper presents an LLM-based system for automatically standardizing legacy biomedical metadata by querying authoritative biomedical terminology services in real time. The system encodes metadata standards as machine-actionable templates with rich field specifications and precise value constraints. It was evaluated on 839 legacy metadata records from the Human BioMolecular Atlas Program (HuBMAP) using an expert-curated gold standard for exact-match assessment. Results show that augmenting the LLM with real-time tool access consistently improves prediction accuracy over static prompt-based approaches for both ontology-constrained and non-ontology-constrained fields. The work demonstrates a practical, scalable approach to producing FAIR-compliant biomedical datasets.

## Key claims
- Scientific metadata are often incomplete and noncompliant with community standards, limiting dataset findability, interoperability, and reuse.
- Existing LLM-based metadata standardization approaches treat ontology constraints as static text prompts, relying solely on the model's training knowledge.
- The proposed system queries authoritative biomedical terminology services in real time to retrieve canonically correct vocabulary terms on demand.
- The system was evaluated on 839 legacy metadata records from the Human BioMolecular Atlas Program (HuBMAP) using an expert-curated gold standard.
- Real-time tool access consistently improves LLM prediction accuracy over the LLM-alone baseline across both ontology-constrained and non-ontology-constrained fields.
- Producing FAIR datasets requires encoding metadata standards as machine-actionable templates with rich field specifications and precise value constraints.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2604.08552>

## Related
[[concepts/llm-agent|llm-agent]] · [[concepts/ontology-constrained-metadata-standardization|ontology-constrained-metadata-standardization]] · [[concepts/fair-data-principles|fair-data-principles]] · [[concepts/retrieval-augmented-generation|retrieval-augmented-generation]] · [[concepts/biomedical-terminology-services|biomedical-terminology-services]] · [[concepts/hubmap|hubmap]] · [[concepts/machine-actionable-metadata-templates|machine-actionable-metadata-templates]] · [[concepts/llms|llms]] · [[concepts/llm|llm]] · [[episodes/2026-04-13|2026-04-13]]
