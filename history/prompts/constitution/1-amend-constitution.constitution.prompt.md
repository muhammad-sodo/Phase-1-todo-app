---
id: 1
title: Amend Constitution
stage: constitution
date: 2026-01-02
surface: agent
model: claude-sonnet-4-5-20250929
feature: none
branch: master
user: user
command: sp.constitution
labels: ["constitution", "setup", "governance"]
links:
  spec: null
  ticket: null
  adr: null
  pr: null
files:
 - .specify/memory/constitution.md
tests:
---

## Prompt

```
sp.constitution
Project

AI-Generated Technical Book with Integrated RAG Chatbot

Objective

Create a fully automated technical book using Spec-Kit Plus and Claude Code, deployed via Docusaurus on GitHub Pages, with an embedded RAG chatbot that answers questions strictly from the book's content.

Core Principles

Accuracy & verifiability

AI-native, retrieval-optimized writing

Clear, developer-focused explanations

Reproducible architecture and code

Technical Stack

Book & Deployment

Docusaurus

Spec-Kit Plus

GitHub Pages

RAG System

FastAPI backend

OpenAI Agents / ChatKit SDK

Qdrant Cloud (vector DB)

Neon Serverless PostgreSQL

Functional Requirements

Book written in modular, semantically chunked Markdown

Content optimized for vector retrieval

RAG chatbot answers only from book content

Supports question answering on user-selected text

Citations or section references included in responses

Quality Standards

Zero hallucination tolerance

All claims verifiable

Clean, production-ready code

Consistent terminology and structure

Deliverables

Docusaurus book (deployed on GitHub Pages)

Fully functional RAG chatbot

Setup, deployment, and architecture documentation

Success Criteria

Build and deploy without errors

Accurate, source-grounded chatbot responses

Clear separation of content, infrastructure, and AI logic
```

## Response snapshot

Updated the project constitution with the specified principles and requirements for the AI-Generated Technical Book with Integrated RAG Chatbot project. The constitution now includes six core principles: Accuracy & Verifiability, AI-Native Retrieval-Optimized Writing, Clear Developer-Focused Explanations, Reproducible Architecture and Code, Modular Semantic Content Structure, and Source-Grounded Responses. It also defines technical stack requirements and development workflow standards.

## Outcome

- ✅ Impact: Updated project constitution with project-specific principles and governance
- 🧪 Tests: N/A
- 📁 Files: Updated .specify/memory/constitution.md
- 🔁 Next prompts: Plan and implement features according to the new constitution
- 🧠 Reflection: Constitution provides clear governance framework for the AI book project

## Evaluation notes (flywheel)

- Failure modes observed: None
- Graders run and results (PASS/FAIL): N/A
- Prompt variant (if applicable): N/A
- Next experiment (smallest change to try): N/A