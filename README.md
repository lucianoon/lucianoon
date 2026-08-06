# Luciano de Oliveira Nunes

*[English version](README.en.md)*

**Engenheiro de IA focado em produção** — construo sistemas agênticos, RAG e
produtos de IA orientados por avaliação. Meus principais projetos combinam
métricas reproduzíveis, testes automatizados, CI e artefatos que permitem
verificar os resultados.

## Projetos principais

### 🔨 [Forgehand](https://github.com/lucianoon/forgehand) — engenharia de agentes

Sistema multiagente para entrega de software com LangGraph, fan-out paralelo,
judge LLM com veto objetivo, gates humanos, memória persistente e execução
durável em PostgreSQL.

- **Piloto:** 88,9% de conclusão em 9 workflows, US$ 0,003 por workflow e p95 de 41,6 s
- **Engenharia:** 95 funções de teste; CI com PostgreSQL 16 e Neo4j 5
- **Evidência:** [metodologia e diagnóstico do piloto](https://github.com/lucianoon/forgehand/blob/main/docs/pilot-report-2026-07-20.md)

### 🔎 [Enterprise RAG System](https://github.com/lucianoon/enterprise-rag-system) — recuperação mensurável

RAG híbrido com busca lexical e vetorial, fusão de scores, reranking, citações
e avaliação de recuperação como parte da própria API.

- **Métricas:** Recall@K e MRR sobre dataset rotulado e versionado
- **Transparência:** scores de cada estágio expostos na resposta
- **Demo:** [API interativa](https://enterprise-rag-demo.onrender.com/docs)

### 🏥 [SRAG Health Monitor](https://github.com/lucianoon/srag-health-monitor) — IA em saúde pública

Geração auditável de relatórios epidemiológicos usando dados
DATASUS/SIVEP-Gripe, com API, worker assíncrono, jobs retomáveis, anonimização
de PII e guardrails.

- **Qualidade:** 89 testes offline
- **Operação:** API e worker em Docker Compose
- **Evidência:** [relatório de exemplo](https://github.com/lucianoon/srag-health-monitor/blob/main/docs/exemplo/relatorio_exemplo.md)

## Especializações demonstradas

| Área | Projeto | Evidência |
|---|---|---|
| Fine-tuning | [LoRA TweetSumm](https://github.com/lucianoon/lora-tweetsumm) | T5 + LoRA, ablação de rank, ROUGE-L e [demo no Hugging Face](https://huggingface.co/spaces/lucianoon/lora-tweetsumm-demo) |
| GraphRAG | [TechScout AI](https://github.com/lucianoon/techscout-ai) | Grafo de conhecimento + busca textual/vetorial, avaliação e cobertura publicada |
| Edge/automotivo | [AutoDiag](https://github.com/lucianoon/autodiag) | Diagnóstico OBD2, CLI/web e [pacote no PyPI](https://pypi.org/project/autodiag/) |
| Otimização | [Sistema de Otimização Logística](https://github.com/lucianoon/sistema-otimizacao-logistica) | OR-Tools, CVRP, análise de custos e interface Streamlit |
| RAG agêntico | [RAG Agentic System](https://github.com/lucianoon/rag-agentic-system) | Recuperação iterativa com tool use e reformulação de consultas |

## Princípios de engenharia

- **Avaliação antes de afirmação:** Recall@K, MRR, ROUGE, datasets e baselines versionados
- **Degradação graciosa:** backends simulados e caminhos determinísticos quando modelos externos falham
- **Produção verificável:** testes, CI, Docker, health checks, retries e execução durável
- **Observabilidade:** custo, latência, falhas e decisões rastreados por execução
- **Stack principal:** Python, FastAPI, PyTorch, Transformers, LangGraph, PostgreSQL, Qdrant e Neo4j

## Foco profissional

**Forward Deployed AI Engineering:** transformar problemas de negócio em
sistemas de IA confiáveis, observáveis e mensuráveis.

[LinkedIn](https://www.linkedin.com/in/luciano-oliveira-nunes/) ·
[GitHub](https://github.com/lucianoon)
