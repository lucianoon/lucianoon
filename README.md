# Luciano de Oliveira Nunes

*[English version](README.en.md)*

**Engenheiro de IA focado em produção.** Construo sistemas que continuam
mensuráveis e verificáveis quando o LLM falha: agentes, RAG, avaliação,
observabilidade e produtos de IA aplicados a problemas reais.

Minha stack principal é Python, FastAPI, LangGraph, PyTorch, PostgreSQL,
Qdrant e Neo4j.

## Projetos em destaque

### 🔨 [Forgehand](https://github.com/lucianoon/forgehand) — engenharia de agentes

Plataforma multiagente para entrega de software com fan-out paralelo, execução
durável, gates humanos e um judge LLM subordinado a verificações objetivas como
`pytest`, `ruff` e `mypy`.

- **Operação:** circuit breakers de custo, tempo e tentativas; tracing OTel/Langfuse
- **Confiabilidade:** checkpoints em PostgreSQL e retomada após interrupções
- **Evidência:** [piloto reproduzível com metodologia e limitações](https://github.com/lucianoon/forgehand/blob/main/docs/pilot-report-2026-07-20.md)

### 🚗 [AutoDiag](https://github.com/lucianoon/autodiag) — IA em um produto vertical

Diagnóstico OBD2 para veículos 2015+, distribuído como pacote Python. Combina
protocolo automotivo, CLI, FastAPI, SSE, SQLite e análise opcional por LLM.

- **Experimente sem hardware:** `pip install autodiag && autodiag scan --demo`
- **Produto:** leitura de DTCs/PIDs/VIN, histórico e interface web local
- **Distribuição:** [pacote publicado no PyPI](https://pypi.org/project/autodiag/)

### 🇧🇷 [mcp-dados-br](https://github.com/lucianoon/mcp-dados-br) — dados públicos para agentes

Servidor MCP com ferramentas para consultar IBGE, Banco Central, INMET, Câmara
dos Deputados e Senado Federal a partir de assistentes de IA.

- **Instalação:** `uvx mcp-dados-br`
- **Adoção:** publicado no [PyPI](https://pypi.org/project/mcp-dados-br/), MCP Registry e Smithery
- **Engenharia:** cache, retry, transporte stdio/HTTP, testes offline e Docker

## Outros trabalhos selecionados

| Área | Projeto | Evidência principal |
|---|---|---|
| RAG mensurável | [Enterprise RAG System](https://github.com/lucianoon/enterprise-rag-system) | Busca híbrida, scores por estágio, Recall@K/MRR e [API interativa](https://enterprise-rag-demo.onrender.com/docs) |
| Fine-tuning | [LoRA TweetSumm](https://github.com/lucianoon/lora-tweetsumm) | T5 + LoRA, ablação de rank, ROUGE e [demo no Hugging Face](https://huggingface.co/spaces/lucianoon/lora-tweetsumm-demo) |
| GraphRAG | [TechScout AI](https://github.com/lucianoon/techscout-ai) | Grafo + busca textual/vetorial, baseline versionado e [demo](https://techscout-demo.onrender.com) |
| Saúde pública | [SRAG Health Monitor](https://github.com/lucianoon/srag-health-monitor) | Relatórios epidemiológicos auditáveis, API, worker e guardrails |
| Engenharia de LLMs | [llm-course](https://github.com/lucianoon/llm-course) | Curso aberto em português com 19 módulos e laboratórios reproduzíveis |
| GovTech | [vigia-licitacoes](https://github.com/lucianoon/vigia-licitacoes) | Monitor do PNCP com regras YAML, deduplicação e alertas no Telegram |

## Como eu trabalho

- **Avaliação antes de afirmação:** datasets e baselines versionados, Recall@K,
  MRR, ROUGE e análise explícita das limitações
- **Degradação graciosa:** backends simulados e caminhos determinísticos para
  executar e testar sem depender de modelos externos
- **Produção verificável:** testes automatizados, CI, Docker, health checks,
  retries e execução durável
- **Observabilidade:** custo, latência, falhas e decisões rastreados por execução

## Foco profissional

**Forward Deployed AI Engineering:** transformar problemas de negócio em
sistemas de IA confiáveis, observáveis e mensuráveis.

[LinkedIn](https://www.linkedin.com/in/luciano-oliveira-nunes/) ·
[GitHub](https://github.com/lucianoon)
