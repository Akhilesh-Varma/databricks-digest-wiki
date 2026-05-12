---
type: story
story_id: community_4accf73d21cc
episode_date: 2026-05-07
rank: 2
source: databricks_community
url: "https://community.databricks.com/t5/technical-blog/three-mcps-one-answer-building-a-data-quality-monitor-on/ba-p/156106"
title: "Three MCPs, One Answer Building a Data Quality Monitor on Databricks Apps"
quality_score: 0.78
content_hash: "sha256:25b07632d76bb6cf5cc5cdf6c43bde2c761392524f04945750d7a399f39001a2"
concepts: [model-context-protocol-mcp, databricks-apps, unity-catalog, openai-agents-sdk, genie, vector-search, spark-declarative-pipelines, ai-gateway, uc-functions, multi-agent-supervisor, lakeflow]
companies: [databricks, openai, slack, jira, salesforce]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-07 10:18:53.179000"
tags: [story, source/databricks-community]
---

## Summary
This article demonstrates building a data quality monitoring chat interface on Databricks using the OpenAI Agents SDK and three Databricks-managed MCP servers. The solution, called 'Data-pipeline monitoring', allows users to ask plain-language questions about data quality and receive grounded answers drawn from pipeline metrics, on-demand checks, and remediation knowledge. The architecture routes queries through a Genie space, Unity Catalog Functions, and a Vector Search index, with Unity Catalog enforcing access control across all tools. The article contrasts two approaches—a managed multi-agent supervisor and a custom Databricks App—ultimately walking through the custom approach for greater control. It covers data preparation, UC function registration, Vector Search indexing, Genie space configuration, agent construction, and deployment.

## Key claims
- The demo builds a Databricks App chat interface backed by an AI agent that orchestrates three Databricks-managed MCP servers to answer data quality questions.
- Unity Catalog is the sole access-control plane, ensuring the agent can only access data the app's identity is permitted to see.
- The Model Context Protocol (MCP) allows AI agents to discover and invoke tools at runtime rather than having tools hardcoded into prompt templates.
- Databricks supports three MCP server flavors: managed MCP servers, external MCP servers registered via AI Gateway, and custom MCP servers hosted as Databricks Apps.
- The custom Databricks Apps approach using the OpenAI Agents SDK provides full control over system prompts, tool-calling logic, and workflow, at the cost of more development effort.
- The agent uses a Genie space for pipeline monitoring metrics, UC Functions for on-demand data quality checks, and a Vector Search index over past incidents and runbooks for remediation knowledge.
- Databricks system tables such as system.access.audit, system.lakeflow.jobs, and system.data_quality are used for data preparation in the demo.

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/technical-blog/three-mcps-one-answer-building-a-data-quality-monitor-on/ba-p/156106>

## Related
[[concepts/model-context-protocol-mcp|model-context-protocol-mcp]] · [[concepts/databricks-apps|databricks-apps]] · [[concepts/unity-catalog|unity-catalog]] · [[concepts/openai-agents-sdk|openai-agents-sdk]] · [[concepts/genie|genie]] · [[concepts/vector-search|vector-search]] · [[concepts/spark-declarative-pipelines|spark-declarative-pipelines]] · [[concepts/ai-gateway|ai-gateway]] · [[concepts/uc-functions|uc-functions]] · [[concepts/multi-agent-supervisor|multi-agent-supervisor]] · [[concepts/declarative-pipelines|declarative-pipelines]] · [[concepts/knowledge-assistant|knowledge-assistant]] · [[concepts/supervisor-agent|supervisor-agent]] · [[concepts/data-quality|data-quality]] · [[concepts/genie-spaces|genie-spaces]] · [[concepts/agent-bricks|agent-bricks]] · [[concepts/mcp-servers|mcp-servers]] · [[concepts/genie-space|genie-space]] · [[concepts/mcp-server|mcp-server]] · [[concepts/databricks|databricks]] · [[concepts/ai-agents|ai-agents]] · [[concepts/pipeline|pipeline]] · [[concepts/spark|spark]] · [[concepts/sdk|sdk]] · [[concepts/mcp|mcp]] · [[concepts/ai|ai]] · [[concepts/uc|uc]] · [[companies/databricks|Databricks]] · [[companies/openai|OpenAI]] · [[companies/slack|Slack]] · [[companies/jira|Jira]] · [[companies/salesforce|Salesforce]] · [[episodes/2026-05-07|2026-05-07]]
