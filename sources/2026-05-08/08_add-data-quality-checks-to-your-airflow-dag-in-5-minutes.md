---
type: story
story_id: devto_3629053
episode_date: 2026-05-08
rank: 8
source: devto
url: "https://dev.to/vahid_saber_d47950be99729/add-data-quality-checks-to-your-airflow-dag-in-5-minutes-7l5"
title: Add Data Quality Checks to Your Airflow DAG in 5 Minutes
quality_score: 0.852
content_hash: "sha256:4ebd313e68257ad0ac619a7e84ddbd30f4cb7f9e361d09b7c0a775d886a758ad"
concepts: [apache-airflow, dag, dqlens, dqlensoperator, bashoperator, data-quality-checks, great-expectations, soda, xcom, schema-drift, postgresql, duckdb, sqlite, mysql]
companies: []
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-08 10:23:05.612000"
tags: [story, source/devto]
---

## Summary
The article describes how to add automated data quality checks to Apache Airflow DAGs using a tool called DQLens in under five minutes. DQLens can be integrated via a BashOperator or a dedicated DQLensOperator, and it auto-generates checks by profiling tables and comparing runs against a stored baseline. It detects issues such as null rate spikes, row count anomalies, schema drift, empty strings, and data freshness problems without requiring users to write checks manually. The article contrasts DQLens with tools like Great Expectations and Soda, which require hand-written check definitions. Supported databases include PostgreSQL, DuckDB, SQLite, and MySQL.

## Key claims
- DQLens can be added to an Airflow DAG in under 5 minutes with no manual check configuration.
- DQLens profiles tables on the first run to establish a baseline and compares subsequent runs against it.
- The tool automatically detects null rate spikes, row count anomalies, schema drift, empty strings, and data freshness issues.
- Only HIGH severity findings (e.g., FK violations, schema changes, major null spikes) fail the Airflow task by default; MEDIUM and LOW findings are logged.
- Great Expectations and Soda require hand-written check definitions (Python suites or YAML), making them time-consuming for large numbers of tables.
- DQLensOperator pushes results to Airflow XCom so downstream tasks can access them.
- DQLens supports PostgreSQL, DuckDB, SQLite, and MySQL databases.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/vahid_saber_d47950be99729/add-data-quality-checks-to-your-airflow-dag-in-5-minutes-7l5>

## Related
[[concepts/apache-airflow|apache-airflow]] · [[concepts/dag|dag]] · [[concepts/dqlens|dqlens]] · [[concepts/dqlensoperator|dqlensoperator]] · [[concepts/bashoperator|bashoperator]] · [[concepts/data-quality-checks|data-quality-checks]] · [[concepts/great-expectations|great-expectations]] · [[concepts/soda|soda]] · [[concepts/xcom|xcom]] · [[concepts/schema-drift|schema-drift]] · [[concepts/data-quality|data-quality]] · [[concepts/warehouse|warehouse]] · [[concepts/pipeline|pipeline]] · [[concepts/airflow|airflow]] · [[concepts/schema|schema]] · [[concepts/python|python]] · [[concepts/yaml|yaml]] · [[episodes/2026-05-08|2026-05-08]]
