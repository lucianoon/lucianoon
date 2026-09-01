# Luciano de Oliveira Nunes

*[Versão em português](README.md)*

**Production-focused AI Engineer** - I build agentic systems, RAG platforms and
evaluation-driven AI products. My projects combine reproducible metrics,
automated tests, CI and artifacts that make their results independently
verifiable.

## Flagship projects

### 🔨 [Forgehand](https://github.com/lucianoon/forgehand) - agent engineering

A multi-agent software delivery system with LangGraph, parallel fan-out,
objective vetoes around the LLM judge, human gates, persistent memory and
durable execution on PostgreSQL.

- **Pilot:** 88.9% completion across 9 workflows, US$0.003 per workflow and 41.6 s p95
- **Engineering:** 95 test functions; CI with PostgreSQL 16 and Neo4j 5
- **Evidence:** [pilot methodology and failure analysis](https://github.com/lucianoon/forgehand/blob/main/docs/pilot-report-2026-07-20.md)

### 🔎 [Enterprise RAG System](https://github.com/lucianoon/enterprise-rag-system) - measurable retrieval

Hybrid RAG with lexical and vector retrieval, score fusion, reranking,
citations and retrieval evaluation built into the API.

- **Metrics:** Recall@K and MRR on a labeled, versioned dataset
- **Transparency:** per-stage scores exposed in every response
- **Demo:** [interactive API](https://enterprise-rag-demo.onrender.com/docs)
- **Sibling tracks:** single-pass measurable retrieval here; iterative tool use in
  [RAG Agentic System](https://github.com/lucianoon/rag-agentic-system); a knowledge
  graph in [TechScout AI](https://github.com/lucianoon/techscout-ai) — three distinct
  retrieval problems, not three versions of the same project

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
| GraphRAG | [TechScout AI](https://github.com/lucianoon/techscout-ai) | Knowledge graph + textual/vector retrieval, evaluation, published coverage and a [live demo](https://techscout-demo.onrender.com) |
| Edge/automotive | [AutoDiag](https://github.com/lucianoon/autodiag) | OBD2 diagnostics, CLI/web and a [PyPI package](https://pypi.org/project/autodiag/) |
| Optimization | [Logistics Optimization System](https://github.com/lucianoon/sistema-otimizacao-logistica) | OR-Tools, CVRP, cost analysis and a Streamlit UI |
| Agentic RAG | [RAG Agentic System](https://github.com/lucianoon/rag-agentic-system) | Iterative tool-use retrieval with query reformulation |
| Vertical multi-agent systems | [multi-agents-recrutadores](https://github.com/lucianoon/multi-agents-recrutadores) | Multi-agent workflow applied to recruiting and operational automation |
| Public data for LLMs | [mcp-dados-br](https://github.com/lucianoon/mcp-dados-br) | MCP server with 19 tools over IBGE, Central Bank, INMET, Chamber and Senate data; on [PyPI](https://pypi.org/project/mcp-dados-br/), MCP Registry and Smithery |
| GovTech automation | [vigia-licitacoes](https://github.com/lucianoon/vigia-licitacoes) | PNCP public-tender monitor with YAML rules, LLM summaries, SQLite dedup and Telegram alerts |

## Portfolio status

Snapshot as of 2026-09-01. Counts are test functions on `main`; the last
column points to the strongest external evidence for each project.

| Repository | Tests | External evidence |
|---|---:|---|
| [Forgehand](https://github.com/lucianoon/forgehand) | 95 | Measured pilot; CI with PostgreSQL and Neo4j |
| [AutoDiag](https://github.com/lucianoon/autodiag) | 283 | [PyPI package](https://pypi.org/project/autodiag/), automated releases |
| [Enterprise RAG System](https://github.com/lucianoon/enterprise-rag-system) | 55 | [Live demo](https://enterprise-rag-demo.onrender.com/docs), Recall@K and MRR in the API |
| [TechScout AI](https://github.com/lucianoon/techscout-ai) | 185 | [Live demo](https://techscout-demo.onrender.com), GraphRAG with Neo4j and Qdrant |
| [SRAG Health Monitor](https://github.com/lucianoon/srag-health-monitor) | 89 | Auditable sample report; CodeQL in CI |
| [mcp-dados-br](https://github.com/lucianoon/mcp-dados-br) | 61 | [PyPI](https://pypi.org/project/mcp-dados-br/), MCP Registry and Smithery; 19 Brazilian public-data tools |
| [llm-course](https://github.com/lucianoon/llm-course) | 39 | 19 modules with reproducible labs and an evaluation gate in CI |
| [LoRA TweetSumm](https://github.com/lucianoon/lora-tweetsumm) | 37 | [Hugging Face demo](https://huggingface.co/spaces/lucianoon/lora-tweetsumm-demo), rank ablation |
| [RAG Agentic System](https://github.com/lucianoon/rag-agentic-system) | 72 | Tool-use loop with a deterministic offline model |
| [vigia-licitacoes](https://github.com/lucianoon/vigia-licitacoes) | 59 | PNCP public-tender monitor with YAML rules and Telegram alerts |
| [Logistics Optimization System](https://github.com/lucianoon/sistema-otimizacao-logistica) | 55 | OR-Tools, CVRP and Streamlit |
| [Pulse Site](https://github.com/lucianoon/pulse-site) | 6 | Clean `check --deploy` and a gunicorn smoke test in CI |
| [multi-agents-recrutadores](https://github.com/lucianoon/multi-agents-recrutadores) | 28 | Multi-agent orchestration demo |

Every active repository has green CI, a license, topics and Docker. Archived
repositories (orbit-ai-orchestrator, novaforge, fde-ai-platform) are deliberately
left out of the table.

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
