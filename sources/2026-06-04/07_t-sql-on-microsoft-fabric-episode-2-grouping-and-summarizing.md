---
type: story
story_id: devto_3816031
episode_date: 2026-06-04
rank: 7
source: devto
url: "https://dev.to/lamkhac/t-sql-on-microsoft-fabric-episode-2-grouping-and-summarizing-data-with-group-by-and-aggregate-4bjm"
title: T-SQL on Microsoft Fabric - Episode 2 Grouping and Summarizing Data with GROUP BY and Aggregate Functions
quality_score: 0.817
content_hash: "sha256:4a782ad9083c0609478163e727314bdcf659294163daf3b34346877eb0d3e280"
concepts: [t-sql, microsoft-fabric, group-by, having, aggregate-functions, microsoft-fabric-warehouse, power-bi]
companies: [microsoft]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-06-04 10:22:42.935000"
tags: [story, source/devto]
---

## Summary
This tutorial article is the second episode in a series covering T-SQL on Microsoft Fabric, focusing on grouping and summarizing data. It explains how to use aggregate functions such as SUM, COUNT, AVG, MIN, and MAX in T-SQL queries. The article demonstrates how GROUP BY organizes rows into groups before aggregation, and how HAVING filters grouped results after aggregation, contrasting it with WHERE which filters rows before grouping. Practical examples are provided using a sample table in a Microsoft Fabric Warehouse, culminating in a real-world product revenue summary for reporting or dashboards.

## Key claims
- T-SQL aggregate functions (SUM, COUNT, AVG, MIN, MAX) are among the most frequently used SQL features in Data Warehouses and Power BI models.
- GROUP BY organizes rows into groups before aggregate functions are applied.
- HAVING filters grouped results after aggregation has been applied, unlike WHERE which filters rows before grouping.
- COUNT can be used to count total rows or distinct values such as unique customers.
- Microsoft Fabric Warehouse supports T-SQL for building product revenue summaries for reporting and dashboards.
- The article references official Microsoft Learn documentation for each aggregate function and GROUP BY/HAVING clauses.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/lamkhac/t-sql-on-microsoft-fabric-episode-2-grouping-and-summarizing-data-with-group-by-and-aggregate-4bjm>

## Related
[[concepts/t-sql|t-sql]] · [[concepts/microsoft-fabric|microsoft-fabric]] · [[concepts/group-by|group-by]] · [[concepts/having|having]] · [[concepts/aggregate-functions|aggregate-functions]] · [[concepts/microsoft-fabric-warehouse|microsoft-fabric-warehouse]] · [[concepts/data-warehouses|data-warehouses]] · [[concepts/data-warehouse|data-warehouse]] · [[concepts/warehouses|warehouses]] · [[concepts/warehouse|warehouse]] · [[concepts/schema|schema]] · [[concepts/sql|sql]] · [[companies/microsoft|Microsoft]] · [[episodes/2026-06-04|2026-06-04]]
