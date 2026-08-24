# Luciano de Oliveira Nunes

*[Versão em português](README.md)*

**Production-focused AI Engineer** - I build agentic systems, RAG platforms and
evaluation-driven AI products. My projects combine reproducible metrics,
automated tests, CI and artifacts that make their results independently
verifiable.

## Flagship projects

### 🤖 [Orbit AI Orchestrator](https://github.com/lucianoon/orbit-ai-orchestrator) - AI task orchestration

An automation platform built around a Plan-Execute-Verify architecture, with a
web frontend, real-time WebSocket updates, a FastAPI orchestrator, Celery
workers and tools for search, browser automation and code execution.

- **Scope:** product-oriented execution of complex tasks with real-time feedback
- **Engineering:** Docker Compose, Redis, Playwright, SearXNG and clear separation between orchestrator and executor
- **Verification:** 30 unit tests plus 4 integration tests running a real Redis broker and Celery worker in CI
- **Positioning:** my strongest agent-platform style project so far

### 🔎 [Enterprise RAG System](https://github.com/lucianoon/enterprise-rag-system) - measurable retrieval

Hybrid RAG with lexical and vector retrieval, score fusion, reranking,
citations and retrieval evaluation built into the API.

- **Metrics:** Recall@K and MRR on a labeled, versioned dataset
- **Transparency:** per-stage scores exposed in every response
- **Demo:** [interactive API](https://enterprise-rag-demo.onrender.com/docs)

### 🔨 [Forgehand](https://github.com/lucianoon/forgehand) - agent engineering

A multi-agent software delivery system with LangGraph, parallel fan-out,
objective vetoes around the LLM judge, human gates, persistent memory and
durable execution on PostgreSQL.

- **Pilot:** 88.9% completion across 9 workflows, US$0.003 per workflow and 41.6 s p95
- **Engineering:** 95 test functions; CI with PostgreSQL 16 and Neo4j 5
- **Evidence:** [pilot methodology and failure analysis](https://github.com/lucianoon/forgehand/blob/main/docs/pilot-report-2026-07-20.md)

### 🌐 [Pulse Site](https://github.com/lucianoon/pulse-site) - institutional fullstack presence

A Django-based website to present AI services, automation offerings, web
projects and commercial positioning.

- **Stack:** Django, server-side templates, Docker and deployment-ready structure
- **Verification:** smoke tests for every page and the contact endpoint in CI
- **Use:** commercial front door for services, case studies and lead capture
- **Portfolio role:** fullstack complement to the technical AI systems

## Demonstrated specializations

| Area | Project | Evidence |
|---|---|---|
| Healthcare AI | [SRAG Health Monitor](https://github.com/lucianoon/srag-health-monitor) | Auditable epidemiological reporting with API, async worker and guardrails |
| Fine-tuning | [LoRA TweetSumm](https://github.com/lucianoon/lora-tweetsumm) | T5 + LoRA, rank ablation, ROUGE-L and a [Hugging Face demo](https://huggingface.co/spaces/lucianoon/lora-tweetsumm-demo) |
| GraphRAG | [TechScout AI](https://github.com/lucianoon/techscout-ai) | Knowledge graph + textual/vector retrieval, evaluation and published coverage |
| Edge/automotive | [AutoDiag](https://github.com/lucianoon/autodiag) | OBD2 diagnostics, CLI/web and a [PyPI package](https://pypi.org/project/autodiag/) |
| Optimization | [Logistics Optimization System](https://github.com/lucianoon/sistema-otimizacao-logistica) | OR-Tools, CVRP, cost analysis and a Streamlit UI |
| Agentic RAG | [RAG Agentic System](https://github.com/lucianoon/rag-agentic-system) | Iterative tool-use retrieval with query reformulation |
| Vertical multi-agent systems | [multi-agents-recrutadores](https://github.com/lucianoon/multi-agents-recrutadores) | Multi-agent workflow applied to recruiting and operational automation |

## Engineering principles

- **Evaluation before claims:** Recall@K, MRR, ROUGE, versioned datasets and baselines
- **Graceful degradation:** simulated backends and deterministic paths when external models fail
- **Verifiable production work:** tests, CI, Docker, health checks, retries and durable execution
- **Observability:** cost, latency, failures and decisions tracked per run
- **Core stack:** Python, FastAPI, Django, PyTorch, Transformers, LangGraph, PostgreSQL, Qdrant and Neo4j

## Professional focus

**Forward Deployed AI Engineering:** turning business problems into reliable,
observable and measurable AI systems.

[LinkedIn](https://www.linkedin.com/in/luciano-oliveira-nunes/) ·
[GitHub](https://github.com/lucianoon)
