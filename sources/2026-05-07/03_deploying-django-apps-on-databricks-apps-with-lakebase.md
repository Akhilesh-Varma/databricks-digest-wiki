---
type: story
story_id: community_a7a35e37bc71
episode_date: 2026-05-07
rank: 3
source: databricks_community
url: "https://community.databricks.com/t5/technical-blog/deploying-django-apps-on-databricks-apps-with-lakebase/ba-p/155450"
title: Deploying Django apps on Databricks Apps with Lakebase
quality_score: 0.78
content_hash: "sha256:b64f3a4b007e1422ee7f374a212ed7e06ce699d1a8f1982e91c6e1d7b8398bb9"
concepts: [databricks-apps, lakebase, django-orm, django, postgresql, oauth-token, app-authorization, databricks-sdk, copy-on-write-branching, flask, streamlit, gradio, dash]
companies: [databricks]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-07 10:19:07.215000"
tags: [story, source/databricks-community]
---

## Summary
This article explains how to deploy Django web applications on Databricks Apps and connect them to Lakebase, Databricks' managed PostgreSQL offering. It highlights the synergy between Django's ORM and Lakebase's architecture, which separates storage from compute and supports features like scale-to-zero, branching, and instant restore. The post demonstrates secure connectivity using app authorization via the Databricks SDK, which mints short-lived OAuth tokens without requiring manual management of service principal credentials. A copy-on-write branching feature in Lakebase is highlighted as particularly useful for safely testing Django migrations. A GitHub template is provided to help developers get started quickly.

## Key claims
- Django applications can be deployed on Databricks Apps alongside other Python frameworks like Flask, Streamlit, Dash, and Gradio.
- Lakebase is Databricks' managed PostgreSQL offering with an architecture that separates storage from compute.
- Lakebase supports scale-to-zero, copy-on-write branching, and instant restore capabilities.
- Databricks Apps uses app authorization via a dedicated service principal, eliminating the need to manage client IDs or secrets manually.
- The Databricks SDK's WorkspaceClient mints short-lived, down-scoped OAuth tokens that are cached and refreshed 30 seconds before expiry.
- Lakebase's copy-on-write branching allows developers to test Django model schema migrations against real data in isolated, disposable Postgres environments.
- An extensible GitHub template is provided for deploying Django on Databricks Apps with Lakebase.

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/technical-blog/deploying-django-apps-on-databricks-apps-with-lakebase/ba-p/155450>

## Related
[[concepts/databricks-apps|databricks-apps]] · [[concepts/lakebase|lakebase]] · [[concepts/django-orm|django-orm]] · [[concepts/django|django]] · [[concepts/postgresql|postgresql]] · [[concepts/oauth-token|oauth-token]] · [[concepts/app-authorization|app-authorization]] · [[concepts/databricks-sdk|databricks-sdk]] · [[concepts/copy-on-write-branching|copy-on-write-branching]] · [[concepts/lakebase-postgresql|lakebase-postgresql]] · [[concepts/databricks-platform|databricks-platform]] · [[concepts/service-principal|service-principal]] · [[concepts/app-development|app-development]] · [[concepts/copy-on-write|copy-on-write]] · [[concepts/governance|governance]] · [[concepts/databricks|databricks]] · [[concepts/protobuf|protobuf]] · [[concepts/postgres|postgres]] · [[concepts/schema|schema]] · [[concepts/python|python]] · [[concepts/oauth|oauth]] · [[concepts/sdk|sdk]] · [[companies/databricks|Databricks]] · [[episodes/2026-05-07|2026-05-07]]
