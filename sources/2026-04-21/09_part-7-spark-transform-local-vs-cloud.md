---
type: story
story_id: devto_3529051
episode_date: 2026-04-21
rank: 9
source: devto
url: "https://dev.to/abdelrahman_adnan/part-7-spark-transform-local-vs-cloud-45l7"
title: Part 7 - Spark Transform Local vs Cloud
quality_score: 0.834
content_hash: "sha256:b690f709265146cbae619db6020b08ab50cecb19646d1fd832e70192f89a536f"
concepts: [spark, lakehouse, emr-serverless, parquet, s3]
companies: [amazon]
people: []
extractor_model: llama-3.3-70b-versatile
extracted_at: "2026-04-28 04:04:44.712000"
tags: [story, source/devto]
---

## Summary
This article discusses the transformation job in Spark, which reads raw OpenAQ and weather JSON, flattens nested structures, joins the datasets, and writes parquet into a staging layer partitioned by time. The job can run in two different environments: locally or in the cloud through EMR Serverless. The Spark code expands nested arrays and structs to create a row-per-reading structure. The job explicitly casts columns into stable types before writing parquet to protect downstream consumers from schema drift. The final write uses partitioning to keep the staging layer aligned with the raw layer and makes time-based reads efficient.

## Key claims
- The Spark job reads raw OpenAQ and weather JSON, flattens nested structures, joins the datasets, and writes parquet into a staging layer partitioned by time.
- The job can run in two different environments: locally or in the cloud through EMR Serverless.
- The Spark code expands nested arrays and structs to create a row-per-reading structure.
- The job explicitly casts columns into stable types before writing parquet to protect downstream consumers from schema drift.
- The final write uses partitioning to keep the staging layer aligned with the raw layer and makes time-based reads efficient.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/abdelrahman_adnan/part-7-spark-transform-local-vs-cloud-45l7>

## Related
[[concepts/spark|spark]] · [[concepts/lakehouse|lakehouse]] · [[concepts/emr-serverless|emr-serverless]] · [[concepts/parquet|parquet]] · [[concepts/data-engineering|data-engineering]] · [[concepts/staging-layer|staging-layer]] · [[concepts/schema-drift|schema-drift]] · [[concepts/partitioning|partitioning]] · [[concepts/postgresql|postgresql]] · [[concepts/warehouse|warehouse]] · [[concepts/analytics|analytics]] · [[concepts/postgres|postgres]] · [[concepts/pipeline|pipeline]] · [[concepts/schema|schema]] · [[concepts/json|json]] · [[concepts/dbt|dbt]] · [[concepts/api|api]] · [[companies/amazon|Amazon]] · [[episodes/2026-04-21|2026-04-21]]
