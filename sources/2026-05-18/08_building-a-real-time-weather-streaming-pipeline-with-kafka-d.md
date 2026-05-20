---
type: story
story_id: devto_3689046
episode_date: 2026-05-18
rank: 8
source: devto
url: "https://dev.to/damaac/-building-a-real-time-weather-streaming-pipeline-with-kafka-docker-python-3e7b"
title: "Building a Real-Time Weather Streaming Pipeline with Kafka, Docker Python"
quality_score: 0.93
content_hash: "sha256:0749f282b58301866a6f498f1555c6865af146d5a7edc61fc48d94b61398a9ef"
concepts: [apache-kafka, docker-compose, event-driven-architecture, etl-pipeline, publish-subscribe-model, postgresql, confluent-platform, rapidapi]
companies: [confluent]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-18 10:20:29.477000"
tags: [story, source/devto]
---

## Summary
This article describes building a real-time weather data streaming pipeline using Apache Kafka, Docker, and Python. A producer script continuously fetches live weather metrics for nine international cities via RapidAPI and publishes the payloads to a Kafka topic. A consumer script implements an ETL pattern, decoding and flattening the nested JSON data before persisting it into a PostgreSQL database. Docker Compose is used to containerize the Confluent Kafka platform, decoupling infrastructure from application logic. The architecture follows an Event-Driven, publish-subscribe model to avoid tight coupling between data sourcing and storage.

## Key claims
- The pipeline uses Apache Kafka as a message broker to decouple data ingestion from data transformation and storage.
- Docker Compose is used to containerize the entire Confluent Kafka platform stack, exposing Kafka on a host port.
- A Python producer script fetches real-time weather data for nine cities via RapidAPI and publishes JSON payloads to a Kafka topic.
- A Python consumer script implements a full ETL pattern, flattening nested API JSON structures and loading records into PostgreSQL.
- The architecture follows an Event-Driven Architecture (EDA) with a publish-subscribe model to improve resilience and scalability.
- Inline JSON serialization is handled via a lambda function passed directly into the Kafka producer constructor.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/damaac/-building-a-real-time-weather-streaming-pipeline-with-kafka-docker-python-3e7b>

## Related
[[concepts/apache-kafka|apache-kafka]] · [[concepts/docker-compose|docker-compose]] · [[concepts/event-driven-architecture|event-driven-architecture]] · [[concepts/etl-pipeline|etl-pipeline]] · [[concepts/publish-subscribe-model|publish-subscribe-model]] · [[concepts/postgresql|postgresql]] · [[concepts/confluent-platform|confluent-platform]] · [[concepts/data-engineering|data-engineering]] · [[concepts/workflows|workflows]] · [[concepts/warehouse|warehouse]] · [[concepts/workspace|workspace]] · [[concepts/pipeline|pipeline]] · [[concepts/docker|docker]] · [[concepts/python|python]] · [[concepts/kafka|kafka]] · [[concepts/json|json]] · [[concepts/cli|cli]] · [[concepts/api|api]] · [[concepts/etl|etl]] · [[companies/confluent|Confluent]] · [[episodes/2026-05-18|2026-05-18]]
