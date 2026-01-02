<!-- Sync Impact Report:
Version change: N/A → 1.0.0
Added sections: All principles and sections for AI-Generated Technical Book project
Removed sections: None (new constitution)
Templates requiring updates: N/A (new project)
Follow-up TODOs: None
-->
# AI-Generated Technical Book with Integrated RAG Chatbot Constitution


## Core Principles

### Accuracy & Verifiability
All content and responses must be grounded in verified sources from the book; Zero hallucination tolerance; All claims must be verifiable and traceable to specific sections of the book

### AI-Native, Retrieval-Optimized Writing
Content must be structured for optimal vector retrieval; Markdown content should be semantically chunked to support RAG system; Writing style optimized for AI consumption and retrieval

### Clear, Developer-Focused Explanations
All technical content must be clearly explained with practical examples; Focus on developer usability and understanding; Complex concepts broken down into digestible, actionable information

### Reproducible Architecture and Code
All technical implementations must be reproducible with clear documentation; Clean, production-ready code; Architecture decisions documented and justified

### Modular, Semantic Content Structure
Content written in modular, semantically chunked Markdown; Clear separation of content, infrastructure, and AI logic; Consistent terminology and structure

### Source-Grounded Responses
RAG chatbot answers only from book content with citations or section references included in responses; Strict adherence to book content without external sources


## Technical Stack and Infrastructure Requirements
Docusaurus for book deployment on GitHub Pages; FastAPI backend for RAG system; OpenAI Agents/ChatKit SDK for AI interactions; Qdrant Cloud for vector database; Neon Serverless PostgreSQL for data storage


## Development Workflow and Quality Standards
All changes must maintain zero hallucination tolerance; Code must follow clean, production-ready standards; Content must be optimized for vector retrieval; Quality gates include accuracy verification and build/deployment validation


## Governance

All implementations must adhere to the core principles of accuracy, AI-native optimization, and developer focus; PRs must verify compliance with quality standards; Architecture decisions must support reproducible and modular design

**Version**: 1.0.0 | **Ratified**: 2026-01-02 | **Last Amended**: 2026-01-02