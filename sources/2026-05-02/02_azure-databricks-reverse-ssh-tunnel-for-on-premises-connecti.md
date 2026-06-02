---
type: story
story_id: community_542395736e47
episode_date: 2026-05-02
rank: 2
source: databricks_community
url: "https://community.databricks.com/t5/technical-blog/azure-databricks-reverse-ssh-tunnel-for-on-premises-connectivity/ba-p/155969"
title: Azure Databricks Reverse SSH Tunnel for On-Premises Connectivity
quality_score: 0.78
content_hash: "sha256:9f77bd64dba56127a5aff2d88cef289ac29fda9fc23ee5c0e845313155c49b90"
concepts: [reverse-ssh-tunnel, azure-databricks, lakeflow-connect, azure-expressroute, site-to-site-vpn, azure-standard-load-balancer, azure-application-gateway, private-endpoint, sd-wan, databricks-serverless-compute]
companies: [databricks, microsoft-azure]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 10:18:56.651000"
tags: [story, source/databricks-community]
---

## Summary
This article describes a reverse SSH tunnel proxy hub architecture for connecting Azure Databricks to on-premises databases when corporate firewalls block all inbound traffic from the cloud. The pattern works by having the on-premises host initiate an outbound SSH connection to a proxy VM in Azure, which then forwards application traffic back over that tunnel to the on-premises database. This inverts the typical connection flow, allowing Azure Databricks (both classic and serverless compute) to reach on-premises resources without requiring any inbound firewall rule changes. The article uses MySQL on port 3306 as a running example but notes the pattern applies to any TCP-based database. It also highlights relevance for Lakeflow Connect customers ingesting data from on-premises databases.

## Key claims
- A reverse SSH tunnel allows Azure Databricks to reach on-premises databases without opening any inbound firewall ports on the corporate network.
- The on-premises host initiates an outbound SSH connection to a proxy VM in Azure, and application traffic rides back over that tunnel in reverse.
- The pattern supports both Azure Databricks classic and serverless compute without relaxing on-premises inbound firewall restrictions.
- Outbound SSH (port 22) from on-premises to the cloud is almost always permitted by corporate firewalls, making this pattern broadly applicable.
- The reverse SSH tunnel pattern is specifically useful for Lakeflow Connect customers ingesting data from on-premises databases.
- The same reverse tunnel pattern works for any TCP-based database, including PostgreSQL, Oracle, and SQL Server.
- This pattern is not appropriate when inbound access to on-premises is already permitted, as simpler options like private endpoints or load-balanced proxies are more direct.

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/technical-blog/azure-databricks-reverse-ssh-tunnel-for-on-premises-connectivity/ba-p/155969>

## Related
[[concepts/reverse-ssh-tunnel|reverse-ssh-tunnel]] · [[concepts/azure-databricks|azure-databricks]] · [[concepts/lakeflow-connect|lakeflow-connect]] · [[concepts/azure-expressroute|azure-expressroute]] · [[concepts/site-to-site-vpn|site-to-site-vpn]] · [[concepts/databricks-serverless-compute|databricks-serverless-compute]] · [[concepts/serverless-compute|serverless-compute]] · [[concepts/sql-server|sql-server]] · [[concepts/databricks|databricks]] · [[concepts/postgresql|postgresql]] · [[concepts/lakeflow|lakeflow]] · [[concepts/azure|azure]] · [[concepts/cloud|cloud]] · [[concepts/mysql|mysql]] · [[concepts/sql|sql]] · [[concepts/ssh|ssh]] · [[companies/databricks|Databricks]] · [[companies/microsoft-azure|Microsoft Azure]] · [[episodes/2026-05-02|2026-05-02]]
