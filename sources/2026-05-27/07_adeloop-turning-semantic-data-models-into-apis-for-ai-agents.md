---
type: story
story_id: devto_3756490
episode_date: 2026-05-27
rank: 7
source: devto
url: "https://dev.to/adeloop/adeloop-turning-semantic-data-models-into-apis-for-ai-agents-212c"
title: Adeloop Turning Semantic Data Models Into APIs for AI Agents
quality_score: 0.926
content_hash: "sha256:f81ce47f9982776117926713675377536f4c517b5d2bfd6ba8d3757ab63251b1"
concepts: [semantic-data-model, agent-console-api, mcp-json-rpc, openapi-3-1, sql-pushdown, semantic-execution-layer, e2b-sandbox, chatgpt-actions, n8n, zapier]
companies: [adeloop, openai, anthropic, snowflake, cursor]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-27 10:19:29.253000"
tags: [story, source/devto]
---

## Summary
Adeloop has launched an Agent Console API that allows AI agents to query business data through governed semantic domains rather than direct database access. The system lets users connect data sources, define semantic domains, publish them, and generate API keys consumable by tools like ChatGPT, Claude, Cursor, n8n, and Zapier. Queries are compiled into safe SQL and pushed down to the warehouse, returning structured JSON without exposing raw SQL to external agents. The platform supports MCP-compatible JSON-RPC endpoints and OpenAPI 3.1 action schemas, enabling deterministic, governed analytics at scale. The company intentionally avoided sandbox Python execution in the main API path, reserving it for async premium analysis jobs.

## Key claims
- Adeloop publishes semantic domains as governed APIs so external AI agents never access raw SQL directly.
- The platform supports connections from ChatGPT, Claude, Cursor, n8n, Zapier, and custom backends via API keys.
- Adeloop compiles semantic metrics and dimensions into safe SQL executed against Postgres, MySQL, Snowflake, and other warehouses.
- The system returns structured JSON along with execution metadata rather than pulling millions of rows into Python.
- Adeloop added MCP-compatible JSON-RPC endpoints and OpenAPI 3.1 action schemas for tool integration.
- The company intentionally excluded E2B sandbox execution from the main API path, reserving Python compute for async premium jobs like forecasting and ML simulations.
- Adeloop positions itself as a semantic execution layer for enterprise data, handling governance, query compilation, federation, caching, and observability.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/adeloop/adeloop-turning-semantic-data-models-into-apis-for-ai-agents-212c>

## Related
[[concepts/semantic-data-model|semantic-data-model]] · [[concepts/agent-console-api|agent-console-api]] · [[concepts/mcp-json-rpc|mcp-json-rpc]] · [[concepts/openapi-3-1|openapi-3-1]] · [[concepts/sql-pushdown|sql-pushdown]] · [[concepts/semantic-execution-layer|semantic-execution-layer]] · [[concepts/anomaly-detection|anomaly-detection]] · [[concepts/vector-search|vector-search]] · [[concepts/observability|observability]] · [[concepts/governance|governance]] · [[concepts/ai-agents|ai-agents]] · [[concepts/warehouse|warehouse]] · [[concepts/snowflake|snowflake]] · [[concepts/analytics|analytics]] · [[concepts/postgres|postgres]] · [[concepts/chatgpt|chatgpt]] · [[concepts/sandbox|sandbox]] · [[concepts/schema|schema]] · [[concepts/cursor|cursor]] · [[concepts/python|python]] · [[concepts/mysql|mysql]] · [[concepts/json|json]] · [[concepts/sql|sql]] · [[concepts/api|api]] · [[concepts/llm|llm]] · [[concepts/mcp|mcp]] · [[concepts/ai|ai]] · [[companies/adeloop|Adeloop]] · [[companies/openai|OpenAI]] · [[companies/anthropic|Anthropic]] · [[companies/snowflake|Snowflake]] · [[companies/cursor|Cursor]] · [[episodes/2026-05-27|2026-05-27]]
