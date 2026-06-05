---
type: story
story_id: rss_24fc2daedda7
episode_date: 2026-06-05
rank: 5
source: rss_feed
url: "https://arxiv.org/abs/2606.05679"
title: Data Flow Control Data Safety Policies for AI Agents
quality_score: 0.756
content_hash: "sha256:3c6ed32f381f920b5f3f8fd4b5e15165e2a92e814c62037d5d1639278ba026d6"
concepts: [data-flow-control-dfc, passant, query-rewriting, provenance-monomials, duckdb, umbra, postgresql, datafusion, sql-server, ai-agents]
companies: []
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-06-05 10:18:27.360000"
tags: [story, source/rss-feed]
---

## Summary
This paper introduces Data Flow Control (DFC), a framework for declaratively specifying and enforcing data safety policies over tuple-level data flows within database management systems. The authors argue that query correctness is insufficient for safety, as semantically valid queries can still violate regulatory, privacy, or business constraints. DFC formalizes data safety as aggregate predicates over provenance monomials and introduces Passant, a portable query rewriting layer that enforces DFC policies without materializing provenance. Passant is evaluated across five DBMS engines—DuckDB, Umbra, PostgreSQL, DataFusion, and SQL Server—achieving zero overhead compared to alternatives. The work positions data safety enforcement as a data infrastructure problem rather than a prompt-engineering or post-hoc checking problem, particularly in the context of AI agents generating SQL and orchestrating pipelines.

## Key claims
- Query correctness is not equivalent to data safety; a semantically valid query can still violate regulatory, privacy, or business constraints.
- Data Flow Control (DFC) is a framework that declaratively specifies and guarantees policy enforcement over tuple-level data flows within a DBMS query.
- DFC formalizes data safety as aggregate predicates over provenance monomials.
- Passant is a portable query rewriting layer that enforces DFC policies without materializing provenance.
- Passant achieves zero overhead and outperforms alternatives by orders of magnitude across DuckDB, Umbra, PostgreSQL, DataFusion, and SQL Server.
- Enforcing data safety constraints is fundamentally a data infrastructure problem, not a prompting or post-hoc checking problem.
- Data Flow Control is released as open-source software.

## Source
- **Origin:** rss_feed
- **URL:** <https://arxiv.org/abs/2606.05679>

## Related
[[concepts/data-flow-control-dfc|data-flow-control-dfc]] · [[concepts/passant|passant]] · [[concepts/query-rewriting|query-rewriting]] · [[concepts/provenance-monomials|provenance-monomials]] · [[concepts/ai-agents|ai-agents]] · [[concepts/open-source|open-source]] · [[concepts/sql|sql]] · [[episodes/2026-06-05|2026-06-05]]
