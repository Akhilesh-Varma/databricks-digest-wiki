---
type: story
story_id: hn_48309986
episode_date: 2026-05-29
rank: 2
source: hacker_news
url: "https://github.com/Kaelio/ktx"
title: Show HN Ktx Open-source executable context layer for data agents
quality_score: 0.839
content_hash: "sha256:d3da6fa611e630b3a0e8cf22dd50d447803e4bd239d35b7f010cd982f4ef78dc"
concepts: [ktx, semantic-layer, dbt, metricflow, lookml, join-fanout, chasm-join, claude-code, codex, apache-2-0-license]
companies: [kaelio, anthropic, openai, google, snowflake, looker, metabase, notion]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-29 10:17:36.735000"
tags: [story, source/hacker-news]
---

## Summary
Ktx is an open-source executable context layer designed to make AI data agents more reliable when querying data warehouses. It addresses common agent failure modes such as stale columns, join fanout, and missing attribution logic by splitting context into Markdown wiki pages for business knowledge and YAML files for queryable definitions of tables, joins, measures, and dimensions. When an agent needs a metric, it requests it from ktx rather than writing raw SQL itself; ktx's planner then handles join path selection, grain metadata, and SQL compilation. The project is released under Apache 2.0 and supports ingestion from warehouses like BigQuery, Snowflake, and Postgres, as well as modeling tools like dbt and BI tools like Looker and Metabase.

## Key claims
- Ktx is an open-source executable context layer that improves accuracy of AI agents operating on data warehouses.
- Common agent failure modes include using deprecated columns, join fanout errors, and incorrect attribution logic.
- Ktx splits context into Markdown wiki pages for unstructured business knowledge and YAML files for queryable table/metric definitions.
- Agents query ktx for measures, dimensions, and filters instead of writing full SQL themselves, reducing incorrect assumptions.
- Ktx's planner selects join paths, applies grain and relationship metadata, and catches issues like join fanout and chasm joins.
- Ktx supports ingestion from BigQuery, Snowflake, Postgres, dbt, MetricFlow, LookML, Looker, Metabase, and Notion.
- The project is licensed under Apache 2.0 and can be installed via npm.

## Source
- **Origin:** hacker_news
- **URL:** <https://github.com/Kaelio/ktx>

## Related
[[concepts/ktx|ktx]] · [[concepts/semantic-layer|semantic-layer]] · [[concepts/dbt|dbt]] · [[concepts/metricflow|metricflow]] · [[concepts/lookml|lookml]] · [[concepts/join-fanout|join-fanout]] · [[concepts/claude-code|claude-code]] · [[concepts/codex|codex]] · [[concepts/knowledge-base|knowledge-base]] · [[concepts/data-warehouse|data-warehouse]] · [[concepts/context-layer|context-layer]] · [[concepts/data-agents|data-agents]] · [[concepts/data-stack|data-stack]] · [[concepts/warehouses|warehouses]] · [[concepts/warehouse|warehouse]] · [[concepts/snowflake|snowflake]] · [[concepts/analytics|analytics]] · [[concepts/postgres|postgres]] · [[concepts/bigquery|bigquery]] · [[concepts/bi-tools|bi-tools]] · [[concepts/markdown|markdown]] · [[concepts/metadata|metadata]] · [[concepts/claude|claude]] · [[concepts/notion|notion]] · [[concepts/sql|sql]] · [[companies/kaelio|Kaelio]] · [[companies/anthropic|Anthropic]] · [[companies/openai|OpenAI]] · [[companies/google|Google]] · [[companies/snowflake|Snowflake]] · [[companies/looker|Looker]] · [[companies/metabase|Metabase]] · [[companies/notion|Notion]] · [[episodes/2026-05-29|2026-05-29]]
