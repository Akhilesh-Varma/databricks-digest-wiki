---
type: story
story_id: devto_3759693
episode_date: 2026-05-27
rank: 6
source: devto
url: "https://dev.to/shai_karmani_2521c2f8e837/copy-job-cdc-with-sql-estate-is-now-ga-in-microsoft-fabric-ggb"
title: Copy Job CDC with SQL estate is now GA in Microsoft Fabric
quality_score: 0.933
content_hash: "sha256:1d785d1ebf4297ef57058594806efd74fc5005babf14313bd0e1b9bed36b3bb4"
concepts: [change-data-capture, copy-job, microsoft-fabric-data-factory, fabric-lakehouse, fabric-data-warehouse, azure-sql-database, azure-sql-managed-instance, sap-datasphere, sql-server]
companies: [microsoft, snowflake, google, sap, oracle]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-27 10:19:13.771000"
tags: [story, source/devto]
---

## Summary
Microsoft has announced that Change Data Capture (CDC) support for SQL estate in Copy Job within Microsoft Fabric Data Factory is now generally available. The feature allows data engineering and BI teams to track and replicate only changed records—updates, inserts, and deletes—from operational SQL systems into analytical destinations, rather than performing full data refreshes. Supported GA sources include SQL Server, Azure SQL Database, Azure SQL Managed Instance, and SAP Datasphere, while destinations include those same sources plus Fabric SQL and Snowflake. Additional CDC connectors for Fabric Lakehouse, Google BigQuery, Oracle, and Fabric Data Warehouse are moving through preview. The update positions CDC as a standard Data Factory pattern inside Fabric, reducing the need for custom replication scripts.

## Key claims
- Copy Job CDC with SQL estate in Microsoft Fabric Data Factory is now generally available.
- GA SQL estate sources include SQL Server, Azure SQL Database, Azure SQL Managed Instance, and SAP Datasphere.
- GA destinations include SQL Server, Azure SQL Database, Azure SQL Managed Instance, Fabric SQL, and Snowflake.
- Additional CDC connectors for Fabric Lakehouse table, Google BigQuery, Snowflake, Oracle, SQL database in Fabric, and Fabric Data Warehouse are in preview.
- CDC in Copy Job reduces load on source systems by moving only changed records rather than performing full table refreshes.
- The feature aims to make CDC a standard Data Factory pattern inside Fabric rather than a custom per-team solution.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/shai_karmani_2521c2f8e837/copy-job-cdc-with-sql-estate-is-now-ga-in-microsoft-fabric-ggb>

## Related
[[concepts/change-data-capture|change-data-capture]] · [[concepts/copy-job|copy-job]] · [[concepts/microsoft-fabric-data-factory|microsoft-fabric-data-factory]] · [[concepts/azure-sql-database|azure-sql-database]] · [[concepts/azure-sql-managed-instance|azure-sql-managed-instance]] · [[concepts/sap-datasphere|sap-datasphere]] · [[concepts/sql-server|sql-server]] · [[concepts/data-engineering|data-engineering]] · [[concepts/microsoft-fabric|microsoft-fabric]] · [[concepts/data-warehouse|data-warehouse]] · [[concepts/warehouse|warehouse]] · [[concepts/snowflake|snowflake]] · [[concepts/lakehouse|lakehouse]] · [[concepts/pipeline|pipeline]] · [[concepts/bigquery|bigquery]] · [[concepts/explain|explain]] · [[concepts/azure|azure]] · [[concepts/sql|sql]] · [[concepts/cdc|cdc]] · [[companies/microsoft|Microsoft]] · [[companies/snowflake|Snowflake]] · [[companies/google|Google]] · [[companies/sap|SAP]] · [[companies/oracle|Oracle]] · [[episodes/2026-05-27|2026-05-27]]
