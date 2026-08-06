# Luciano de Oliveira Nunes

*[Versão em português](README.md)*

**Production-focused AI Engineer** — I build agentic systems, RAG platforms and
evaluation-driven AI products. My main projects combine reproducible metrics,
automated tests, CI and artifacts that make their results independently
verifiable.

## Flagship projects

### 🔨 [Forgehand](https://github.com/lucianoon/forgehand) — agent engineering

A multi-agent software delivery system with LangGraph, parallel fan-out,
objective vetoes around the LLM judge, human gates, persistent memory and
durable execution on PostgreSQL.

- **Pilot:** 88.9% completion across 9 workflows, US$0.003 per workflow and 41.6 s p95
- **Engineering:** 95 test functions; CI with PostgreSQL 16 and Neo4j 5
- **Evidence:** [pilot methodology and failure analysis](https://github.com/lucianoon/forgehand/blob/main/docs/pilot-report-2026-07-20.md)

### 🔎 [Enterprise RAG System](https://github.com/lucianoon/enterprise-rag-system) — measurable retrieval

Hybrid RAG with lexical and vector retrieval, score fusion, reranking,
citations and retrieval evaluation built into the API.

- **Metrics:** Recall@K and MRR on a labeled, versioned dataset
- **Transparency:** per-stage scores exposed in every response
- **Demo:** [interactive API](https://enterprise-rag-demo.onrender.com/docs)

### 🏥 [SRAG Health Monitor](https://github.com/lucianoon/srag-health-monitor) — AI for public health

Auditable epidemiological reports from Brazilian DATASUS/SIVEP-Gripe data,
with an API, asynchronous worker, resumable jobs, PII anonymization and
guardrails.

- **Quality:** 89 offline tests
- **Operations:** API and worker through Docker Compose
- **Evidence:** [versioned example report](https://github.com/lucianoon/srag-health-monitor/blob/main/docs/exemplo/relatorio_exemplo.md)

### 🛒 [E-commerce Sales Agent](https://github.com/lucianoon/ecommerce-sales-agent) — business-oriented AI

A multi-tenant sales assistant covering recommendations, carts, Pix payments,
abandonment recovery and human handoff.

- **Integrations:** Nuvemshop, WhatsApp Business and Mercado Pago
- **Reliability:** PostgreSQL, deterministic fallback and CI
- **Product:** operator dashboard plus conversion and assisted-revenue metrics

## Demonstrated specializations

| Area | Project | Evidence |
|---|---|---|
| Fine-tuning | [LoRA TweetSumm](https://github.com/lucianoon/lora-tweetsumm) | T5 + LoRA, rank ablation, ROUGE-L and a [Hugging Face demo](https://huggingface.co/spaces/lucianoon/lora-tweetsumm-demo) |
| GraphRAG | [TechScout AI](https://github.com/lucianoon/techscout-ai) | Knowledge graph + textual/vector retrieval, evaluation and published coverage |
| Edge/automotive | [AutoDiag](https://github.com/lucianoon/autodiag) | OBD2 diagnostics, CLI/web and a [PyPI package](https://pypi.org/project/autodiag/) |
| Optimization | [Logistics Optimization System](https://github.com/lucianoon/sistema-otimizacao-logistica) | OR-Tools, CVRP, cost analysis and a Streamlit UI |
| Agentic RAG | [RAG Agentic System](https://github.com/lucianoon/rag-agentic-system) | Iterative tool-use retrieval with query reformulation |

## Engineering principles

- **Evaluation before claims:** Recall@K, MRR, ROUGE, versioned datasets and baselines
- **Graceful degradation:** simulated backends and deterministic paths when external models fail
- **Verifiable production work:** tests, CI, Docker, health checks, retries and durable execution
- **Observability:** cost, latency, failures and decisions tracked per run
- **Core stack:** Python, FastAPI, PyTorch, Transformers, LangGraph, PostgreSQL, Qdrant and Neo4j

## Professional focus

**Forward Deployed AI Engineering:** turning business problems into reliable,
observable and measurable AI systems.

[LinkedIn](https://www.linkedin.com/in/luciano-oliveira-nunes/) ·
[GitHub](https://github.com/lucianoon)
