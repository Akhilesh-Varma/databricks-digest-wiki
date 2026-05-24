---
type: story
story_id: devto_3508275
episode_date: 2026-04-16
rank: 8
source: devto
url: "https://dev.to/mfarizala/how-i-built-an-end-to-end-data-engineering-pipeline-for-hong-kongs-public-transport-network-1bkl"
title: "How I Built an End-to-End Data Engineering Pipeline for Hong Kong's Public Transport Network"
quality_score: 0.857
content_hash: "sha256:aece700fba11cb4400f40d1cbffb402285c0819782cebc2f96fc27eaef2ff882"
concepts: [gtfs, bruin, opentofu, bigquery, redpanda-cloud, streamlit, cloud-run, github-actions, workload-identity-federation, cloud-scheduler, google-cloud-storage, infrastructure-as-code, batch-pipeline, streaming-pipeline]
companies: [google, redpanda, mtr-corporation]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:14:06.799000"
tags: [story, source/devto]
---

## Summary
A data engineer built an end-to-end pipeline called HK Transit Pulse to ingest, transform, and visualise Hong Kong's public transport data from GTFS feeds, MTR open data CSVs, and real-time schedule APIs. The pipeline runs a daily batch process and a streaming layer that updates every minute, all hosted on GCP's free tier. The stack includes Bruin for orchestration, OpenTofu for infrastructure-as-code, BigQuery as the data warehouse, Redpanda Cloud for Kafka-compatible streaming, and Streamlit for dashboarding. The project answers questions about stop traffic, service patterns, and live MTR train activity. CI/CD is handled via GitHub Actions with Workload Identity Federation for keyless authentication.

## Key claims
- The pipeline ingests data from GTFS feeds, MTR open data CSVs, and real-time schedule APIs scattered across government portals.
- The batch pipeline runs daily while the streaming layer updates every minute.
- The entire stack runs on GCP free tier using services including Cloud Run, BigQuery, and Cloud Scheduler.
- Bruin is used as the orchestration tool, enabling unified Python and SQL pipelines in a single tool.
- Redpanda Cloud serves as a Kafka-compatible streaming layer without requiring ZooKeeper.
- OpenTofu, the open-source Terraform fork, is used for reproducible infrastructure-as-code.
- GitHub Actions with Workload Identity Federation provides keyless authentication for CI/CD.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/mfarizala/how-i-built-an-end-to-end-data-engineering-pipeline-for-hong-kongs-public-transport-network-1bkl>

## Related
[[concepts/gtfs|gtfs]] · [[concepts/bruin|bruin]] · [[concepts/opentofu|opentofu]] · [[concepts/bigquery|bigquery]] · [[concepts/redpanda-cloud|redpanda-cloud]] · [[concepts/streamlit|streamlit]] · [[concepts/cloud-run|cloud-run]] · [[concepts/github-actions|github-actions]] · [[concepts/workload-identity-federation|workload-identity-federation]] · [[concepts/cloud-scheduler|cloud-scheduler]] · [[concepts/google-cloud-storage|google-cloud-storage]] · [[concepts/batch-pipeline|batch-pipeline]] · [[concepts/streaming-pipeline|streaming-pipeline]] · [[concepts/data-engineering-pipeline|data-engineering-pipeline]] · [[concepts/data-engineering|data-engineering]] · [[concepts/data-warehouse|data-warehouse]] · [[concepts/cloud-run-jobs|cloud-run-jobs]] · [[concepts/orchestration|orchestration]] · [[concepts/google-cloud|google-cloud]] · [[concepts/zookeeper|zookeeper]] · [[concepts/warehouse|warehouse]] · [[concepts/terraform|terraform]] · [[concepts/data-lake|data-lake]] · [[concepts/pipeline|pipeline]] · [[concepts/redpanda|redpanda]] · [[concepts/python|python]] · [[concepts/kafka|kafka]] · [[concepts/sql|sql]] · [[companies/google|Google]] · [[companies/redpanda|Redpanda]] · [[companies/mtr-corporation|MTR Corporation]] · [[episodes/2026-04-16|2026-04-16]]
