# MedVector AI

Production-ready medical retrieval assistant using a hybrid RAG + CAG architecture with source-grounded answers and enterprise document indexing.

[Live Website](https://med-rag-sigma.vercel.app/) | [Architecture](docs/ARCHITECTURE.md) | [Features](docs/FEATURES.md) | [Roadmap](docs/ROADMAP.md)

## Live Product

- Public demo: https://med-rag-sigma.vercel.app/
- Focus: clinical question answering with explainable sources
- Includes: search workflow, citation panel, source chunk preview, enterprise PDF indexing

## Why This Repository Exists

This repository is intentionally documentation-first for showcase purposes.

It helps recruiters, collaborators, and reviewers understand:
- product scope and value
- architecture and technical decisions
- UX and explainability approach
- deployment and operational maturity

Implementation source code is intentionally private.

## Product Highlights

- Hybrid CAG + RAG query flow
- Source-cited answers with chunk-level evidence
- Separate latency visibility for total, CAG, and RAG paths
- Enterprise upload workflow with upload and indexing states
- Chunk preview and full-detail source modal for long evidence passages
- Vercel web analytics integration for product telemetry

## Screenshot Gallery

### 1) Search Landing Experience

![Search landing page](project_images/Search_intial_page%20(1).png)

### 2) Query Results With Cited Sources

![Search results](project_images/Search_results.png)

### 3) Source Card Selection and Evidence Snippet

![Source and chunk citation panel](project_images/Source%20%2C%20chunk%20cited.png)

### 4) Full Chunk Modal for Deep Evidence Review

![Source chunk in detail modal](project_images/Source%20Chunk%20in%20Detail.png)

### 5) Enterprise Document Upload and Indexing State

![Enterprise document indexing flow](project_images/Enterprise_Document_Indexing.png)

## System Overview

Core system components:
- frontend web experience for search, upload, and source explainability
- backend API for orchestration, retrieval, and ingestion
- FAISS-based vector retrieval with metadata joins
- reranker + answer generation service with fallback behavior
- cloud deployment configuration for production use

For full technical details, see [docs/ARCHITECTURE.md](docs/ARCHITECTURE.md).

## Access and Permissions

This public repository does not include source code access.

If you need private implementation access:
- use the Access Request issue template
- include GitHub username, review purpose, and expected duration
- maintainer approval is required

Full policy: [ACCESS_POLICY.md](ACCESS_POLICY.md)

## Security

- No patient-identifiable information is included in this repository
- This is a showcase repository with documentation and visuals only
- Vulnerability reports should follow [SECURITY.md](SECURITY.md)

## Collaboration

- Contribution guide: [CONTRIBUTING.md](CONTRIBUTING.md)
- Code of conduct: [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)

## License

All rights reserved.

This repository is for showcase and informational use only.
See [LICENSE](LICENSE).
