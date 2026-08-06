# Luciano de Oliveira Nunes

*[English version](README.en.md)*

**Engenheiro de IA focado em producao** - construo sistemas agenticos, RAG e
produtos de IA orientados por avaliacao. Meus projetos combinam metricas
reproduziveis, testes automatizados, CI e artefatos que permitem verificar os
resultados.

## Projetos principais

### 🤖 [Orbit AI Orchestrator](https://github.com/lucianoon/orbit-ai-orchestrator) - orquestracao de tarefas com IA

Plataforma de automacao com arquitetura Plan-Execute-Verify, frontend web,
WebSocket em tempo real, orquestrador FastAPI, workers Celery e ferramentas de
busca, browser e execucao de codigo.

- **Escopo:** produto orientado a execucao de tarefas complexas com feedback em tempo real
- **Engenharia:** Docker Compose, Redis, Playwright, SearXNG e separacao clara entre orquestrador e executor
- **Posicionamento:** meu projeto mais proximo de uma plataforma de agentes pronta para produto

### 🔎 [Enterprise RAG System](https://github.com/lucianoon/enterprise-rag-system) - recuperacao mensuravel

RAG hibrido com busca lexical e vetorial, fusao de scores, reranking, citacoes
e avaliacao de recuperacao como parte da propria API.

- **Metricas:** Recall@K e MRR sobre dataset rotulado e versionado
- **Transparencia:** scores de cada estagio expostos na resposta
- **Demo:** [API interativa](https://enterprise-rag-demo.onrender.com/docs)

### 🔨 [Forgehand](https://github.com/lucianoon/forgehand) - engenharia de agentes

Sistema multiagente para entrega de software com LangGraph, fan-out paralelo,
judge LLM com veto objetivo, gates humanos, memoria persistente e execucao
duravel em PostgreSQL.

- **Piloto:** 88,9% de conclusao em 9 workflows, US$ 0,003 por workflow e p95 de 41,6 s
- **Engenharia:** 95 funcoes de teste; CI com PostgreSQL 16 e Neo4j 5
- **Evidencia:** [metodologia e diagnostico do piloto](https://github.com/lucianoon/forgehand/blob/main/docs/pilot-report-2026-07-20.md)

### 🌐 [Pulse Site](https://github.com/lucianoon/pulse-site) - presenca institucional e fullstack

Site institucional em Django para apresentar servicos de IA, automacao,
atendimento, paginas web e presenca comercial.

- **Stack:** Django, templates server-side, Docker e deploy pronto para evolucao
- **Uso:** base comercial para apresentar servicos, casos e captacao de clientes
- **Funcao no portfolio:** complemento fullstack aos projetos tecnicos de IA

## Especializacoes demonstradas

| Area | Projeto | Evidencia |
|---|---|---|
| IA em saude | [SRAG Health Monitor](https://github.com/lucianoon/srag-health-monitor) | Relatorios epidemiologicos auditaveis com API, worker assincrono e guardrails |
| Fine-tuning | [LoRA TweetSumm](https://github.com/lucianoon/lora-tweetsumm) | T5 + LoRA, ablacao de rank, ROUGE-L e [demo no Hugging Face](https://huggingface.co/spaces/lucianoon/lora-tweetsumm-demo) |
| GraphRAG | [TechScout AI](https://github.com/lucianoon/techscout-ai) | Grafo de conhecimento + busca textual/vetorial, avaliacao e cobertura publicada |
| Edge/automotivo | [AutoDiag](https://github.com/lucianoon/autodiag) | Diagnostico OBD2, CLI/web e [pacote no PyPI](https://pypi.org/project/autodiag/) |
| Otimizacao | [Sistema de Otimizacao Logistica](https://github.com/lucianoon/sistema-otimizacao-logistica) | OR-Tools, CVRP, analise de custos e interface Streamlit |
| RAG agentico | [RAG Agentic System](https://github.com/lucianoon/rag-agentic-system) | Recuperacao iterativa com tool use e reformulacao de consultas |
| Multiagentes verticais | [multi-agents-recrutadores](https://github.com/lucianoon/multi-agents-recrutadores) | Aplicacao de agentes em recrutamento e automacao de fluxo especifico |

## Principios de engenharia

- **Avaliacao antes de afirmacao:** Recall@K, MRR, ROUGE, datasets e baselines versionados
- **Degradacao graciosa:** backends simulados e caminhos deterministicos quando modelos externos falham
- **Producao verificavel:** testes, CI, Docker, health checks, retries e execucao duravel
- **Observabilidade:** custo, latencia, falhas e decisoes rastreados por execucao
- **Stack principal:** Python, FastAPI, Django, PyTorch, Transformers, LangGraph, PostgreSQL, Qdrant e Neo4j

## Foco profissional

**Forward Deployed AI Engineering:** transformar problemas de negocio em
sistemas de IA confiaveis, observaveis e mensuraveis.

[LinkedIn](https://www.linkedin.com/in/luciano-oliveira-nunes/) ·
[GitHub](https://github.com/lucianoon)
