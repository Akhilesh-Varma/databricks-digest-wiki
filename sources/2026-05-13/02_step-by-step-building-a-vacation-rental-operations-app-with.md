---
type: story
story_id: community_beaf997b496f
episode_date: 2026-05-13
rank: 2
source: databricks_community
url: "https://community.databricks.com/t5/technical-blog/step-by-step-building-a-vacation-rental-operations-app-with/ba-p/155833"
title: Step-by-Step Building a Vacation Rental Operations App with AppKit
quality_score: 0.78
content_hash: "sha256:346fb65363c359dc36711d48d0236893fa9a9f00ee96ab36b0a1c72c801a37c5"
concepts: [appkit, sql-warehouse, lakebase, genie, databricks-apps, unity-catalog, databricks-cli, samples-wanderbricks]
companies: [databricks, anthropic, github]
people: [james-broadhead, evan-pandya]
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-13 10:21:20.315000"
tags: [story, source/databricks-community]
---

## Summary
This article walks through building a vacation rental operations app using Databricks AppKit, leveraging the samples.wanderbricks dataset included in every Databricks workspace. The app features four capabilities: revenue analytics from a SQL Warehouse, a booking manager, user actions persisted in Lakebase (a serverless Postgres database), and a conversational AI panel powered by Genie. The architecture separates reads (SQL Warehouse) from writes (Lakebase), avoiding data duplication. The post also describes a fast-path approach using AI coding agents like Cursor, Copilot, or Claude Code to scaffold and deploy the entire app automatically.

## Key claims
- The app uses SQL Warehouse for all read operations including revenue aggregations and booking lookups against samples.wanderbricks.
- Lakebase, a fully-managed serverless Postgres database, handles all write operations such as booking flags and notes.
- Genie provides conversational AI over warehouse data, allowing users to ask questions in plain English.
- An AI coding agent can be used to detect the workspace, scaffold the project, wire up plugins, and deploy the app without manual steps.
- The samples.wanderbricks dataset ships with every Databricks workspace and contains 16 tables covering bookings, users, properties, payments, reviews, and more.
- The app goes beyond standard dashboards by enabling users to act on data, such as flagging suspicious bookings and leaving shift notes.

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/technical-blog/step-by-step-building-a-vacation-rental-operations-app-with/ba-p/155833>

## Related
[[concepts/appkit|appkit]] · [[concepts/sql-warehouse|sql-warehouse]] · [[concepts/lakebase|lakebase]] · [[concepts/genie|genie]] · [[concepts/databricks-apps|databricks-apps]] · [[concepts/databricks-cli|databricks-cli]] · [[concepts/samples-wanderbricks|samples-wanderbricks]] · [[concepts/databricks-workspace|databricks-workspace]] · [[concepts/sql-warehouses|sql-warehouses]] · [[concepts/claude-code|claude-code]] · [[concepts/genie-space|genie-space]] · [[concepts/genie-code|genie-code]] · [[concepts/databricks|databricks]] · [[concepts/warehouses|warehouses]] · [[concepts/warehouse|warehouse]] · [[concepts/workspace|workspace]] · [[concepts/analytics|analytics]] · [[concepts/postgres|postgres]] · [[concepts/node-js|node-js]] · [[concepts/cursor|cursor]] · [[concepts/react|react]] · [[concepts/rest|rest]] · [[concepts/sql|sql]] · [[concepts/cli|cli]] · [[concepts/git|git]] · [[concepts/ai|ai]] · [[concepts/uc|uc]] · [[companies/databricks|Databricks]] · [[companies/anthropic|Anthropic]] · [[companies/github|GitHub]] · [[people/james-broadhead|James Broadhead]] · [[people/evan-pandya|Evan Pandya]] · [[episodes/2026-05-13|2026-05-13]]
