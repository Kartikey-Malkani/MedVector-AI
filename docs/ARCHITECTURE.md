# Architecture Overview

## System Goals

- medically grounded responses
- source transparency
- scalable retrieval and indexing
- production-friendly deployment

## Components

### 1) Frontend Application
Responsibilities:
- user query input
- answer rendering with citations
- source/chunk inspection
- enterprise upload UX
- analytics and product telemetry

### 2) Backend API Service
Responsibilities:
- request validation
- retrieval orchestration
- answer routing/fallback
- source enrichment for UI
- document ingestion and metadata tracking

### 3) Retrieval Layer
Responsibilities:
- vector similarity search
- metadata joins for source context
- top-k candidate preparation for reranking

### 4) Reranker + Answer Service
Responsibilities:
- context ranking refinement
- answer synthesis with structured output
- robust fallback behavior under latency constraints

### 5) Data Stores
- vector index for semantic retrieval
- metadata store for documents and chunks
- cache for repeated-query acceleration

## Query Flow

1. User asks a question.
2. Backend checks cache (CAG path).
3. If miss, retrieval + reranking executes (RAG path).
4. Answer is generated with source references.
5. Frontend displays answer, confidence cues, and source details.

## Upload Flow

1. PDF is uploaded.
2. Text extraction and chunking run.
3. Embeddings are generated.
4. Chunks are inserted into vector index.
5. Metadata is persisted for traceability.

## Operational Focus

- low-latency response path
- graceful degradation under model failures
- source-level explainability
- observable performance metrics
