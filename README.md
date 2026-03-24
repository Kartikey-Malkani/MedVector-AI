# MedVector AI

Production-ready medical retrieval and answer assistant built with a hybrid RAG + CAG architecture.

This repository is a **showcase profile** of the project for portfolio, product explanation, and architecture walkthrough.

## Why This Repository Exists

This is a public, documentation-first repository created to explain:
- what the project does
- how the system is designed
- what problems it solves
- how it performs in production

The implementation codebase is intentionally private.

## Project Summary

MedVector AI is designed to answer clinical and enterprise document questions with:
- retrieval-grounded responses
- source traceability
- fast fallback strategies
- production deployment support

Core capabilities include:
- medical Q&A with cited evidence
- enterprise PDF upload and indexing
- chunk-level source inspection
- cache-aware answer generation (CAG)
- latency reporting for CAG and RAG
- frontend UX built for explainability

## High-Level Architecture

The system combines multiple services:
- frontend web app (query, source cards, upload flow, analytics)
- backend API (query orchestration, document ingest, metadata)
- vector retrieval layer (FAISS + metadata store)
- reranker/answer service
- deployment infra on cloud platforms

See [docs/ARCHITECTURE.md](docs/ARCHITECTURE.md) for a deeper breakdown.

## Product Features

- Retrieval + rerank + answer pipeline
- Cited answers with chunk references
- Detailed source cards and chunk preview UX
- Upload pipeline for enterprise PDFs
- Upload phase visibility (uploading vs indexing)
- Operational metrics surfaced in UI

See [docs/FEATURES.md](docs/FEATURES.md).

## Access & Permissions

This repository does not provide source code access.

If you are:
- Recruiter or hiring manager: request a guided demo or architecture review.
- Collaborator candidate: request private access with your GitHub handle and intended scope.
- Security reviewer: request restricted review access under NDA if needed.

Access requests can be submitted through repository Issues using the Access Request template.

See [ACCESS_POLICY.md](ACCESS_POLICY.md).

## Security & Responsible Use

- No patient-identifiable information is included in this repository.
- Demo content is non-sensitive and used for product showcase only.
- Security disclosures should follow [SECURITY.md](SECURITY.md).

## Roadmap Snapshot

- improved retrieval explainability
- richer enterprise document controls
- evaluation dashboard and benchmarking exports
- governance and audit enhancements

See [docs/ROADMAP.md](docs/ROADMAP.md).

## Contact

For demo, collaboration, or access discussion, open an Issue in this repository.

## License

All rights reserved. Content in this repository is for showcase purposes only.
See [LICENSE](LICENSE).
