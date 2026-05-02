---
type: story
story_id: community_a9e9454a5418
episode_date: 2026-04-26
rank: 2
source: databricks_community
url: "https://community.databricks.com/t5/announcements/customer-story-toyota-uses-zerobus-ingest-for-real-time-factory/td-p/155358"
title: CUSTOMER STORY Toyota uses Zerobus Ingest for real-time factory data
quality_score: 0.66
content_hash: "sha256:5045e686c1f9a7fef0e515b8b511c96740d06b94a7468a6aeb22954f24f5974a"
concepts: [zerobus-ingest, databricks, unity-catalog, soracom, telemetry]
companies: [toyota, databricks, soracom]
people: [kento-izumi]
extractor_model: gemini-2.5-flash-lite
extracted_at: "2026-04-28 03:22:38.546000"
tags: [story, source/databricks-community]
---

## Summary
Toyota is leveraging Zerobus Ingest on the Databricks platform to process factory telemetry data in near real-time. This implementation has drastically reduced data latency by 98%, from 4.5 seconds to 0.1 seconds, enabling faster detection of critical issues like overheating conditions. The new architecture, which streams data directly from factory equipment via Soracom and Zerobus Ingest into Databricks, improves operational efficiency, worker safety, and supports Toyota's carbon-neutrality goals. Furthermore, the integration with Unity Catalog and Toyota's Vista platform ensures the data is governed, secured, and ready for advanced analytics and AI applications.

## Key claims
- Toyota is using Zerobus Ingest on Databricks to stream factory telemetry data in near real-time.
- Data latency has been reduced by 98%, from 4.5 seconds to 0.1 seconds.
- The reduced latency allows for the detection of overheating conditions in minutes instead of hours.
- The new architecture simplifies data streaming by flowing telemetry directly from factory equipment via Soracom and Zerobus Ingest into Databricks.
- Unity Catalog and Toyota's Vista platform are used to govern, secure, and prepare the telemetry data for analytics and AI.
- The real-time data processing contributes to improved worker safety and operational efficiency.

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/announcements/customer-story-toyota-uses-zerobus-ingest-for-real-time-factory/td-p/155358>

## Related
[[concepts/zerobus-ingest|zerobus-ingest]] · [[concepts/databricks|databricks]] · [[concepts/unity-catalog|unity-catalog]] · [[concepts/anomaly-detection|anomaly-detection]] · [[concepts/analytics|analytics]] · [[concepts/ai|ai]] · [[companies/toyota|Toyota]] · [[companies/databricks|Databricks]] · [[companies/soracom|Soracom]] · [[people/kento-izumi|Kento Izumi]] · [[episodes/2026-04-26|2026-04-26]]
