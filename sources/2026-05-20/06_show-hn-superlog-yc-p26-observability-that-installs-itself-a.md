---
type: story
story_id: hn_48195021
episode_date: 2026-05-20
rank: 6
source: hacker_news
url: "https://superlog.sh/"
title: Show HN Superlog YC P26 Observability that installs itself and fixes bugs
quality_score: 0.731
content_hash: "sha256:0a9e515a9aa8135db2fbe49fb968fab9dc90c5ca6599fba7d21aac69d123d0c8"
concepts: [opentelemetry, observability, model-context-protocol-mcp, alert-fatigue, error-fingerprinting, claude-code, distributed-tracing]
companies: [superlog, y-combinator, datadog, sentry, grafana, dash0, amazon-web-services, anthropic]
people: [nico, arseniy]
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-20 10:22:42.818000"
tags: [story, source/hacker-news]
---

## Summary
Superlog is a self-installing, self-healing observability platform founded by Nico and Arseniy (YC P26) that automatically instruments codebases with OpenTelemetry and uses an AI agent to investigate errors and open pull requests. The tool aims to eliminate manual observability setup by running a daily wizard that scans repositories and adds structured logs, traces, and metrics. It addresses alert fatigue by fingerprinting and grouping errors into single incidents with clear summaries and severity scores. When an incident occurs, the agent either produces a tested PR or posts findings and pulls in relevant engineers based on documentation and Slack history. Superlog is vendor-neutral, preserving all telemetry data independently of the platform.

## Key claims
- Superlog automatically instruments codebases with OpenTelemetry SDKs via a wizard that runs daily to keep telemetry up to date.
- An AI agent investigates errors and opens a single pull request per incident, or posts findings for the engineering team if context is insufficient.
- Errors are fingerprinted and grouped into incidents to reduce duplicate alerts and alert fatigue.
- Superlog is MCP-native and agent-first, requiring zero manual setup from users.
- The platform tracks LLM and upstream costs by callsite, tenant, and model.
- Telemetry installed by Superlog is vendor-neutral, meaning users retain all logs, metrics, and traces.
- Co-founder Arseniy previously worked at Datadog handling production incidents, informing the product's design.

## Source
- **Origin:** hacker_news
- **URL:** <https://superlog.sh/>

## Related
[[concepts/opentelemetry|opentelemetry]] · [[concepts/observability|observability]] · [[concepts/model-context-protocol-mcp|model-context-protocol-mcp]] · [[concepts/alert-fatigue|alert-fatigue]] · [[concepts/error-fingerprinting|error-fingerprinting]] · [[concepts/telemetry|telemetry]] · [[concepts/grafana|grafana]] · [[concepts/claude|claude]] · [[concepts/merge|merge]] · [[concepts/aws|aws]] · [[concepts/llm|llm]] · [[concepts/mcp|mcp]] · [[companies/superlog|Superlog]] · [[companies/y-combinator|Y Combinator]] · [[companies/datadog|Datadog]] · [[companies/sentry|Sentry]] · [[companies/grafana|Grafana]] · [[companies/dash0|Dash0]] · [[companies/amazon-web-services|Amazon Web Services]] · [[companies/anthropic|Anthropic]] · [[people/nico|Nico]] · [[people/arseniy|Arseniy]] · [[episodes/2026-05-20|2026-05-20]]
