# Luciano de Oliveira Nunes

*[Versão em português](README.md)*

**Production-focused AI Engineer** — agentic systems, RAG and
evaluation-driven platforms. Every project below has tests, CI, published
metrics and a way for you to verify the claims without taking my word for it.

## Three projects that sum up my work

### 🔨 [Forgehand](https://github.com/lucianoon/forgehand) — agents with production guarantees

Multi-agent software delivery system: LangGraph orchestration, parallel
fan-out, LLM judge with objective veto (`pytest`, `ruff` and `mypy` can reject
a delivery even when the judge approves), human gates and durable execution
with PostgreSQL checkpoints.

> **Measured pilot:** 88.9% completion across 9 real workflows, average cost of
> US$ 0.003 per workflow and p95 latency of 41.6 s — methodology and failure
> diagnosis in the [pilot report](https://github.com/lucianoon/forgehand/blob/main/docs/pilot-report-2026-07-20.md).
> 95 test functions, CI with PostgreSQL 16 and Neo4j 5.

### 🔎 [Enterprise RAG System](https://github.com/lucianoon/enterprise-rag-system) — retrieval you can measure

Hybrid RAG (BM25 + vector) with score fusion, reranking, cited answers and
**Recall@K / MRR as a first-class API endpoint**. Every response exposes
per-stage scores — you can see *why* a chunk was retrieved, not just *that*
it was.

> 55 offline tests, a labeled and versioned dataset, and the same code from the
> in-memory backend to Qdrant.

### 🏥 [SRAG Health Monitor](https://github.com/lucianoon/srag-health-monitor) — AI applied to a real public-data domain

Epidemiological reports from Brazilian DATASUS/SIVEP-Gripe data: FastAPI,
async worker, per-step resumable jobs, auditing, PII anonymization and
guardrails.

> 89 offline tests, Docker Compose, and an
> [example report](https://github.com/lucianoon/srag-health-monitor/blob/main/docs/exemplo/relatorio_exemplo.md)
> versioned in the repository — the output is verifiable before installing anything.

## Other projects

| Project | Evidence |
|---|---|
| [AutoDiag](https://github.com/lucianoon/autodiag) | OBD2 diagnostics **[published on PyPI](https://pypi.org/project/autodiag/)** — 89 tests, full hardware-free demo, CLI + web |
| [LoRA TweetSumm](https://github.com/lucianoon/lora-tweetsumm) | T5 fine-tuning with LoRA — rank ablation, ROUGE-L 0.357 and a **[live demo](https://huggingface.co/spaces/lucianoon/lora-tweetsumm-demo)** on Hugging Face |
| [RAG Agentic System](https://github.com/lucianoon/rag-agentic-system) | Tool-use loop with Claude over retrieval — multi-step reasoning, complementary to Enterprise RAG |
| [Logistics Optimization System](https://github.com/lucianoon/sistema-otimizacao-logistica) | OR-Tools, CVRP with Brazilian logistics constraints, algorithm comparison and a Streamlit UI |

## How I work

- **Evaluation first:** Recall@K, MRR, ROUGE, groundedness and versioned datasets — if you can't measure it, you can't improve it
- **Production, not demos:** Docker, queues/workers, health checks, retries, circuit breakers and durable execution
- **Observability:** OpenTelemetry, Langfuse, Prometheus, with cost and latency tracked per run
- **Automated quality:** pytest, ruff, mypy and GitHub Actions across all projects
- **Stack:** Python, FastAPI, PyTorch, Transformers, PEFT/LoRA, LangGraph, PostgreSQL, Qdrant, Neo4j

## Focus

**Forward Deployed AI Engineering:** translating complex business problems
into reliable, observable and measurable AI systems.

📫 [LinkedIn](https://www.linkedin.com/in/luciano-oliveira-nunes/)
