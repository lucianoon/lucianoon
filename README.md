# Luciano de Oliveira Nunes

AI Engineer focused on production-grade LLM applications, agentic systems, RAG pipelines and cloud-native AI platforms.

I build practical AI systems that connect business problems to reliable software: APIs, agent workflows, retrieval pipelines, evaluation layers, observability, deployment and operational guardrails.

## Core Skills

- Python, FastAPI, Pydantic
- LangGraph, LangChain, LlamaIndex
- RAG, Agents, Tool Calling, MCP
- PostgreSQL, Redis, Qdrant
- Docker, Kubernetes, AWS, Azure
- OpenTelemetry, Prometheus, Grafana, Langfuse
- Evaluation, Guardrails, Cost and Latency Monitoring

## Production-Style AI Systems

### [Forgehand](https://github.com/lucianoon/forgehand)

Multi-agent software delivery system on LangGraph: parallel task fan-out with merge-by-id reducers, incremental LLM-judge with objective veto (pytest/ruff/mypy signals), human approval gates, token/cost budget circuit breakers, durable execution with Postgres checkpoints, OTel/Langfuse tracing and a mission-control dashboard.

### [FDE AI Platform](https://github.com/lucianoon/fde-ai-platform)

Platform for building, evaluating and observing LLM agent workflows: typed workflow state, FastAPI contracts, evaluation hooks, per-run trace metadata and Docker Compose — with a deterministic generation fallback so tests and CI run without API keys.

### [Enterprise RAG System](https://github.com/lucianoon/enterprise-rag-system)

Retrieval-quality-first RAG engine: hybrid BM25 + vector score fusion, reranking, citations, per-stage score transparency and a Recall@K / MRR evaluation endpoint — designed so retrieval quality is measured, not assumed.

### [RAG Agentic System](https://github.com/lucianoon/rag-agentic-system)

Agentic RAG system in Python for intelligent document search, retrieval workflows and AI orchestration.

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
