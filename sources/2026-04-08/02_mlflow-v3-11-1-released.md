---
type: story
story_id: github_release_mlflow_mlflow_306406312
episode_date: 2026-04-08
rank: 2
source: github_releases
url: "https://github.com/mlflow/mlflow/releases/tag/v3.11.1"
title: MLflow v3.11.1 released
quality_score: 0.722
content_hash: "sha256:5a57d208ae4a5fb5159841ed114fc2211c428b71e9c1631069d9b3ef14238db4"
concepts: [mlflow, ai-gateway, opentelemetry-genai-semantic-conventions, otlp, trace-graph-view, budget-policies]
companies: [mlflow-oss-project]
people: [tome-hirata, joel-robin]
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:32:26.778000"
tags: [story, source/github-releases]
---

## Summary
MLflow version 3.11.1 introduces several major features including automatic AI-powered issue identification in agent traces, configurable budget alerts and spending limits for the AI Gateway, and an interactive graph view for visualizing trace hierarchies. The release also adds native support for OpenTelemetry GenAI Semantic Conventions, enabling seamless trace export to OTel-compatible observability platforms. These improvements focus on enhancing observability, cost control, and debugging capabilities for AI and machine learning workflows.

## Key claims
- MLflow 3.11.1 introduces a 'Detect Issues' button that uses AI to automatically identify quality issues in agent traces across correctness, safety, and performance categories.
- The new AI Gateway budget policies allow users to set spending limits by daily, weekly, or monthly time windows and block requests automatically when limits are reached.
- A new Trace Graph View provides an interactive visual representation of multi-level trace hierarchies and parent-child relationships.
- MLflow now natively supports OpenTelemetry GenAI Semantic Conventions for trace export when the MLFLOW_ENABLE_OTEL_GENAI_SEMCONV flag is enabled.
- Budget management in the AI Gateway includes a UI for tracking spending, configuring webhooks for notifications, and monitoring violations across gateway endpoints.

## Source
- **Origin:** github_releases
- **URL:** <https://github.com/mlflow/mlflow/releases/tag/v3.11.1>

## Related
[[concepts/mlflow|mlflow]] · [[concepts/ai-gateway|ai-gateway]] · [[concepts/opentelemetry-genai-semantic-conventions|opentelemetry-genai-semantic-conventions]] · [[concepts/trace-graph-view|trace-graph-view]] · [[concepts/observability|observability]] · [[concepts/opentelemetry|opentelemetry]] · [[concepts/genai|genai]] · [[concepts/ai|ai]] · [[companies/mlflow-oss-project|MLflow (OSS Project)]] · [[people/tome-hirata|Tome Hirata]] · [[people/joel-robin|Joel Robin]] · [[episodes/2026-04-08|2026-04-08]]
