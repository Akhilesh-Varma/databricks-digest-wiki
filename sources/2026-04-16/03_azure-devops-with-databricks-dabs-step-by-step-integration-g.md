---
type: story
story_id: community_11c8c9a67339
episode_date: 2026-04-16
rank: 3
source: databricks_community
url: "https://community.databricks.com/t5/technical-blog/azure-devops-with-databricks-dabs-step-by-step-integration-guide/ba-p/141451"
title: Azure DevOps with Databricks DABs Step-by-Step Integration Guide
quality_score: 0.78
content_hash: "sha256:5e1e3b3e38ba1a4596b3f86e672fab550b80d88937e638edfbff3258e8263299"
concepts: [databricks-asset-bundles-dabs, ci-cd, unity-catalog, databricks-git-folders, azure-devops, trunk-based-branching-strategy, databricks-oidc, azure-devops-service-connections, declarative-automation-bundles, visual-studio-code]
companies: [databricks, microsoft]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:12:17.189000"
tags: [story, source/databricks-community]
---

## Summary
This article provides a comprehensive step-by-step guide for integrating Azure DevOps with Databricks Asset Bundles (DABs) to establish a CI/CD process for data and AI workloads in Azure Databricks. It recommends using Declarative Automation Bundles for deployment, integrated with Databricks Git Folders and Azure DevOps service connections. The guide covers infrastructure and governance alignment, versioned bundle development, and pipeline setup for staging and production deployments. A trunk-based branching strategy is recommended, where staging deploys automatically after pull requests merge into main, and production requires an additional approval step. The article also compares DevOps service connection and Databricks OIDC approaches for connectivity.

## Key claims
- Databricks Asset Bundles (DABs), formerly known as Databricks Asset Bundles, are the recommended deployment mechanism for CI/CD in Azure Databricks.
- The recommended branching strategy is trunk-based, with automatic staging deployment after pull request merges into main and a manual approval gate for production.
- Azure DevOps service connections are used for Databricks connectivity, and the article compares this approach with Databricks OIDC.
- Bundles integrate seamlessly with Databricks Git Folders for version control and Azure DevOps for automation.
- The guide supports multiple independent teams sharing infrastructure, using separate Unity Catalog catalogs (bu1_dev, bu1_stg, bu1_prd) within a single metastore.
- Organizations can use two or three Databricks workspaces aligned with environments, with staging optionally deploying to a secure folder in the dev workspace.
- The approach supports both the Databricks workspace UI and IDEs like Visual Studio Code.

## Source
- **Origin:** databricks_community
- **URL:** <https://community.databricks.com/t5/technical-blog/azure-devops-with-databricks-dabs-step-by-step-integration-guide/ba-p/141451>

## Related
[[concepts/databricks-asset-bundles-dabs|databricks-asset-bundles-dabs]] · [[concepts/ci-cd|ci-cd]] · [[concepts/unity-catalog|unity-catalog]] · [[concepts/databricks-git-folders|databricks-git-folders]] · [[concepts/azure-devops|azure-devops]] · [[concepts/trunk-based-branching-strategy|trunk-based-branching-strategy]] · [[concepts/azure-devops-service-connections|azure-devops-service-connections]] · [[concepts/declarative-automation-bundles|declarative-automation-bundles]] · [[concepts/databricks-asset-bundles|databricks-asset-bundles]] · [[concepts/unity-catalog-metastore|unity-catalog-metastore]] · [[concepts/continuous-integration|continuous-integration]] · [[concepts/databricks-workspace|databricks-workspace]] · [[concepts/azure-databricks|azure-databricks]] · [[concepts/git-folders|git-folders]] · [[concepts/governance|governance]] · [[concepts/databricks|databricks]] · [[concepts/workspace|workspace]] · [[concepts/pipeline|pipeline]] · [[concepts/devops|devops]] · [[concepts/azure|azure]] · [[concepts/oidc|oidc]] · [[concepts/dabs|dabs]] · [[concepts/git|git]] · [[concepts/ai|ai]] · [[companies/databricks|Databricks]] · [[companies/microsoft|Microsoft]] · [[episodes/2026-04-16|2026-04-16]]
