---
type: story
story_id: hn_47935246
episode_date: 2026-04-29
rank: 5
source: hacker_news
url: "https://github.com/rocky-data/rocky"
title: "Show HN Rocky Rust SQL engine with branches, replay, column lineage"
quality_score: 0.817
content_hash: "sha256:9bd32dcaf79ea4ee04396d146c5581da3444962a6068439515602f9f3877d75a"
concepts: [rocky, unity-catalog, column-level-lineage, dag-directed-acyclic-graph, delta-shallow-clone, snowflake-zero-copy-cloning, lsp-language-server-protocol, scim, dagster, dbt, duckdb, apache-2-0-license]
companies: [databricks, snowflake, google-bigquery, fivetran, airbyte, dagster-labs]
people: [hugo]
extractor_model: claude-sonnet-4-6
extracted_at: "2026-04-29 10:20:29.842000"
tags: [story, source/hacker-news]
---

## Summary
Rocky is a Rust-based SQL pipeline control plane built by Hugo, designed to sit on top of existing warehouses like Databricks and Snowflake rather than replace them. It owns the DAG, providing compile-time column-level lineage, branching and replay of pipeline runs, cost attribution, and a governance surface including column classification, per-environment masking, and audit trails. The project reached a governance milestone with engine versions v1.16.0 and v1.17.4, integrating with Unity Catalog on Databricks and masking policies on Snowflake. Rocky is open-source under Apache 2.0, ships a VS Code extension with LSP support, and offers a first-class Dagster integration for orchestration. Adapters exist for Databricks (GA), Snowflake (Beta), BigQuery (Beta), and DuckDB.

## Key claims
- Rocky is a Rust-based control plane for warehouse SQL pipelines that keeps storage and compute in the existing warehouse while owning the DAG.
- Column-level lineage is derived at compile time by a type checker that traces columns through joins, CTEs, and windows, surfaced inline in VS Code via LSP.
- Rocky v1.16.0 and v1.17.4 (tagged 2026-04-26) completed end-to-end governance features including column classification, per-env masking, an 8-field audit trail, compliance rollup, role-graph reconciliation, and retention policies.
- Branching creates logical copies of pipeline table schemas, with native Delta SHALLOW CLONE and Snowflake zero-copy planned; replay reconstructs which SQL ran against which inputs.
- Every pipeline run produces per-model cost metrics (bytes, duration), and budget blocks in rocky.toml can fire a budget_breach hook event.
- Rocky integrates with Unity Catalog for Databricks governance and with Snowflake masking policies, and supports dialect-divergence linting across Databricks, Snowflake, BigQuery, and DuckDB.
- Rocky is released under Apache 2.0 and is explicitly not a warehouse replacement, not a Fivetran replacement, and not a hosted dbt Cloud equivalent.

## Source
- **Origin:** hacker_news
- **URL:** <https://github.com/rocky-data/rocky>

## Related
[[concepts/rocky|rocky]] · [[concepts/unity-catalog|unity-catalog]] · [[concepts/column-level-lineage|column-level-lineage]] · [[concepts/dag-directed-acyclic-graph|dag-directed-acyclic-graph]] · [[concepts/dagster|dagster]] · [[concepts/databricks|databricks]] · [[concepts/governance|governance]] · [[concepts/snowflake|snowflake]] · [[concepts/dbt-cloud|dbt-cloud]] · [[concepts/pipeline|pipeline]] · [[concepts/bigquery|bigquery]] · [[concepts/parquet|parquet]] · [[concepts/delta|delta]] · [[concepts/saas|saas]] · [[concepts/dag|dag]] · [[concepts/sql|sql]] · [[concepts/git|git]] · [[concepts/ai|ai]] · [[companies/databricks|Databricks]] · [[companies/snowflake|Snowflake]] · [[companies/google-bigquery|Google BigQuery]] · [[companies/fivetran|Fivetran]] · [[companies/airbyte|Airbyte]] · [[companies/dagster-labs|Dagster Labs]] · [[people/hugo|Hugo]] · [[episodes/2026-04-29|2026-04-29]]
