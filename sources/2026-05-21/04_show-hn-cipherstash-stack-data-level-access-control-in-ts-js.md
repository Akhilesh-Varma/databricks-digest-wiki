---
type: story
story_id: hn_48216786
episode_date: 2026-05-21
rank: 4
source: hacker_news
url: "https://cipherstash.com/blog/introducing-cipherstash-stack"
title: Show HN CipherStash Stack Data Level Access Control in TS JS
quality_score: 0.618
content_hash: "sha256:0e21f25bdc3610dd075405e245f7f45081a2217b67c11b15b59b60658031f616"
concepts: [searchable-encryption, zerokms, hardware-security-module, transparent-sql-proxy, oidc-federation, prisma, drizzle-orm, cipherstash-stack]
companies: [cipherstash, auth0, clerk, supabase]
people: [dan-draper]
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-21 10:21:14.010000"
tags: [story, source/hacker-news]
---

## Summary
CipherStash Stack is a data-level access control and searchable encryption platform for TypeScript/JavaScript and Postgres, announced by founder Dan Draper. It includes an open-source SDK, a key management service called ZeroKMS backed by hardware security modules, a transparent SQL proxy, and an OIDC federation auth library. The platform integrates with popular tools like Prisma, Drizzle, Auth0, Clerk, and Supabase, and can be initialized with a single CLI command. The team claims most encrypted queries run in a few milliseconds, with full benchmarks published publicly. The goal is to make per-value searchable encryption practical for everyday engineering teams.

## Key claims
- CipherStash Stack provides per-value searchable encryption for TypeScript/JavaScript applications using Postgres.
- The platform includes ZeroKMS, a key management service backed by hardware security modules (HSMs).
- A transparent SQL proxy is included to handle encrypted queries without application-level changes.
- Setup can be completed in approximately 15 minutes using a single 'npx stash init' command.
- Most encrypted queries execute in a few milliseconds according to published benchmarks.
- The SDK integrates with Prisma, Drizzle, Auth0, Clerk, and Supabase.
- CipherStash has spent five years developing the underlying searchable encryption technology.

## Source
- **Origin:** hacker_news
- **URL:** <https://cipherstash.com/blog/introducing-cipherstash-stack>

## Related
[[concepts/searchable-encryption|searchable-encryption]] · [[concepts/zerokms|zerokms]] · [[concepts/hardware-security-module|hardware-security-module]] · [[concepts/transparent-sql-proxy|transparent-sql-proxy]] · [[concepts/oidc-federation|oidc-federation]] · [[concepts/cipherstash-stack|cipherstash-stack]] · [[concepts/postgres|postgres]] · [[concepts/oidc|oidc]] · [[concepts/sdk|sdk]] · [[concepts/sql|sql]] · [[companies/cipherstash|CipherStash]] · [[companies/auth0|Auth0]] · [[companies/clerk|Clerk]] · [[companies/supabase|Supabase]] · [[people/dan-draper|Dan Draper]] · [[episodes/2026-05-21|2026-05-21]]
