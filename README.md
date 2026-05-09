# Legal AI & Open Source Programs

A curated list of interesting tools, frameworks, and open-source projects at the intersection of legal practice and AI. Divided into two sections: dedicated Legal AI infrastructure tools (orchestration, data, Word/DOCX) and general-purpose open-source projects useful in legal contexts.

---

## Part 1 — Dedicated Legal AI Tools

### 1a — Orchestration

Agent frameworks and pipeline coordination for multi-step legal AI workflows.

| Name | License | Language | Description | Links |
|------|---------|----------|-------------|-------|
| [LangGraph](https://langchain-ai.github.io/langgraph/) | MIT | Python | Stateful, graph-based agent orchestration; ideal for multi-step legal research and review workflows | [GitHub](https://github.com/langchain-ai/langgraph) |
| [CrewAI](https://www.crewai.com/) | MIT | Python | Multi-agent framework for assembling specialist legal AI agents (researcher, drafter, reviewer) | [GitHub](https://github.com/crewAIInc/crewAI) |
| [AutoGen](https://microsoft.github.io/autogen/) | MIT | Python | Microsoft's conversational multi-agent framework; supports legal document drafting pipelines | [GitHub](https://github.com/microsoft/autogen) |
| [Agno](https://docs.agno.com/) | MPL-2.0 | Python | Lightweight agent framework with built-in memory, tools, and knowledge; fast multi-agent orchestration | [GitHub](https://github.com/agno-agi/agno) |
| [LangFuse](https://langfuse.com/) | MIT / EE | Python / TS | Open-source LLM observability — traces, evals, and cost tracking for legal AI pipelines | [GitHub](https://github.com/langfuse/langfuse) |

### 1b — Data

Ingestion, parsing, RAG, NLP, and output validation for legal document corpora.

| Name | License | Language | Description | Links |
|------|---------|----------|-------------|-------|
| [LlamaIndex](https://www.llamaindex.ai/) | MIT | Python | RAG framework for ingesting, indexing, and querying legal documents (contracts, case law, filings) | [GitHub](https://github.com/run-llama/llama_index) |
| [Haystack](https://haystack.deepset.ai/) | Apache-2.0 | Python | End-to-end NLP pipelines for document search and Q&A; widely used for legal document retrieval | [GitHub](https://github.com/deepset-ai/haystack) |
| [Unstructured](https://unstructured.io/) | Apache-2.0 | Python | Preprocessing library for extracting text from legal PDFs, court filings, and HTML pages | [GitHub](https://github.com/Unstructured-IO/unstructured) |
| [OpenContracts](https://github.com/JSv4/OpenContracts) | Apache-2.0 | Python | Open-source legal document annotation and analysis platform built on Django + GraphQL | [GitHub](https://github.com/JSv4/OpenContracts) |
| [Spacy-LLM](https://spacy.io/usage/large-language-models) | MIT | Python | Integrates LLMs into spaCy NLP pipelines for legal NER (parties, dates, clauses, jurisdiction) | [GitHub](https://github.com/explosion/spacy-llm) |
| [NeMo Guardrails](https://github.com/NVIDIA/NeMo-Guardrails) | Apache-2.0 | Python | NVIDIA's toolkit for adding programmable guardrails (topical, safety, factual) to LLM applications | [GitHub](https://github.com/NVIDIA/NeMo-Guardrails) |
| [Guardrails AI](https://www.guardrailsai.com/) | Apache-2.0 | Python | Validates and corrects LLM outputs against schemas and rules; useful for contract clause extraction | [GitHub](https://github.com/guardrails-ai/guardrails) |
| [Garak](https://garak.ai/) | Apache-2.0 | Python | LLM vulnerability scanner; red-teaming tool to probe legal AI systems for hallucination and bias | [GitHub](https://github.com/NVIDIA/garak) |

### 1c — Word (DOCX)

Libraries for generating, editing, and templating Word documents — contracts, pleadings, briefs.

| Name | License | Language | Description | Links |
|------|---------|----------|-------------|-------|
| [Docling](https://ds4sd.github.io/docling/) | MIT | Python | IBM document parsing library; converts PDFs, DOCX, and scanned contracts into structured data | [GitHub](https://github.com/DS4SD/docling) |
| [python-docx](https://python-docx.readthedocs.io/) | MIT | Python | Create and modify Word (.docx) files programmatically; the standard library for contract generation | [GitHub](https://github.com/python-openxml/python-docx) |
| [docxtpl](https://docxtpl.readthedocs.io/) | MIT | Python | Jinja2-based DOCX templating; fill legal document templates with structured data from Python | [GitHub](https://github.com/elapouya/python-docx-template) |
| [Mammoth](https://github.com/mwilliamson/mammoth.py) | BSD-2 | Python / JS | Converts DOCX to clean HTML or Markdown; useful for ingesting Word contracts into AI pipelines | [GitHub](https://github.com/mwilliamson/mammoth.py) |
| [Pandoc](https://pandoc.org/) | GPL-2.0 | Haskell | Universal document converter (DOCX ↔ PDF ↔ Markdown ↔ HTML); essential for legal doc pipelines | [GitHub](https://github.com/jgm/pandoc) |

---

## Part 2 — General Open Source (Useful in Legal Contexts)

General-purpose tools not built exclusively for legal use but highly relevant for legal AI applications — document management, search, workflow automation, and data infrastructure.

| Name | Category | License | Language | Description | Links |
|------|----------|---------|----------|-------------|-------|
| [Apache Tika](https://tika.apache.org/) | Document Parsing | Apache-2.0 | Java | Detects and extracts content from thousands of file types; the backbone of many legal document pipelines | [GitHub](https://github.com/apache/tika) |
| [Tesseract OCR](https://tesseract-ocr.github.io/) | OCR | Apache-2.0 | C++ | Industry-standard OCR engine; essential for digitizing scanned court documents and contracts | [GitHub](https://github.com/tesseract-ocr/tesseract) |
| [Meilisearch](https://www.meilisearch.com/) | Search | MIT | Rust | Fast, typo-tolerant full-text search engine; good for building in-house legal knowledge bases | [GitHub](https://github.com/meilisearch/meilisearch) |
| [OpenSearch](https://opensearch.org/) | Search | Apache-2.0 | Java | Scalable search and analytics; used for enterprise legal document discovery and e-discovery | [GitHub](https://github.com/opensearch-project/OpenSearch) |
| [Weaviate](https://weaviate.io/) | Vector DB | BSD-3 | Go | Open-source vector database for semantic search over legal corpora | [GitHub](https://github.com/weaviate/weaviate) |
| [Qdrant](https://qdrant.tech/) | Vector DB | Apache-2.0 | Rust | High-performance vector search engine; well-suited for contract similarity and case law retrieval | [GitHub](https://github.com/qdrant/qdrant) |
| [n8n](https://n8n.io/) | Workflow | Fair-code | TypeScript | Self-hostable workflow automation; useful for building legal intake, routing, and notification pipelines | [GitHub](https://github.com/n8n-io/n8n) |
| [Prefect](https://www.prefect.io/) | Workflow | Apache-2.0 | Python | Data pipeline orchestration; manage scheduled legal data processing jobs (court feed ingestion, etc.) | [GitHub](https://github.com/PrefectHQ/prefect) |
| [Airflow](https://airflow.apache.org/) | Workflow | Apache-2.0 | Python | Battle-tested pipeline scheduler; runs large-scale legal data ETL and model evaluation workflows | [GitHub](https://github.com/apache/airflow) |
| [Supabase](https://supabase.com/) | Database | Apache-2.0 | TypeScript | Open-source Firebase alternative (Postgres + Auth + Storage); rapid backend for legal AI apps | [GitHub](https://github.com/supabase/supabase) |
| [Metabase](https://www.metabase.com/) | Analytics | AGPL-3.0 | Clojure | Self-hosted BI tool; dashboards for legal ops metrics (matter volume, cost, cycle time) | [GitHub](https://github.com/metabase/metabase) |
| [Paperless-ngx](https://docs.paperless-ngx.com/) | Document Mgmt | GPL-3.0 | Python | Self-hosted document management with OCR and tagging; useful for law firm document organization | [GitHub](https://github.com/paperless-ngx/paperless-ngx) |
| [OpenProject](https://www.openproject.org/) | Project Mgmt | GPL-3.0 | Ruby | Open-source project management for legal teams — matter tracking, deadlines, billing | [GitHub](https://github.com/opf/openproject) |
| [Label Studio](https://labelstud.io/) | Annotation | Apache-2.0 | Python | Data labeling platform for building legal NLP training datasets (clause classification, NER) | [GitHub](https://github.com/HumanSignal/label-studio) |
| [MLflow](https://mlflow.org/) | MLOps | Apache-2.0 | Python | Experiment tracking and model registry; manage versions of legal classification and extraction models | [GitHub](https://mlflow.org/) |
| [Ollama](https://ollama.com/) | LLM Runtime | MIT | Go | Run open-weight LLMs locally; critical for air-gapped legal environments where data cannot leave premises | [GitHub](https://github.com/ollama/ollama) |
| [vLLM](https://docs.vllm.ai/) | LLM Runtime | Apache-2.0 | Python | High-throughput LLM serving; deploy open models for internal legal AI with production performance | [GitHub](https://github.com/vllm-project/vllm) |

---

## Notes

- **Part 1 subsections:** `1a Orchestration` = agent/pipeline coordination · `1b Data` = ingestion, parsing, RAG, guardrails · `1c Word (DOCX)` = document generation and templating
- **License legend:** MIT / Apache-2.0 = permissive · GPL / AGPL = copyleft · Fair-code = source-available with usage restrictions
- Add new entries by duplicating a row and filling in all columns.
