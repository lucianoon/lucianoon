# Luciano de Oliveira Nunes

*[English version](README.en.md)*

**Engenheiro de IA focado em produção** — construo sistemas agênticos, RAG e
produtos de IA orientados por avaliação. Meus projetos combinam métricas
reproduzíveis, testes automatizados, CI e artefatos que permitem verificar os
resultados.

## Projetos principais

### 🔨 [Forgehand](https://github.com/lucianoon/forgehand) - engenharia de agentes

Sistema multiagente para entrega de software com LangGraph, fan-out paralelo,
judge LLM com veto objetivo, gates humanos, memória persistente e execução
durável em PostgreSQL.

- **Piloto:** 88,9% de conclusão em 9 workflows, US$ 0,003 por workflow e p95 de 41,6 s
- **Engenharia:** 95 funções de teste; CI com PostgreSQL 16 e Neo4j 5
- **Evidência:** [metodologia e diagnóstico do piloto](https://github.com/lucianoon/forgehand/blob/main/docs/pilot-report-2026-07-20.md)

### 🔎 [Enterprise RAG System](https://github.com/lucianoon/enterprise-rag-system) - recuperação mensurável

RAG híbrido com busca lexical e vetorial, fusão de scores, reranking, citações
e avaliação de recuperação como parte da própria API.

- **Métricas:** Recall@K e MRR sobre dataset rotulado e versionado
- **Transparência:** scores de cada estágio expostos na resposta
- **Demo:** [API interativa](https://enterprise-rag-demo.onrender.com/docs)
- **Trilhas irmãs:** recuperação única e mensurável aqui; tool use iterativo no
  [RAG Agentic System](https://github.com/lucianoon/rag-agentic-system); grafo de
  conhecimento no [TechScout AI](https://github.com/lucianoon/techscout-ai) — três
  problemas de recuperação distintos, não três versões do mesmo projeto

### 🌐 [Pulse Site](https://github.com/lucianoon/pulse-site) - presença institucional e fullstack

Site institucional em Django para apresentar serviços de IA, automação,
atendimento, páginas web e presença comercial.

- **Stack:** Django, templates server-side, Docker e deploy pronto para evolução
- **Verificação:** testes de fumaça das páginas e do endpoint de contato no CI
- **Uso:** base comercial para apresentar serviços, casos e captação de clientes
- **Função no portfólio:** complemento fullstack aos projetos técnicos de IA

## Especializações demonstradas

| Área | Projeto | Evidência |
|---|---|---|
| IA em saúde | [SRAG Health Monitor](https://github.com/lucianoon/srag-health-monitor) | Relatórios epidemiológicos auditáveis com API, worker assíncrono e guardrails |
| Fine-tuning | [LoRA TweetSumm](https://github.com/lucianoon/lora-tweetsumm) | T5 + LoRA, ablação de rank, ROUGE-L e [demo no Hugging Face](https://huggingface.co/spaces/lucianoon/lora-tweetsumm-demo) |
| GraphRAG | [TechScout AI](https://github.com/lucianoon/techscout-ai) | Grafo de conhecimento + busca textual/vetorial, avaliação, cobertura publicada e [demo ao vivo](https://techscout-demo.onrender.com) |
| Edge/automotivo | [AutoDiag](https://github.com/lucianoon/autodiag) | Diagnóstico OBD2, CLI/web e [pacote no PyPI](https://pypi.org/project/autodiag/) |
| Otimização | [Sistema de Otimização Logística](https://github.com/lucianoon/sistema-otimizacao-logistica) | OR-Tools, CVRP, análise de custos e interface Streamlit |
| RAG agêntico | [RAG Agentic System](https://github.com/lucianoon/rag-agentic-system) | Recuperação iterativa com tool use e reformulação de consultas |
| Multiagentes verticais | [multi-agents-recrutadores](https://github.com/lucianoon/multi-agents-recrutadores) | Aplicação de agentes em recrutamento e automação de fluxo específico |

## Estado do portfólio

Levantamento de 01/09/2026. A contagem é de funções de teste na `main`; a
última coluna aponta a evidência externa mais forte de cada projeto.

| Repositório | Testes | Evidência externa |
|---|---:|---|
| [Forgehand](https://github.com/lucianoon/forgehand) | 95 | Piloto medido; CI com PostgreSQL e Neo4j |
| [AutoDiag](https://github.com/lucianoon/autodiag) | 283 | [Pacote no PyPI](https://pypi.org/project/autodiag/), release automatizado |
| [Enterprise RAG System](https://github.com/lucianoon/enterprise-rag-system) | 55 | [Demo ao vivo](https://enterprise-rag-demo.onrender.com/docs), Recall@K e MRR na API |
| [TechScout AI](https://github.com/lucianoon/techscout-ai) | 185 | [Demo ao vivo](https://techscout-demo.onrender.com), GraphRAG com Neo4j e Qdrant |
| [SRAG Health Monitor](https://github.com/lucianoon/srag-health-monitor) | 89 | Relatório de exemplo auditável; CodeQL no CI |
| [mcp-dados-br](https://github.com/lucianoon/mcp-dados-br) | 61 | [PyPI](https://pypi.org/project/mcp-dados-br/), MCP Registry e Smithery; 19 tools de dados públicos |
| [llm-course](https://github.com/lucianoon/llm-course) | 39 | 19 módulos com laboratórios reproduzíveis e portão de avaliação no CI |
| [LoRA TweetSumm](https://github.com/lucianoon/lora-tweetsumm) | 37 | [Demo no Hugging Face](https://huggingface.co/spaces/lucianoon/lora-tweetsumm-demo), ablação de rank |
| [RAG Agentic System](https://github.com/lucianoon/rag-agentic-system) | 72 | Loop de tool use com modelo determinístico offline |
| [vigia-licitacoes](https://github.com/lucianoon/vigia-licitacoes) | 59 | Monitor do PNCP com regras YAML e alertas no Telegram |
| [Sistema de Otimização Logística](https://github.com/lucianoon/sistema-otimizacao-logistica) | 55 | OR-Tools, CVRP e Streamlit |
| [Pulse Site](https://github.com/lucianoon/pulse-site) | 6 | `check --deploy` sem avisos e smoke do gunicorn no CI |
| [multi-agents-recrutadores](https://github.com/lucianoon/multi-agents-recrutadores) | 28 | Demonstração de orquestração multiagente |

Todos os repositórios ativos têm CI verde, licença, topics e Docker. Repositórios
arquivados (orbit-ai-orchestrator, novaforge, fde-ai-platform) ficam fora da
tabela de propósito.

## Princípios de engenharia

- **Avaliação antes de afirmação:** Recall@K, MRR, ROUGE, datasets e baselines versionados
- **Degradação graciosa:** backends simulados e caminhos determinísticos quando modelos externos falham
- **Produção verificável:** testes, CI, Docker, health checks, retries e execução durável
- **Observabilidade:** custo, latência, falhas e decisões rastreadas por execução
- **Stack principal:** Python, FastAPI, Django, PyTorch, Transformers, LangGraph, PostgreSQL, Qdrant e Neo4j

## Foco profissional

**Forward Deployed AI Engineering:** transformar problemas de negócio em
sistemas de IA confiáveis, observáveis e mensuráveis.

[LinkedIn](https://www.linkedin.com/in/luciano-oliveira-nunes/) ·
[GitHub](https://github.com/lucianoon)
