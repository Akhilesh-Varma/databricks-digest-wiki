---
type: story
story_id: devto_3713487
episode_date: 2026-05-21
rank: 10
source: devto
url: "https://dev.to/micro-saas-journal/the-ghost-protocol-stack-how-we-rebuilt-payments-when-every-vendor-cut-us-off-42c9"
title: The Ghost Protocol Stack How We Rebuilt Payments When Every Vendor Cut Us Off
quality_score: 0.777
content_hash: "sha256:1dee62266643459f5eb7a6bb763fba2ff051bd72a4bd129382627f1169229e4f"
concepts: [rtp-ii-instant-payment-rail, apache-flink, clickhouse, ipfs, amazon-kinesis-data-streams, tendermint, ussd, ach, cid-v1, amazon-s3, ec2-spot-instances, bigquery]
companies: [stripe, paypal, payhip, gumroad, mcb-sakuk, amazon-web-services, google]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-21 10:22:40.974000"
tags: [story, source/devto]
---

## Summary
A small creator platform with 8,400 monthly active users faced a payment crisis in late 2024 when their country's central bank restricted Stripe, PayPal, Payhip, and Gumroad. After a failed first attempt using a local merchant-acquiring bank and a Tendermint-based ledger, the team rebuilt their payment stack using an unbundled protocol architecture. The new stack leveraged a local e-money issuer on the RTP-II instant-payment rail, IPFS for signed receipts, Kinesis and Apache Flink for real-time validation, and ClickHouse for analytics. The rebuilt system achieved a median end-to-end latency of 2.3 seconds and reduced query costs from $48,000 to $8,200 per month compared to BigQuery.

## Key claims
- The platform's country added Stripe, PayPal, Payhip, and Gumroad to a payment-restriction list, cutting off all international payment vendors.
- The first architecture using a local merchant-acquiring bank and a Tendermint-based ledger produced 3-hour latency spikes and cost $0.78 per transaction.
- The rebuilt stack used MCB-Sakuk, a local e-money issuer running on the central bank's RTP-II instant-payment switch, to onboard creators.
- Signed JSON receipts were emitted to IPFS (CID v1) pinned across two geographically separate clusters for receipt integrity.
- A Flink job validated IPFS CIDs from Kinesis Data Streams and wrote results to a ClickHouse materialized view within 2.1 seconds.
- ClickHouse cost $8,200 per month for a 200 GB daily table versus $48,000 for the BigQuery equivalent.
- After six weeks in production, median end-to-end latency was 2.3 seconds and 99th-percentile latency was 8.7 seconds, within the 15-second SLA.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/micro-saas-journal/the-ghost-protocol-stack-how-we-rebuilt-payments-when-every-vendor-cut-us-off-42c9>

## Related
[[concepts/rtp-ii-instant-payment-rail|rtp-ii-instant-payment-rail]] · [[concepts/apache-flink|apache-flink]] · [[concepts/clickhouse|clickhouse]] · [[concepts/ipfs|ipfs]] · [[concepts/amazon-kinesis-data-streams|amazon-kinesis-data-streams]] · [[concepts/materialized-view|materialized-view]] · [[concepts/egress-fees|egress-fees]] · [[concepts/python|python]] · [[concepts/json|json]] · [[concepts/sdk|sdk]] · [[concepts/api|api]] · [[concepts/s3|s3]] · [[companies/stripe|Stripe]] · [[companies/paypal|PayPal]] · [[companies/payhip|Payhip]] · [[companies/gumroad|Gumroad]] · [[companies/mcb-sakuk|MCB-Sakuk]] · [[companies/amazon-web-services|Amazon Web Services]] · [[companies/google|Google]] · [[episodes/2026-05-21|2026-05-21]]
