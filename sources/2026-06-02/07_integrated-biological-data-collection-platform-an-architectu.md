---
type: story
story_id: devto_3795976
episode_date: 2026-06-02
rank: 7
source: devto
url: "https://dev.to/jeferson0993/integrated-biological-data-collection-platform-an-architecture-for-automated-curation-of-public-3fl7"
title: Integrated Biological Data Collection Platform An Architecture for Automated Curation of Public Repositories
quality_score: 0.847
content_hash: "sha256:6724224711531e2b2c34d84c9a8c87e3a4ac1c9272a7952a27e08cb7204c327b"
concepts: [data-lake, rest-api, minio, postgresql, docker-compose, fastapi, gene-expression-omnibus, ncbi-gene, pubmed, uniprot, object-storage, metadata, containerized, data-collection, reproducibility, asynchronous, retry-mechanism]
companies: [minio]
people: []
extractor_model: gemini-2.5-flash-lite
extracted_at: "2026-06-02 10:20:28.533000"
tags: [story, source/devto]
---

## Summary
This article introduces an architecture for an Integrated Biological Data Collection Platform designed to automate the curation of public biological repositories. The platform addresses the challenges of data diversity, standardization, and reproducibility in biomedical research. It utilizes a containerized Biomedical Data Collector coupled with a Data Lake, offering a REST API for asynchronous data collection from sources like GEO, NCBI Gene, PubMed, and UniProt. The system stores raw data in MinIO and metadata in PostgreSQL, ensuring traceability and resilience through a multi-layered architecture and robust error handling.

## Key claims
- The exponential growth of biological data in public repositories presents challenges due to diverse formats, protocols, and metadata models.
- Lack of standardization in data storage compromises the reproducibility of scientific studies.
- An architecture treating data collection as a service is necessary to overcome the limitations of ad hoc solutions.
- The proposed platform provides a REST API for automated, asynchronous data collection from major biological repositories.
- Raw data is stored immutably in MinIO, and metadata is persisted in PostgreSQL.
- The system ensures traceability and resilience through a multi-layered architecture and retry mechanisms.
- The platform's collector engine follows a lifecycle of fetch, validate, upload, and metadata generation for each data source.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/jeferson0993/integrated-biological-data-collection-platform-an-architecture-for-automated-curation-of-public-3fl7>

## Related
[[concepts/data-lake|data-lake]] · [[concepts/rest-api|rest-api]] · [[concepts/minio|minio]] · [[concepts/postgresql|postgresql]] · [[concepts/fastapi|fastapi]] · [[concepts/object-storage|object-storage]] · [[concepts/metadata|metadata]] · [[concepts/containerized|containerized]] · [[concepts/data-collection|data-collection]] · [[concepts/reproducibility|reproducibility]] · [[concepts/asynchronous|asynchronous]] · [[concepts/retry-mechanism|retry-mechanism]] · [[concepts/metadata-management|metadata-management]] · [[concepts/bioinformatics|bioinformatics]] · [[concepts/orchestration|orchestration]] · [[concepts/docker|docker]] · [[concepts/rest|rest]] · [[concepts/api|api]] · [[companies/minio|MinIO]] · [[episodes/2026-06-02|2026-06-02]]
