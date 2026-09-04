# Luciano de Oliveira Nunes

*[Versão em português](README.md)*

**Production-focused AI Engineer.** I build systems that remain measurable and
verifiable when the LLM fails: agents, RAG, evaluation, observability and AI
products applied to real-world problems.

My core stack is Python, FastAPI, LangGraph, PyTorch, PostgreSQL, Qdrant and
Neo4j.

## Featured projects

### 🔨 [Forgehand](https://github.com/lucianoon/forgehand) — agent engineering

A multi-agent software delivery platform with parallel fan-out, durable
execution, human gates and an LLM judge constrained by objective checks such as
`pytest`, `ruff` and `mypy`.

- **Operations:** cost, time and retry circuit breakers; OTel/Langfuse tracing
- **Reliability:** PostgreSQL checkpoints and recovery after interruptions
- **Evidence:** [reproducible pilot with methodology and limitations](https://github.com/lucianoon/forgehand/blob/main/docs/pilot-report-2026-07-20.md)

### 🚗 [AutoDiag](https://github.com/lucianoon/autodiag) — AI in a vertical product

An OBD2 diagnostics tool for 2015+ vehicles, distributed as a Python package.
It combines automotive protocols, a CLI, FastAPI, SSE, SQLite and optional LLM
analysis.

- **Try it without hardware:** `pip install autodiag && autodiag scan --demo`
- **Product:** DTC/PID/VIN reading, history and a local web interface
- **Distribution:** [published on PyPI](https://pypi.org/project/autodiag/)

### 🇧🇷 [mcp-dados-br](https://github.com/lucianoon/mcp-dados-br) — public data for agents

An MCP server that lets AI assistants query data from IBGE, the Central Bank of
Brazil, INMET, the Chamber of Deputies and the Federal Senate.

- **Install:** `uvx mcp-dados-br`
- **Adoption:** published on [PyPI](https://pypi.org/project/mcp-dados-br/), MCP Registry and Smithery
- **Engineering:** caching, retries, stdio/HTTP transports, offline tests and Docker

## Other selected work

| Area | Project | Primary evidence |
|---|---|---|
| Measurable RAG | [Enterprise RAG System](https://github.com/lucianoon/enterprise-rag-system) | Hybrid search, per-stage scores, Recall@K/MRR and an [interactive API](https://enterprise-rag-demo.onrender.com/docs) |
| Fine-tuning | [LoRA TweetSumm](https://github.com/lucianoon/lora-tweetsumm) | T5 + LoRA, rank ablation, ROUGE and a [Hugging Face demo](https://huggingface.co/spaces/lucianoon/lora-tweetsumm-demo) |
| GraphRAG | [TechScout AI](https://github.com/lucianoon/techscout-ai) | Graph + textual/vector retrieval, a versioned baseline and a [live demo](https://techscout-demo.onrender.com) |
| Public health | [SRAG Health Monitor](https://github.com/lucianoon/srag-health-monitor) | Auditable epidemiological reports, API, worker and guardrails |
| LLM engineering | [llm-course](https://github.com/lucianoon/llm-course) | Open Portuguese-language course with 19 modules and reproducible labs |
| GovTech | [vigia-licitacoes](https://github.com/lucianoon/vigia-licitacoes) | PNCP monitor with YAML rules, deduplication and Telegram alerts |

## How I work

- **Evaluation before claims:** versioned datasets and baselines, Recall@K, MRR,
  ROUGE and explicit analysis of limitations
- **Graceful degradation:** simulated backends and deterministic paths that run
  and test without external models
- **Verifiable production work:** automated tests, CI, Docker, health checks,
  retries and durable execution
- **Observability:** cost, latency, failures and decisions tracked per run

## Professional focus

**Forward Deployed AI Engineering:** turning business problems into reliable,
observable and measurable AI systems.

[LinkedIn](https://www.linkedin.com/in/luciano-oliveira-nunes/) ·
[GitHub](https://github.com/lucianoon)
