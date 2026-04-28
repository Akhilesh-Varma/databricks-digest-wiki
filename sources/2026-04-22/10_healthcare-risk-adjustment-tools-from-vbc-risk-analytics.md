---
type: story
story_id: devto_3532678
episode_date: 2026-04-22
rank: 10
source: devto
url: "https://dev.to/vbc_risk_analytics/building-healthcare-risk-adjustment-tools-an-introduction-to-vbc-risk-analytics-50n6"
title: Healthcare Risk Adjustment Tools from VBC Risk Analytics
quality_score: 0.809
content_hash: "sha256:3d9a65e58d3a4a405cf2075ae20c2bebc696e3d9a64d70d40083aac43ef71f6e"
concepts: [hierarchical-condition-category, risk-adjustment-factor, icd-10, cms-hcc-model]
companies: [vbc-risk-analytics]
people: []
extractor_model: llama-3.3-70b-versatile
extracted_at: "2026-04-28 04:03:16.529000"
tags: [story, source/devto]
---

## Summary
Healthcare risk adjustment is a complex process used by Medicare to ensure fair payment to health plans based on the health status of their enrolled members. The process involves calculating a Risk Adjustment Factor (RAF) score for each member, which reflects their predicted cost relative to the average Medicare beneficiary. The RAF score is built by mapping ICD-10 diagnosis codes to Hierarchical Condition Category (HCC) categories and applying interaction factors. Small errors in this calculation can result in significant over- or underpayment for health plans. VBC Risk Analytics has spent years building API-first tools to address the technical complexity of healthcare risk adjustment.

## Key claims
- Risk adjustment is the process Medicare uses to ensure fair payment to health plans based on the health status of their enrolled members.
- The Hierarchical Condition Category (HCC) model is used to calculate the Risk Adjustment Factor (RAF) score for each Medicare Advantage member.
- The ICD-10-to-HCC mapping is not a simple lookup table, with approximately 70,000 ICD-10-CM codes and 86 HCC categories in the CMS-HCC V28 model.
- Small errors in the RAF score calculation can result in significant over- or underpayment for health plans with large numbers of Medicare Advantage members.
- The CMS-HCC model coefficients change with each model version, requiring updates to implementation code to ensure accurate calculations.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/vbc_risk_analytics/building-healthcare-risk-adjustment-tools-an-introduction-to-vbc-risk-analytics-50n6>

## Related
[[concepts/hierarchical-condition-category|hierarchical-condition-category]] · [[concepts/risk-adjustment-factor|risk-adjustment-factor]] · [[concepts/cms-hcc-model|cms-hcc-model]] · [[concepts/data-engineering|data-engineering]] · [[concepts/analytics|analytics]] · [[concepts/api|api]] · [[companies/vbc-risk-analytics|VBC Risk Analytics]] · [[episodes/2026-04-22|2026-04-22]]
