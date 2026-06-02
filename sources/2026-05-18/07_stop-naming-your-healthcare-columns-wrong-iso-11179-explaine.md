---
type: story
story_id: devto_3690500
episode_date: 2026-05-18
rank: 7
source: devto
url: "https://dev.to/season_mudbhary_7856e4083/stop-naming-your-healthcare-columns-wrong-iso-11179-explained-2hnb"
title: Stop Naming Your Healthcare Columns Wrong ISO-11179 Explained
quality_score: 0.936
content_hash: "sha256:2a33a1fccd54da639ea17a67a7fda300a39d2176c4d0574ef0ee959e49ab9301"
concepts: [iso-11179, snake-case, data-element-naming-standards, healthcare-data-warehouse, mdatool]
companies: [snowflake, google-bigquery, databricks]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-18 10:20:15.788000"
tags: [story, source/devto]
---

## Summary
The article argues that healthcare data engineering suffers from inconsistent column naming across systems, making data integration difficult. It introduces ISO-11179, an international standard for naming data elements, as a solution that enforces a predictable structure of entity, concept, and type suffix. The standard mandates lowercase snake_case, standardized abbreviations, and domain-specific prefixes for areas like claims, members, providers, and pharmacy. A tool called mdatool is referenced as a resource for looking up 100,000 standardized healthcare terms and auditing column names against the standard. The article provides concrete before-and-after examples of common naming mistakes and their ISO-11179-compliant corrections.

## Key claims
- ISO-11179 is an international standard designed to make data elements interoperable across systems, directly addressing healthcare data naming inconsistencies.
- Every ISO-11179-compliant column name should encode the entity, concept, and data type, eliminating the need to consult a data dictionary.
- Standard suffixes such as Date, Code, Id, Amt, Nm, Ind, and Cnt communicate the expected data type directly in the column name.
- Lowercase snake_case is recommended because Snowflake, BigQuery, and Databricks all handle it consistently, avoiding case-sensitivity issues.
- The mdatool healthcare data glossary contains 100,000 standardized healthcare terms with their ISO-11179 abbreviations.
- Common naming mistakes include missing entity prefixes, PascalCase, SCREAMING_SNAKE_CASE, and ambiguous abbreviations that lack domain context.
- Healthcare domains such as claims, member enrollment, provider, clinical, and pharmacy each have their own standard ISO-11179 prefixes.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/season_mudbhary_7856e4083/stop-naming-your-healthcare-columns-wrong-iso-11179-explained-2hnb>

## Related
[[concepts/iso-11179|iso-11179]] · [[concepts/snake-case|snake-case]] · [[concepts/data-element-naming-standards|data-element-naming-standards]] · [[concepts/healthcare-data-warehouse|healthcare-data-warehouse]] · [[concepts/mdatool|mdatool]] · [[concepts/data-engineering|data-engineering]] · [[concepts/data-warehouses|data-warehouses]] · [[concepts/databricks|databricks]] · [[concepts/warehouses|warehouses]] · [[concepts/snowflake|snowflake]] · [[concepts/pipeline|pipeline]] · [[concepts/bigquery|bigquery]] · [[companies/snowflake|Snowflake]] · [[companies/google-bigquery|Google BigQuery]] · [[companies/databricks|Databricks]] · [[episodes/2026-05-18|2026-05-18]]
