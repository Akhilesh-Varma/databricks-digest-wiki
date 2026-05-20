---
type: story
story_id: community_c5e238082e99
episode_date: 2026-04-13
rank: 2
source: databricks_community
url: "https://community.databricks.com/t5/technical-blog/from-19-hours-to-80-milliseconds-a-geospatial-cheesecake/ba-p/153693"
title: From 19 Hours to 80 Milliseconds A Geospatial Cheesecake
quality_score: 0.78
content_hash: "sha256:d6af8577e5874f5791da368a13c31ffb45dae0e484166c2d7e8e68af9f052b3f"
concepts: [lakebase, point-in-polygon-query, gist-index, geopackage, delta-lake, apache-spark, photon, postgis, mapserver, lakehouse, spatial-join, etl-pipeline]
companies: [databricks, uk-environment-agency]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:21:44.169000"
tags: [story, source/databricks-community]
---

## Summary
A Databricks community blog post describes how geospatial point-in-polygon queries against national flood risk datasets took up to 19 hours in a standard SQL warehouse due to the absence of spatial indexes. The author proposes replacing a traditional three-system architecture (Lakehouse batch processing, a separate PostGIS/Postgres instance, and a GIS tile server) with a unified solution built on Databricks Lakebase, which provides GIST index support for real-time spatial queries. By leveraging Lakebase alongside Delta Lake and Spark, query times were reduced from 19 hours to approximately 80 milliseconds. The article uses an extended cheesecake metaphor to illustrate the complexity of multi-system geospatial pipelines and the elegance of consolidating them into a single governed platform. The use case centers on the UK Environment Agency's flood risk data for England.

## Key claims
- A single point-in-polygon query against a national geospatial dataset in a SQL warehouse without spatial indexes took up to 19 hours.
- The traditional architecture for real-time geospatial serving required three separate systems: a Lakehouse for batch processing, a Postgres/PostGIS instance for serving, and a GIS server for tile serving.
- Databricks Lakebase provides GIST index support, enabling real-time spatial queries at approximately 80 milliseconds.
- SQL warehouses with Photon have improved spatial join optimisations but are not suited for real-time point-in-polygon serving against millions of complex geometries.
- Consolidating geospatial workloads into Lakebase eliminates separate governance, infrastructure, and ETL costs associated with multi-system architectures.
- The demo used UK Environment Agency flood risk data covering all of England as the geospatial dataset.

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/technical-blog/from-19-hours-to-80-milliseconds-a-geospatial-cheesecake/ba-p/153693>

## Related
[[concepts/lakebase|lakebase]] · [[concepts/point-in-polygon-query|point-in-polygon-query]] · [[concepts/gist-index|gist-index]] · [[concepts/geopackage|geopackage]] · [[concepts/delta-lake|delta-lake]] · [[concepts/apache-spark|apache-spark]] · [[concepts/photon|photon]] · [[concepts/postgis|postgis]] · [[concepts/lakehouse|lakehouse]] · [[concepts/spatial-join|spatial-join]] · [[concepts/batch-processing|batch-processing]] · [[concepts/streaming-data|streaming-data]] · [[concepts/sql-warehouse|sql-warehouse]] · [[concepts/etl-pipelines|etl-pipelines]] · [[concepts/governance|governance]] · [[concepts/databricks|databricks]] · [[concepts/ai-agents|ai-agents]] · [[concepts/warehouse|warehouse]] · [[concepts/analytics|analytics]] · [[concepts/postgres|postgres]] · [[concepts/delta|delta]] · [[concepts/spark|spark]] · [[concepts/sql|sql]] · [[concepts/etl|etl]] · [[concepts/ai|ai]] · [[companies/databricks|Databricks]] · [[companies/uk-environment-agency|UK Environment Agency]] · [[episodes/2026-04-13|2026-04-13]]
