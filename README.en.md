# Luciano de Oliveira Nunes

*[Versão em português](README.md)*

AI Engineer focused on production-grade LLM applications, agentic systems, RAG pipelines and evaluation-driven AI platforms.

I build practical AI systems that connect business problems to reliable software: APIs, agent workflows, retrieval pipelines, evaluation layers, observability, deployment and operational guardrails.

## Core Skills

Every item below is exercised by code in the repositories on this profile.

- Python, FastAPI, Pydantic, asyncio
- LangGraph, LangChain, CrewAI
- RAG, agents, tool calling, structured output with JSON Schema
- PostgreSQL, Qdrant, Neo4j, SQLite
- PyTorch, Transformers, PEFT/LoRA, ONNX
- Docker, Docker Compose, GitHub Actions, ruff, mypy, pytest
- OpenTelemetry, Langfuse, Prometheus metrics
- Evaluation, guardrails, audit logging, cost and latency monitoring
- TypeScript, React, Vite (secondary)

## Production-Style AI Systems

### [Forgehand](https://github.com/lucianoon/forgehand)

Multi-agent software delivery system on LangGraph: parallel task fan-out with merge-by-id reducers, incremental LLM-judge with objective veto (pytest/ruff/mypy signals), human approval gates, token/cost budget circuit breakers, durable execution with Postgres checkpoints, OTel/Langfuse tracing and a mission-control dashboard.

### [Enterprise RAG System](https://github.com/lucianoon/enterprise-rag-system)

**Single-shot retrieval, optimized for measurable answer quality.** Hybrid BM25 + vector score fusion, heuristic reranking (title and exact-phrase overlap), grounded citations, per-stage score transparency and a Recall@K / MRR evaluation endpoint over a versioned labeled dataset. Pluggable embedders (hashing → TF-IDF → sentence-transformers) and vector stores (in-memory → Qdrant), so the whole pipeline runs offline in CI and swaps to production backends by environment variable. Built so retrieval quality is measured, not assumed.

### [RAG Agentic System](https://github.com/lucianoon/rag-agentic-system)

**Multi-step agent loop over retrieval, for questions one query cannot answer.** Where the Enterprise RAG engine retrieves once and answers, this one runs a Claude tool-use loop (`search_documents`, `get_task_history`): the agent decides when to search, refines the query and searches again when the first results fall short, and iterates under a bounded step cap. Answers are then scored for groundedness against the evidence the tools actually returned — a deterministic lexical proxy, not semantic entailment — and flagged when they drift. Conversational memory, a scripted offline model so the full loop is testable without API keys, and a CLI for corpus ingestion.

### [SRAG Health Monitor](https://github.com/lucianoon/srag-health-monitor)

Public-health reporting system (DATASUS/SIVEP-Gripe) with a multi-agent pipeline coordinated by a blackboard: steps declare preconditions over shared state instead of calling each other, run in parallel when ready, and persist progress per step. Failed jobs resume from the exact point of failure via a retry API endpoint. FastAPI, async worker, audit guardrails, Docker.

### [LoRA TweetSumm](https://github.com/lucianoon/lora-tweetsumm)

Parameter-efficient fine-tuning of T5 with LoRA (rank ablation, ROUGE evaluation, tests, CI, Docker) — with a **[live demo that runs entirely in your browser](https://huggingface.co/spaces/lucianoon/lora-tweetsumm-demo)** (adapter merged, exported to ONNX, INT8-quantized, served via Transformers.js).

### [AutoDiag](https://github.com/lucianoon/autodiag)

Universal OBD2 diagnostics for 2015+ vehicles, **[published on PyPI](https://pypi.org/project/autodiag/)** (`pip install autodiag`): DTC reading and SAE J2012 decoding, live PIDs, local + NHTSA VIN lookup, urgency heuristics, streaming AI explanations and SQLite history — CLI and FastAPI web UI, cross-platform port autodetection, a hardware-free demo mode (`autodiag scan --demo`), 67 unit tests, ruff + mypy in CI.

### [Multi-Agent Recruiters](https://github.com/lucianoon/multi-agents-recrutadores)

CrewAI pipeline that turns hiring inputs into a polished job description through three specialized agents (researcher, writer, reviewer) chained across five sequential tasks — with a structural test suite that validates agent/task wiring without calling LLMs.

### [NovaForge](https://github.com/lucianoon/novaforge)

Fullstack technology consulting platform built with TypeScript, React, Vite and Tailwind CSS.

Every project above ships with an MIT license and GitHub Actions CI.

## Building Next

- Telecom AI Agent: multi-agent customer support workflow inspired by telecom operations.
- LLM Evaluation Lab: framework for groundedness, latency, cost, refusal and hallucination risk.
- Prompt Security Gateway: protection layer for prompt injection, PII detection and audit logs.

## Positioning

I am building toward Forward Deployed AI Engineering: translating complex business problems into reliable, observable and scalable AI systems.
