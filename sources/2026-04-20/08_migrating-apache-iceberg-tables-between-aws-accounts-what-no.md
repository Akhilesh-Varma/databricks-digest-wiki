---
type: story
story_id: devto_3524635
episode_date: 2026-04-20
rank: 8
source: devto
url: "https://dev.to/dutvmta/migrating-apache-iceberg-tables-between-aws-accounts-what-nobody-tells-you-5en7"
title: Migrating Apache Iceberg Tables Between AWS Accounts What Nobody Tells You
quality_score: 0.816
content_hash: "sha256:0a9abd34e4f12167838d7692eec9e4cd8a251128b5482c0d05a61b28030403f8"
concepts: [apache-iceberg, s3, parquet, avro]
companies: [aws]
people: []
extractor_model: llama-3.3-70b-versatile
extracted_at: "2026-04-28 04:06:11.605000"
tags: [story, source/devto]
---

## Summary
The article discusses the challenges of migrating Apache Iceberg tables between AWS accounts, which requires a deep understanding of Iceberg's metadata structure. The author shares their experience of successfully migrating nearly 2,000 Iceberg tables while maintaining full data integrity. The process involves handling edge cases and verifying data consistency at scale. Standard approaches, such as copying files or using CTAS INSERT OVERWRITE, fall short due to issues with metadata and compute costs. The author provides insights into Iceberg's metadata structure, including the role of metadata.json, manifest lists, and manifest files.

## Key claims
- Migrating Apache Iceberg tables between AWS accounts is complex due to the hardcoded S3 URI in Iceberg's metadata.
- Standard approaches, such as copying files or using CTAS INSERT OVERWRITE, are not sufficient for migrating Iceberg tables.
- Iceberg's metadata structure consists of multiple layers, including metadata.json, manifest lists, and manifest files.
- Understanding Iceberg's metadata structure is crucial for successful migration.
- Delete files in Iceberg v2 require special handling during migration.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/dutvmta/migrating-apache-iceberg-tables-between-aws-accounts-what-nobody-tells-you-5en7>

## Related
[[concepts/apache-iceberg|apache-iceberg]] · [[concepts/s3|s3]] · [[concepts/data-consistency|data-consistency]] · [[concepts/manifest-list|manifest-list]] · [[concepts/snapshot|snapshot]] · [[concepts/iceberg|iceberg]] · [[concepts/schema|schema]] · [[concepts/spark|spark]] · [[concepts/ctas|ctas]] · [[concepts/aws|aws]] · [[companies/aws|AWS]] · [[episodes/2026-04-20|2026-04-20]]
