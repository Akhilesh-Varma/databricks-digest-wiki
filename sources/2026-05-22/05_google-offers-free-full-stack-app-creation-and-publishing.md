---
type: story
story_id: hn_48226634
episode_date: 2026-05-22
rank: 5
source: hacker_news
url: "https://cloud.google.com/blog/products/databases/vibe-coded-ai-studio-apps-with-firestore-firebase-cloud-sql"
title: Google offers free full-stack app creation and publishing
quality_score: 0.653
content_hash: "sha256:394c47f00bc5e61132b191a893497167821124efc2fc0a75bf8fe37a8e530ce6"
concepts: [google-ai-studio, google-cloud-starter-tier, cloud-run, cloud-sql, firestore, firebase-auth, postgresql, vibe-coding, google-workspace]
companies: [google, google-cloud, firebase]
people: [justin-mahood, gopal-ashok]
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-22 10:20:52.683000"
tags: [story, source/hacker-news]
---

## Summary
At Google I/O 2026, Google announced expanded integration between Google AI Studio and Google Cloud, allowing new users to deploy up to two full-stack applications for free on the Google Cloud Starter Tier without a billing account. The update adds Cloud SQL (PostgreSQL) as a relational database option alongside the existing Firestore non-relational database, with an AI agent that can automatically infer the appropriate database type. Applications are deployed to Cloud Run with Firebase Auth handling authentication, and the new Cloud SQL developer edition scales to zero to minimize costs. Google Workspace tools such as Sheets, Calendar, and Gmail are also integrated via Firebase Auth as a unified login flow. Users who outgrow the Starter Tier can upgrade to a standard billable Google Cloud project with all resources transferred automatically.

## Key claims
- New users can deploy up to two full-stack applications on the Google Cloud Starter Tier at no cost, with no billing account or credit card required.
- Cloud SQL for PostgreSQL is introduced as a new relational database option alongside Firestore for non-relational data in AI Studio integrations.
- The AI agent in AI Studio can automatically infer whether to use a relational or non-relational database for a given application.
- A new Cloud SQL for PostgreSQL developer edition supports automatic scale-to-zero, so users only pay when the app is actively used.
- Firebase Auth serves as the single user login flow and enables tight integration with Google Workspace tools like Sheets, Calendar, and Gmail.
- Applications are deployed to Cloud Run with a single click directly from AI Studio.
- Users who exceed Starter Tier limits can upgrade to a standard Google Cloud project and all resources are transferred to the billable project.

## Source
- **Origin:** hacker_news
- **URL:** <https://cloud.google.com/blog/products/databases/vibe-coded-ai-studio-apps-with-firestore-firebase-cloud-sql>

## Related
[[concepts/google-ai-studio|google-ai-studio]] · [[concepts/google-cloud-starter-tier|google-cloud-starter-tier]] · [[concepts/cloud-run|cloud-run]] · [[concepts/cloud-sql|cloud-sql]] · [[concepts/firestore|firestore]] · [[concepts/firebase-auth|firebase-auth]] · [[concepts/postgresql|postgresql]] · [[concepts/vibe-coding|vibe-coding]] · [[concepts/relational-database|relational-database]] · [[concepts/google-cloud|google-cloud]] · [[concepts/workspace|workspace]] · [[concepts/ai-agent|ai-agent]] · [[concepts/schema|schema]] · [[concepts/cloud|cloud]] · [[concepts/sql|sql]] · [[concepts/ai|ai]] · [[companies/google|Google]] · [[companies/google-cloud|Google Cloud]] · [[companies/firebase|Firebase]] · [[people/justin-mahood|Justin Mahood]] · [[people/gopal-ashok|Gopal Ashok]] · [[episodes/2026-05-22|2026-05-22]]
