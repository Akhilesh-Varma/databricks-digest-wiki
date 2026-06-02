---
type: story
story_id: hn_47891569
episode_date: 2026-04-25
rank: 5
source: hacker_news
url: "https://privateclaw.dev"
title: Show HN PrivateClaw AI agents running in confidential VMs you can verify
quality_score: 0.611
content_hash: "sha256:81954e748d5b99203dcb53741e0da3e3b23db1b9614d4fc824b91faaf9b73ee7"
concepts: [confidential-vms, trusted-execution-environments, amd-sev-snp, hardware-level-encryption, vllm, azure-confidential-compute, attestation, reproducible-builds, open-source-cli]
companies: [amd, azure, confidential-ai]
people: []
extractor_model: gemini-2.5-flash-lite
extracted_at: "2026-04-27 13:06:54.060099"
tags: [story, source/hacker-news]
---

## Summary
PrivateClaw offers a service for running AI agents within confidential virtual machines (CVMs) that leverage AMD's SEV-SNP technology for hardware-level data encryption. This ensures that user data, prompts, and completions remain private, as they are encrypted at the hardware layer and inaccessible even to the hypervisor or host OS. The service provides a dedicated CVM per user and includes an open-source CLI for a multi-step verification process, allowing users to confirm the integrity and security of their AI agent's environment. PrivateClaw runs on Azure Confidential Compute and utilizes Confidential AI's vLLM deployment, with plans for verifiable builds and reproducible builds in the future.

## Key claims
- PrivateClaw removes the need to trust hosted platforms with plaintext data by running AI agents in confidential VMs.
- PrivateClaw utilizes AMD SEV-SNP technology for hardware-level data encryption within Trusted Execution Environments (TEEs).
- User data, prompts, and completions are encrypted at the hardware level and protected from the host OS and hypervisor.
- Each user receives a dedicated Confidential VM (CVM) with hardware-enforced memory encryption.
- An open-source CLI enables users to perform a 5-step verification process to ensure the security of their CVM.
- PrivateClaw runs on Azure Confidential Compute and uses Confidential AI's TEE-backed vLLM deployment.
- Future roadmap includes attestable and reproducible builds for enhanced software verification.

## Source
- **Origin:** hacker_news
- **URL:** <https://privateclaw.dev>

## Related
[[concepts/confidential-vms|confidential-vms]] · [[concepts/trusted-execution-environments|trusted-execution-environments]] · [[concepts/amd-sev-snp|amd-sev-snp]] · [[concepts/hardware-level-encryption|hardware-level-encryption]] · [[concepts/vllm|vllm]] · [[concepts/azure-confidential-compute|azure-confidential-compute]] · [[concepts/attestation|attestation]] · [[concepts/open-source-cli|open-source-cli]] · [[concepts/confidential-compute|confidential-compute]] · [[concepts/access-control|access-control]] · [[concepts/open-source|open-source]] · [[concepts/ai-agents|ai-agents]] · [[concepts/openclaw|openclaw]] · [[concepts/azure|azure]] · [[concepts/cloud|cloud]] · [[concepts/cli|cli]] · [[concepts/ssh|ssh]] · [[concepts/ai|ai]] · [[companies/amd|AMD]] · [[companies/azure|Azure]] · [[companies/confidential-ai|Confidential AI]] · [[episodes/2026-04-25|2026-04-25]]
