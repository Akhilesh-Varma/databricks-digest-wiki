---
type: story
story_id: devto_3865898
episode_date: 2026-06-11
rank: 7
source: devto
url: "https://dev.to/dalla/modern-data-stack-migration-day-1-scaling-to-8-companies-with-dry-architecture-and-chasing-a-34e2"
title: Modern Data Stack Migration Day 1 Scaling to 8 Companies with DRY Architecture and Chasing a 2M Discrepancy
quality_score: 0.847
content_hash: "sha256:e0e8304a738b3e1d83e29fa7be566a3242c545191cef883c77ff93a687c06bd7"
concepts: [modern-data-stack, dry-architecture, dbt, clickhouse, bronze-silver-gold-lakehouse-architecture, qlik, dbt-macros, cli-parameterization, claude]
companies: [anthropic]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-06-11 10:18:06.132000"
tags: [story, source/devto]
---

## Summary
The author describes Day 1 of migrating a legacy data system—built on spreadsheets and Qlik—into a modern data stack using Python, ClickHouse, and dbt across 8 companies. The migration involved refactoring duplicated per-company extraction scripts into a single parameterized DRY architecture. While Bronze and Silver layer ingestion validated successfully with matching row counts, the Gold layer revealed a $2 million USD revenue discrepancy compared to the legacy system. The author suspects undocumented legacy business rules around invoice filtering, cancellation logic, or tax handling are responsible. Next steps include auditing dbt macros, aligning multi-company transformation logic, and scaling the pipeline to the remaining 7 companies once parity is achieved.

## Key claims
- The legacy system had duplicated Python extraction scripts for each of 8 companies, which were refactored into a single parameterized DRY codebase.
- Claude (AI) was used to generate the initial application skeleton for the new architecture.
- Bronze and Silver layer data ingestion validated successfully with matching row counts against the legacy system.
- The Gold layer materialization revealed a $2 million USD revenue overcount compared to the legacy system.
- The discrepancy is suspected to stem from undocumented legacy business rules such as multi-company exclusions, cancellation filters, or tax logic.
- The migration strategy keeps ClickHouse Bronze tables structured 1-to-1 with legacy CSV schemas to minimize disruption for BI consumers.
- The plan is to achieve 100% data parity for Company 1 before scaling the pipeline to the remaining 7 companies.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/dalla/modern-data-stack-migration-day-1-scaling-to-8-companies-with-dry-architecture-and-chasing-a-34e2>

## Related
[[concepts/modern-data-stack|modern-data-stack]] · [[concepts/dry-architecture|dry-architecture]] · [[concepts/dbt|dbt]] · [[concepts/clickhouse|clickhouse]] · [[concepts/bronze-silver-gold-lakehouse-architecture|bronze-silver-gold-lakehouse-architecture]] · [[concepts/qlik|qlik]] · [[concepts/dbt-macros|dbt-macros]] · [[concepts/data-engineering|data-engineering]] · [[concepts/data-ingestion|data-ingestion]] · [[concepts/bronze-layer|bronze-layer]] · [[concepts/gold-layer|gold-layer]] · [[concepts/data-stack|data-stack]] · [[concepts/pipeline|pipeline]] · [[concepts/having|having]] · [[concepts/python|python]] · [[concepts/cli|cli]] · [[concepts/csv|csv]] · [[concepts/ai|ai]] · [[companies/anthropic|Anthropic]] · [[episodes/2026-06-11|2026-06-11]]
