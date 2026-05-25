---
type: story
story_id: devto_3739765
episode_date: 2026-05-25
rank: 5
source: devto
url: "https://dev.to/aws-builders/databricks-and-fsx-for-ontap-s3-access-points-a-layer-by-layer-validation-of-observed-boundaries-p4d"
title: Databricks and FSx for ONTAP S3 Access Points A Layer-by-Layer Validation of Observed Boundaries
quality_score: 0.886
content_hash: "sha256:c7b3c3cab03e2dc899dd4d5b902cacc8f198bf7ff900758b8ce59f0f1e3712bd"
concepts: [unity-catalog, fsx-for-ontap-s3-access-points, unity-catalog-external-locations, delta-lake, nfs-kernel-mount, seccomp, instance-profile, boto3, apache-spark, strace, lakehouse, vpc]
companies: [databricks, amazon-web-services, netapp]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-25 10:18:16.871000"
tags: [story, source/devto]
---

## Summary
This article documents a layer-by-layer technical validation of integrating Databricks with FSx for ONTAP S3 Access Points, testing multiple approaches including Unity Catalog External Locations, NFS mounts, Instance Profiles, and various VPC configurations. The author found that Unity Catalog's session policy initially blocks the FSx for ONTAP S3 Access Point ARN pattern with a 403 error, and while setting a specific field on the External Location partially resolves this, UC table creation, subdirectory listing, and write operations remain blocked. NFS kernel mounts are blocked by seccomp by design, as confirmed by Databricks Support, while Instance Profile boto3 works for direct S3 Access Point access bypassing Unity Catalog. The validation was performed on DBR 17.3 LTS in the ap-northeast-1 region, and the article is explicitly scoped to one environment and should not be treated as a general compatibility statement.

## Key claims
- Unity Catalog's session policy initially blocks the FSx for ONTAP S3 Access Point ARN pattern with a 403 error.
- Setting the External Location field partially resolves the session policy issue, but UC table creation, subdirectory listing, and write operations remain blocked.
- NFS kernel mount is blocked by seccomp by design, confirmed by Databricks Support.
- Instance Profile boto3 works for direct S3 Access Point access, bypassing Unity Catalog governance.
- Spark read with an explicit file path under UC governance succeeded, reading a sensor CSV of 1000 rows.
- UC governance features such as lineage, tags, and fine-grained access cannot yet be applied to FSx for ONTAP S3 Access Points.
- The validation was conducted on DBR 17.3 LTS in the ap-northeast-1 AWS region.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/aws-builders/databricks-and-fsx-for-ontap-s3-access-points-a-layer-by-layer-validation-of-observed-boundaries-p4d>

## Related
[[concepts/unity-catalog|unity-catalog]] · [[concepts/fsx-for-ontap-s3-access-points|fsx-for-ontap-s3-access-points]] · [[concepts/unity-catalog-external-locations|unity-catalog-external-locations]] · [[concepts/nfs-kernel-mount|nfs-kernel-mount]] · [[concepts/seccomp|seccomp]] · [[concepts/instance-profile|instance-profile]] · [[concepts/boto3|boto3]] · [[concepts/apache-spark|apache-spark]] · [[concepts/external-locations|external-locations]] · [[concepts/governance|governance]] · [[concepts/databricks|databricks]] · [[concepts/delta|delta]] · [[concepts/spark|spark]] · [[concepts/s3|s3]] · [[concepts/uc|uc]] · [[companies/databricks|Databricks]] · [[companies/amazon-web-services|Amazon Web Services]] · [[companies/netapp|NetApp]] · [[episodes/2026-05-25|2026-05-25]]
