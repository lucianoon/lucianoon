# Luciano de Oliveira Nunes

*[English version](README.en.md)*

Engenheiro de IA focado em aplicações LLM de nível de produção, sistemas agênticos, pipelines de RAG e plataformas de IA orientadas a avaliação.

Construo sistemas de IA práticos que ligam problemas de negócio a software confiável: APIs, workflows de agentes, pipelines de recuperação, camadas de avaliação, observabilidade, deploy e guardrails operacionais.

## Projetos em destaque

| Projeto | O que demonstra | Evidência |
|---|---|---|
| [Forgehand](https://github.com/lucianoon/forgehand) | Entrega de software com múltiplos agentes | Paralelismo, judge objetivo, gates humanos, estado durável e tracing |
| [AutoDiag](https://github.com/lucianoon/autodiag) | Produto Python para um domínio de hardware real | [PyPI](https://pypi.org/project/autodiag/), demo sem hardware, 67 testes, CLI e interface web |
| [Enterprise RAG](https://github.com/lucianoon/enterprise-rag-system) | Qualidade de recuperação medida | Busca híbrida, reranking, citações, Recall@K e MRR |
| [LoRA TweetSumm](https://github.com/lucianoon/lora-tweetsumm) | Experimentação reproduzível em ML | Ablação de rank, resultados ROUGE, CI, Docker e [demo ao vivo](https://huggingface.co/spaces/lucianoon/lora-tweetsumm-demo) |
| [SRAG Health Monitor](https://github.com/lucianoon/srag-health-monitor) | IA resiliente aplicada à saúde pública | Ingestão DATASUS, jobs retomáveis, guardrails e relatório de exemplo |
| [NovaForge](https://github.com/lucianoon/novaforge) | Engenharia de produto fullstack | React, TypeScript, Express, PostgreSQL e testes automatizados |

## Competências

Todo item abaixo é exercitado por código nos repositórios deste perfil.

- Python, FastAPI, Pydantic, asyncio
- LangGraph, LangChain, CrewAI
- RAG, agentes, tool calling, saída estruturada com JSON Schema
- PostgreSQL, Qdrant, Neo4j, SQLite
- PyTorch, Transformers, PEFT/LoRA, ONNX
- Docker, Docker Compose, GitHub Actions, ruff, mypy, pytest
- OpenTelemetry, Langfuse, métricas Prometheus
- Avaliação, guardrails, log de auditoria, monitoramento de custo e latência
- TypeScript, React, Vite (secundário)

## Detalhes dos sistemas

### [Forgehand](https://github.com/lucianoon/forgehand)

Sistema multiagente de entrega de software sobre LangGraph: fan-out paralelo de tarefas com reducers merge-by-id, judge incremental com veto objetivo (sinais de pytest/ruff/mypy), gates de aprovação humana, circuit breakers de orçamento de tokens e custo, execução durável com checkpoints em Postgres, tracing OTel/Langfuse e um dashboard de mission control.

### [Enterprise RAG System](https://github.com/lucianoon/enterprise-rag-system)

**Recuperação em passo único, otimizada para qualidade de resposta mensurável.** Fusão de scores híbrida BM25 + vetorial, reranking heurístico (sobreposição de título e frase exata), citações fundamentadas, transparência de score por estágio e um endpoint de avaliação Recall@K / MRR sobre um dataset rotulado e versionado. Embedders plugáveis (hashing → TF-IDF → sentence-transformers) e vector stores plugáveis (em memória → Qdrant), de modo que o pipeline inteiro roda offline na CI e troca para os backends de produção por variável de ambiente. Feito para que a qualidade da recuperação seja medida, não presumida.

### [RAG Agentic System](https://github.com/lucianoon/rag-agentic-system)

**Loop de agente em múltiplos passos sobre recuperação, para perguntas que uma única consulta não responde.** Onde o Enterprise RAG recupera uma vez e responde, este roda um loop de tool use com Claude (`search_documents`, `get_task_history`): o agente decide quando buscar, refina a consulta e busca de novo quando os primeiros resultados não bastam, iterando sob um limite de passos. As respostas são então pontuadas quanto ao embasamento nas evidências que as ferramentas de fato retornaram — um proxy lexical determinístico, não implicação semântica — e sinalizadas quando divergem. Memória conversacional, um modelo scripted que torna o loop inteiro testável sem chave de API, e uma CLI para ingestão de corpus.

### [SRAG Health Monitor](https://github.com/lucianoon/srag-health-monitor)

Sistema de relatórios de saúde pública (DATASUS/SIVEP-Gripe) com pipeline multiagente coordenado por blackboard: as etapas declaram pré-condições sobre o estado compartilhado em vez de chamarem umas às outras, rodam em paralelo quando prontas e persistem progresso por etapa. Jobs que falham retomam do ponto exato da falha via endpoint de retry. FastAPI, worker assíncrono, guardrails de auditoria, Docker.

### [LoRA TweetSumm](https://github.com/lucianoon/lora-tweetsumm)

Fine-tuning eficiente em parâmetros do T5 com LoRA (ablação de rank, avaliação ROUGE, testes, CI, Docker) — com uma **[demo ao vivo que roda inteiramente no seu navegador](https://huggingface.co/spaces/lucianoon/lora-tweetsumm-demo)** (adaptador mesclado, exportado para ONNX, quantizado em INT8, servido via Transformers.js).

### [AutoDiag](https://github.com/lucianoon/autodiag)

Diagnóstico OBD2 universal para veículos 2015+, **[publicado no PyPI](https://pypi.org/project/autodiag/)** (`pip install autodiag`): leitura de DTCs e decodificação SAE J2012, PIDs ao vivo, consulta de VIN local + NHTSA, heurística de urgência, explicações de IA em streaming e histórico em SQLite — CLI e interface web em FastAPI, autodetecção de porta multiplataforma, modo demo sem hardware (`autodiag scan --demo`), 67 testes unitários, ruff + mypy na CI.

### [Multi-Agent Recruiters](https://github.com/lucianoon/multi-agents-recrutadores)

Pipeline em CrewAI que transforma insumos de contratação em uma descrição de vaga finalizada, através de três agentes especializados (pesquisador, redator, revisor) encadeados em cinco tarefas sequenciais — com uma suíte de testes estrutural que valida a ligação entre agentes e tarefas sem chamar LLM nenhum.

### [NovaForge](https://github.com/lucianoon/novaforge)

Plataforma fullstack de consultoria em tecnologia, construída com TypeScript, React, Vite e Tailwind CSS.

Todos os projetos acima têm licença MIT e CI no GitHub Actions.

## Posicionamento

Estou construindo em direção a Forward Deployed AI Engineering: traduzir problemas de negócio complexos em sistemas de IA confiáveis, observáveis e escaláveis.
