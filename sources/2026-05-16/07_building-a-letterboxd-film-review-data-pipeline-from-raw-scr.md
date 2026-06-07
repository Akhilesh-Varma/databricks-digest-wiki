---
type: story
story_id: devto_3678073
episode_date: 2026-05-16
rank: 7
source: devto
url: "https://dev.to/can_ylmaz_da7b70586976b3/building-a-letterboxd-film-review-data-pipeline-from-raw-scrape-to-first-insight-4bo6"
title: Building a Letterboxd Film Review data pipeline from raw scrape to first insight
quality_score: 0.848
content_hash: "sha256:33849e6485d0282a65f683455f87952824e7d285797bc9a2892e36b524bea92b"
concepts: [letterboxd-scraper, elt-pipeline, object-storage, duckdb, bigquery, snowflake, staging-table, incremental-scraping, schema-drift, sentiment-tracking]
companies: [letterboxd, amazon-web-services, google-cloud, cloudflare, snowflake]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-16 10:20:02.603000"
tags: [story, source/devto]
---

## Summary
The article describes building a data pipeline for Letterboxd film review data, from scraping raw records to loading them into a warehouse for analysis. The author outlines a four-stage pipeline: extract, land, transform, and serve. Key design decisions include using daily incremental scraping due to moderate rate-limiting, storing raw JSON in object storage partitioned by date, and using a columnar warehouse for staging and curated layers. Operational concerns such as schema drift, duplicate records, and silent failures are highlighted, with record-count assertions recommended as an early warning system.

## Key claims
- Letterboxd uses list-based pagination and moderate rate-limiting, making it suitable for daily incremental jobs rather than streaming.
- Raw scraped records should be stored as JSON in object storage partitioned by date to enable history replay without re-scraping.
- The pipeline follows four stages: Extract, Land, Transform, and Serve.
- Schema drift, duplicate records from overlapping scrape windows, and quietly failing runs are the three main operational risks for this type of pipeline.
- Record-count assertions should be wired up early to detect upstream site changes.
- Recommended tooling includes S3, GCS, or R2 for raw landing zones and BigQuery, Snowflake, or DuckDB for staging and curated layers.
- Deeply nested or free-text fields should be stored in a TEXT column rather than normalized during warehouse ingestion.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/can_ylmaz_da7b70586976b3/building-a-letterboxd-film-review-data-pipeline-from-raw-scrape-to-first-insight-4bo6>

## Related
[[concepts/letterboxd-scraper|letterboxd-scraper]] · [[concepts/elt-pipeline|elt-pipeline]] · [[concepts/object-storage|object-storage]] · [[concepts/duckdb|duckdb]] · [[concepts/staging-table|staging-table]] · [[concepts/incremental-scraping|incremental-scraping]] · [[concepts/schema-drift|schema-drift]] · [[concepts/warehouse|warehouse]] · [[concepts/streaming|streaming]] · [[concepts/pipeline|pipeline]] · [[concepts/schema|schema]] · [[concepts/python|python]] · [[concepts/json|json]] · [[concepts/gcs|gcs]] · [[concepts/api|api]] · [[concepts/s3|s3]] · [[companies/letterboxd|Letterboxd]] · [[companies/amazon-web-services|Amazon Web Services]] · [[companies/google-cloud|Google Cloud]] · [[companies/cloudflare|Cloudflare]] · [[companies/snowflake|Snowflake]] · [[episodes/2026-05-16|2026-05-16]]
