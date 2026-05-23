---
type: story
story_id: community_147c6901dc38
episode_date: 2026-05-23
rank: 2
source: databricks_community
url: "https://community.databricks.com/t5/technical-blog/partner-blog-847-models-12-weeks-77-less-inside-r1-s-snowflake/ba-p/157284"
title: "PARTNER BLOG 847 Models, 12 Weeks, 77 Less Inside R1's Snowflake-to-Databricks Migration"
quality_score: 0.78
content_hash: "sha256:687f6aecff9f8a82a3fffbe6df1119f6e27d9216677ee4dad93641f9ff337c5f"
concepts: [data-vault, dbt-core, delta-lake, unity-catalog, databricks-sql-warehouse, delta-merge, phare-revenue-operating-system, federated-query, predicate-pushdown]
companies: [r1, databricks, snowflake, lovelytics]
people: [zheng-zhu]
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-23 10:18:32.444000"
tags: [story, source/databricks-community]
---

## Summary
R1, a healthcare revenue cycle management company, migrated 847 dbt models from Snowflake to Databricks in 12 weeks, achieving a 77% reduction in per-run DBU costs. The migration was led by R1's Zheng Zhu and delivered in partnership with Lovelytics, covering a full Data Vault pipeline across five layers built on dbt Core, Delta Lake, and Unity Catalog. Key engineering challenges included non-portable hash functions, differences in MERGE semantics between Snowflake and Delta, complex dependency graphs with 735 internal edges, and the need to read from three simultaneous data sources. The team had to maintain synchronization with a live Snowflake codebase throughout the migration to ensure continuity of operations. The final output comprises 35 Information Mart tables representing the business-ready view of the entire revenue cycle.

## Key claims
- R1 migrated 847 dbt models from Snowflake to Databricks in 12 weeks.
- The migration reduced per-run DBU costs by approximately 77%.
- The pipeline was built on dbt Core, Delta Lake, and Unity Catalog on Databricks, running on a 2XL SQL Warehouse.
- Snowflake's HASH function is non-portable, meaning surrogate keys differ between platforms by design, requiring a custom testing strategy.
- Delta MERGE requires at most one source row per target key, unlike Snowflake's MERGE which accepts duplicates non-deterministically, necessitating QUALIFY ROW_NUMBER fixes across hundreds of models.
- R1's Information Mart Transient layer contains 460 models with 735 internal dependency edges, requiring wave-ordered build selectors for safe parallel execution.
- The pipeline had to simultaneously read from Delta tables outside Unity Catalog, Delta tables inside Unity Catalog, and live federated Snowflake without forking the codebase.

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/technical-blog/partner-blog-847-models-12-weeks-77-less-inside-r1-s-snowflake/ba-p/157284>

## Related
[[concepts/data-vault|data-vault]] · [[concepts/dbt-core|dbt-core]] · [[concepts/delta-lake|delta-lake]] · [[concepts/unity-catalog|unity-catalog]] · [[concepts/databricks-sql-warehouse|databricks-sql-warehouse]] · [[concepts/delta-merge|delta-merge]] · [[concepts/phare-revenue-operating-system|phare-revenue-operating-system]] · [[concepts/federated-query|federated-query]] · [[concepts/surrogate-keys|surrogate-keys]] · [[concepts/sql-warehouse|sql-warehouse]] · [[concepts/orchestration|orchestration]] · [[concepts/delta-tables|delta-tables]] · [[concepts/databricks|databricks]] · [[concepts/warehouse|warehouse]] · [[concepts/snowflake|snowflake]] · [[concepts/analytics|analytics]] · [[concepts/pipeline|pipeline]] · [[concepts/merge|merge]] · [[concepts/delta|delta]] · [[concepts/dbt|dbt]] · [[concepts/sql|sql]] · [[concepts/dbu|dbu]] · [[concepts/ai|ai]] · [[companies/r1|R1]] · [[companies/databricks|Databricks]] · [[companies/snowflake|Snowflake]] · [[companies/lovelytics|Lovelytics]] · [[people/zheng-zhu|Zheng Zhu]] · [[episodes/2026-05-23|2026-05-23]]
