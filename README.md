# Awesome Enterprise AI Solutions

A curated collection of open-source frameworks, infrastructure, and implementation patterns for building enterprise-grade AI systems. The focus is on production readiness, private deployments, scalability, observability, governance, and cost-aware architecture.

## Why this repo

This repository is for architects, developers, and engineering teams evaluating practical open-source building blocks for enterprise AI.

It is organized around the stack you typically need in real projects:

- Agent frameworks and LLM application frameworks.
- Retrieval, knowledge systems, and vector databases.
- Workflow orchestration and serving infrastructure.
- Observability, metadata, quality, and governance.
- Hands-on starter projects and enterprise implementation patterns.

## Enterprise AI stack

### Agent frameworks

- **[LangGraph](https://github.com/langchain-ai/langgraph)** - Low-level orchestration framework for building durable, stateful, and controllable language agents.

### LLM application frameworks

- **[LLMware](https://github.com/llmware-ai/llmware)** - Framework for enterprise RAG pipelines and compact task-focused models.
- **[LangChain](https://github.com/langchain-ai/langchain)** - Widely used framework for building LLM applications and agent workflows.
- **[LlamaIndex](https://github.com/run-llama/llama_index)** - Framework for connecting private and enterprise data to LLM applications.

### Retrieval and knowledge systems

- **[Haystack](https://github.com/deepset-ai/haystack)** - Open-source framework for retrieval, RAG pipelines, and question answering systems.
- **[Jina](https://github.com/jina-ai/jina)** - Framework for multimodal AI and neural search applications.

### Vector databases

- **[Qdrant](https://github.com/qdrant/qdrant)** - High-performance vector database for semantic search and recommendation workloads.
- **[Weaviate](https://github.com/weaviate/weaviate)** - Open-source vector database designed for semantic search and AI-native applications.

### Workflow orchestration

- **[Apache Airflow](https://github.com/apache/airflow)** - Workflow orchestration platform for scheduled and data-driven pipelines.
- **[Prefect](https://github.com/PrefectHQ/prefect)** - Modern workflow orchestration platform for Python-first automation and data/ML flows.

### Serving and inference

- **[vLLM](https://github.com/vllm-project/vllm)** - High-throughput LLM inference and serving engine.
- **[BentoML](https://github.com/bentoml/BentoML)** - Framework for packaging and serving ML and LLM applications.
- **[Seldon Core](https://github.com/SeldonIO/seldon-core)** - Kubernetes-native model serving for production ML systems.

### Observability and evaluation

- **[Langfuse](https://github.com/langfuse/langfuse)** - Open-source LLM engineering and observability platform for tracing, prompts, and evaluation.
- **[Prometheus](https://prometheus.io/)** - Metrics collection and monitoring for infrastructure and AI services.

### Metadata, quality, and governance

- **[Great Expectations](https://github.com/great-expectations/great_expectations)** - Data quality validation framework for pipelines and structured datasets.
- **[OpenMetadata](https://github.com/open-metadata/OpenMetadata)** - Unified metadata platform for discovery, lineage, governance, and collaboration.

### Learning and references

- **[LLMs from Scratch](https://github.com/rasbt/LLMs-from-scratch)** - Practical implementation-oriented guide to understanding modern LLM systems.
- **[Awesome LLM Agents](https://github.com/kaushikjadhav01/awesome-llm-agents)** - Curated reference list for agent tooling and patterns.

## Starter projects

Beginner-friendly projects for learning open-source AI components with a hands-on approach.

| Project | Description | Status |
|---|---|---|
| `starter_open_source_ai/local_llm_chatbot` | Build a local conversational assistant with open-source models. | Available |
| `starter_open_source_ai/rag_over_pdfs` | Build a simple document Q&A workflow over PDFs. | Planned |
| `starter_open_source_ai/basic_rest_agent` | Build an AI workflow that calls external APIs. | Planned |
| `starter_open_source_ai/batch_inference_pipeline` | Run scheduled inference with orchestration and model serving. | Planned |

## Enterprise implementation patterns

Reference patterns for production-oriented enterprise AI solutions.

| Pattern | Stack | Status |
|---|---|---|
| `enterprise_rag_patterns/local_rag_llama_qdrant` | Llama 3, Qdrant, LangChain | Available |
| `enterprise_rag_patterns/hybrid_search_rag` | Haystack, Weaviate or Qdrant | Planned |
| `enterprise_rag_patterns/rag_as_a_service` | FastAPI, Docker, LlamaIndex | Planned |
| `enterprise_ai_agents/system_architect_agent` | LangGraph or LangChain, enterprise reasoning workflows | Planned |
| `enterprise_ai_agents/incident_triage_agent` | Retrieval, logs, alert analysis, remediation suggestions | Planned |
| `enterprise_ai_agents/requirements_agent` | Requirements drafting and document generation workflows | Planned |

## Repository status

At the moment, only the following example folders are available in the repository:

- `starter_open_source_ai/local_llm_chatbot`
- `enterprise_rag_patterns/local_rag_llama_qdrant`

The remaining examples listed above are intended roadmap items. Keeping them marked as **Planned** makes the README accurate while still showing the direction of the repository.

## Getting started

1. Clone the repository.
2. Open one of the available example folders.
3. Install dependencies from that example.
4. Copy environment variables if the example includes an `.env.example` file.
5. Run the project locally.

```bash
git clone https://github.com/SwapnilPopat/awesome-enterprise-ai-solutions.git
cd awesome-enterprise-ai-solutions
```

### Run the currently available starter project

```bash
cd starter_open_source_ai/local_llm_chatbot
pip install -r requirements.txt
cp .env.example .env  # if present
python main.py
```

### Run the currently available enterprise RAG pattern

```bash
cd enterprise_rag_patterns/local_rag_llama_qdrant
pip install -r requirements.txt
cp .env.example .env  # if present
python main.py
```

## Contribution guidelines

Contributions are welcome.

When submitting a pull request, please include:

- Project or framework name.
- Clear category placement.
- Short description of the use case.
- Setup steps and dependencies.
- Notes on production relevance, trade-offs, or enterprise fit.

## Roadmap ideas

- Add more runnable examples for agent workflows, hybrid search, and multimodal pipelines.
- Add architecture diagrams for each enterprise pattern.
- Add a comparison matrix for framework selection.
- Add observability and evaluation examples with Langfuse.
- Add deployment guides for local, Docker, and Kubernetes environments.

## License

MIT License
