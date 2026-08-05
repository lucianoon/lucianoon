# Luciano de Oliveira Nunes

*[English version](README.en.md)*

**Engenheiro de IA focado em produção** — sistemas agênticos, RAG e plataformas
orientadas a avaliação. Cada projeto abaixo tem testes, CI, métricas publicadas
e uma forma de você verificar as afirmações sem acreditar na minha palavra.

## Três projetos que resumem meu trabalho

### 🔨 [Forgehand](https://github.com/lucianoon/forgehand) — agentes com garantias de produção

Sistema multiagente de entrega de software: orquestração LangGraph, fan-out
paralelo, judge LLM com veto objetivo (`pytest`, `ruff` e `mypy` podem reprovar
mesmo quando o judge aprova), gates humanos e execução durável com checkpoints
em PostgreSQL.

> **Piloto medido:** 88,9% de conclusão em 9 workflows reais, custo médio de
> US$ 0,003 por workflow e latência p95 de 41,6 s — metodologia e diagnóstico
> no [relatório do piloto](https://github.com/lucianoon/forgehand/blob/main/docs/pilot-report-2026-07-20.md).
> 95 funções de teste, CI com PostgreSQL 16 e Neo4j 5.

### 🔎 [Enterprise RAG System](https://github.com/lucianoon/enterprise-rag-system) — recuperação que dá para medir

RAG híbrido (BM25 + vetorial) com fusão de scores, reranking, respostas com
citações e **Recall@K / MRR como endpoint de primeira classe da API**. Toda
resposta expõe os scores de cada estágio — dá para ver *por que* um trecho foi
recuperado, não apenas *que* ele foi.

> 55 testes offline, dataset rotulado e versionado, mesmo código do backend em
> memória ao Qdrant. **[Demo ao vivo](https://enterprise-rag-demo.onrender.com/docs)**
> — experimente o `/query` e o `/evaluate/batch` no navegador.

### 🏥 [SRAG Health Monitor](https://github.com/lucianoon/srag-health-monitor) — IA aplicada a um domínio público real

Relatórios epidemiológicos a partir de dados DATASUS/SIVEP-Gripe: API FastAPI,
worker assíncrono, jobs retomáveis por etapa, auditoria, anonimização de PII e
guardrails.

> 89 testes offline, Docker Compose, e um
> [relatório de exemplo](https://github.com/lucianoon/srag-health-monitor/blob/main/docs/exemplo/relatorio_exemplo.md)
> versionado no repositório — a saída é verificável antes de instalar qualquer coisa.

## Outros projetos

| Projeto | Evidência |
|---|---|
| [AutoDiag](https://github.com/lucianoon/autodiag) | Diagnóstico OBD2 **[publicado no PyPI](https://pypi.org/project/autodiag/)** — 89 testes, demo completa sem hardware, CLI + web |
| [LoRA TweetSumm](https://github.com/lucianoon/lora-tweetsumm) | Fine-tuning T5 com LoRA — ablação de rank, ROUGE-L 0,357 e **[demo ao vivo](https://huggingface.co/spaces/lucianoon/lora-tweetsumm-demo)** no Hugging Face |
| [RAG Agentic System](https://github.com/lucianoon/rag-agentic-system) | Loop de tool use com Claude sobre recuperação — raciocínio multi-passo, complementar ao Enterprise RAG |
| [TechScout AI](https://github.com/lucianoon/techscout-ai) | GraphRAG para perguntas relacionais que nenhum trecho isolado responde — **Recall@K e MRR medidos** sobre dataset rotulado, comparando grafo, BM25 e a fusão dos dois. 171 testes, 83% de branch coverage, baseline reexecutado a cada push |
| [Sistema de Otimização Logística](https://github.com/lucianoon/sistema-otimizacao-logistica) | OR-Tools, CVRP com restrições logísticas do Brasil, comparação de algoritmos e interface Streamlit |

## Como eu trabalho

- **Avaliação primeiro:** Recall@K, MRR, ROUGE, groundedness e datasets versionados — se não dá para medir, não dá para melhorar
- **Produção, não demo:** Docker, filas/workers, health checks, retries, circuit breakers e execução durável
- **Observabilidade:** OpenTelemetry, Langfuse, Prometheus, custo e latência rastreados por execução
- **Qualidade automatizada:** pytest, ruff, mypy e GitHub Actions em todos os projetos
- **Stack:** Python, FastAPI, PyTorch, Transformers, PEFT/LoRA, LangGraph, PostgreSQL, Qdrant, Neo4j

## Foco

**Forward Deployed AI Engineering:** traduzir problemas de negócio complexos
em sistemas de IA confiáveis, observáveis e mensuráveis.

📫 [LinkedIn](https://www.linkedin.com/in/luciano-oliveira-nunes/)
