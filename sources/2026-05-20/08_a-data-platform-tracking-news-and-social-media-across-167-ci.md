---
type: story
story_id: devto_3701496
episode_date: 2026-05-20
rank: 8
source: devto
url: "https://dev.to/gscdataanalytic/a-data-platform-tracking-news-and-social-media-across-167-cities-in-rio-grande-do-norte-for-under-5hh8"
title: A data platform tracking news and social media across 167 cities in Rio Grande do Norte for under R 5 month.
quality_score: 0.928
content_hash: "sha256:a29b6560b9bd3e3f8ffc8842a33ba95f1009c017bfd7b49d50dd8466782ad66a"
concepts: [cloud-run-jobs, apache-airflow, duckdb, bigquery, spacy, dbt, fastapi, workload-identity-federation, oidc, parquet, terraform, github-actions, react, uv-workspace, claude-code]
companies: [google-cloud-platform, anthropic, meta, github]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-20 10:23:18.858000"
tags: [story, source/devto]
---

## Summary
A developer built a data platform monitoring all 167 municipalities in Rio Grande do Norte, Brazil, tracking news and social media (Facebook, Instagram, X, TikTok) for under R$5/month. The cost was dramatically reduced by using Cloud Run Jobs instead of always-on Airflow, local DuckDB for development, and spaCy-based NLP instead of LLMs for routine text processing. The stack includes Python, dbt, BigQuery, Terraform, GCP, FastAPI, React, TypeScript, spaCy, and uv workspace, with CI/CD via GitHub Actions using Workload Identity Federation. The author emphasizes that many modern data stacks are oversized by default, and documents every architectural decision in the project README.

## Key claims
- The platform monitors all 167 municipalities in Rio Grande do Norte using news and social media data for under R$5/month.
- Using Cloud Run Jobs instead of always-on Airflow reduced infrastructure costs by approximately 30x.
- DuckDB is used locally during development to avoid burning cloud quota, with BigQuery reserved for production.
- spaCy with deterministic Portuguese-language rules is used for NLP instead of LLMs, keeping processing fast, cheap, and auditable.
- LLMs are only invoked when a user requests an explanation of specific content.
- GitHub Actions authenticates to GCP via Workload Identity Federation with OIDC, storing zero private keys in secrets.
- Part of the development was done via pair programming with Claude Code, which the author credits for accelerating writing but not replacing technical decision-making.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/gscdataanalytic/a-data-platform-tracking-news-and-social-media-across-167-cities-in-rio-grande-do-norte-for-under-5hh8>

## Related
[[concepts/cloud-run-jobs|cloud-run-jobs]] · [[concepts/apache-airflow|apache-airflow]] · [[concepts/duckdb|duckdb]] · [[concepts/bigquery|bigquery]] · [[concepts/spacy|spacy]] · [[concepts/dbt|dbt]] · [[concepts/fastapi|fastapi]] · [[concepts/workload-identity-federation|workload-identity-federation]] · [[concepts/parquet|parquet]] · [[concepts/github-actions|github-actions]] · [[concepts/identity-federation|identity-federation]] · [[concepts/workload-identity|workload-identity]] · [[concepts/data-engineering|data-engineering]] · [[concepts/data-pipeline|data-pipeline]] · [[concepts/open-source|open-source]] · [[concepts/typescript|typescript]] · [[concepts/data-lake|data-lake]] · [[concepts/workspace|workspace]] · [[concepts/analytics|analytics]] · [[concepts/cloud-run|cloud-run]] · [[concepts/pipeline|pipeline]] · [[concepts/airflow|airflow]] · [[concepts/claude|claude]] · [[concepts/python|python]] · [[concepts/cloud|cloud]] · [[concepts/mlops|mlops]] · [[concepts/llms|llms]] · [[concepts/api|api]] · [[concepts/ai|ai]] · [[companies/google-cloud-platform|Google Cloud Platform]] · [[companies/anthropic|Anthropic]] · [[companies/meta|Meta]] · [[companies/github|GitHub]] · [[episodes/2026-05-20|2026-05-20]]
