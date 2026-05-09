# Legal AI & Open Source Programs

A curated list of interesting tools, frameworks, and open-source projects at the intersection of legal practice and AI. Divided into two sections: dedicated Legal AI infrastructure tools (orchestration, data, Word/DOCX) and general-purpose open-source projects useful in legal contexts.

---

## Part 1 — Dedicated Legal AI Tools

### 1a — Orchestration

Agent frameworks and pipeline coordination for multi-step legal AI workflows.

| Name | License | Language | Description | Links |
|------|---------|----------|-------------|-------|
| [Mike](https://github.com/willchen96/mike) | AGPL-3.0 | TypeScript | Open-source AI legal platform with Next.js frontend and Express backend; integrates Supabase Auth + Postgres, S3-compatible storage, and LibreOffice for DOC/DOCX-to-PDF conversion | [GitHub](https://github.com/willchen96/mike) |
| [Suzie Law](https://github.com/firelex/suzielaw) | MIT | TypeScript | Open-source alternative to Harvey; legal AI workspace with counsel chat, 12 practice-area personas, 160+ agentic prompt recipes, document Q&A, DOCX drafting, RAG knowledge base, CourtListener case-law research, and local model support; built on the Team Suzie agent platform | [GitHub](https://github.com/firelex/suzielaw) · [Site](https://suzielaw.com) |



### 1b — Data

Ingestion, parsing, RAG, NLP, and output validation for legal document corpora.

| Name | License | Language | Description | Links |
|------|---------|----------|-------------|-------|
| [legal-sources](https://github.com/worldwidelaw/legal-sources) | AGPL-3.0 | Python | 243 collection scripts for open legal data from 50+ countries (EU, EFTA, UK, US, CA and more); standardized scrapers for legislation and case law from official government portals and APIs; normalizes to a common schema; powers the Legal Data Hunter search API (6M+ documents indexed) | [GitHub](https://github.com/worldwidelaw/legal-sources) · [Dashboard](https://legaldatahunter.com) |
| [Water Law Dataset](https://github.com/jrklaus8/water-law-dataset) | MIT | Python | 83,596 water law judicial decisions from Brazil (27 state courts), Canada (CanLII API), and the Netherlands (Rechtspraak); includes scrapers, a regex-based jurimetric coding engine (21 categories, 4 languages), and merge utilities; academic research dataset 2016–2026 | [GitHub](https://github.com/jrklaus8/water-law-dataset) · [Dashboard](https://jrklaus8.github.io/water-law-dataset/) · [Zenodo](https://doi.org/10.5281/zenodo.19836413) |



### 1c — Word (DOCX)

Libraries for generating, editing, and templating Word documents — contracts, pleadings, briefs.

| Name | License | Language | Description | Links |
|------|---------|----------|-------------|-------|
| [Docling](https://ds4sd.github.io/docling/) | MIT | Python | IBM document parsing library; converts PDFs, DOCX, and scanned contracts into structured data | [GitHub](https://github.com/DS4SD/docling) |
| [python-docx](https://python-docx.readthedocs.io/) | MIT | Python | Create and modify Word (.docx) files programmatically; the standard library for contract generation | [GitHub](https://github.com/python-openxml/python-docx) |
| [docxtpl](https://docxtpl.readthedocs.io/) | MIT | Python | Jinja2-based DOCX templating; fill legal document templates with structured data from Python | [GitHub](https://github.com/elapouya/python-docx-template) |
| [Mammoth](https://github.com/mwilliamson/mammoth.py) | BSD-2 | Python / JS | Converts DOCX to clean HTML or Markdown; useful for ingesting Word contracts into AI pipelines | [GitHub](https://github.com/mwilliamson/mammoth.py) |


---

## Part 2 — General Open Source (Useful in Legal Contexts)



### 2a - Agentic capapilites 
| Name | License | Language | Description | Links |
|------|---------|----------|-------------|-------|
| [LangGraph](https://langchain-ai.github.io/langgraph/) | MIT | Python | Stateful, graph-based agent orchestration; ideal for multi-step legal research and review workflows | [GitHub](https://github.com/langchain-ai/langgraph) |
| [CrewAI](https://www.crewai.com/) | MIT | Python | Multi-agent framework for assembling specialist legal AI agents (researcher, drafter, reviewer) | [GitHub](https://github.com/crewAIInc/crewAI) |
| [AutoGen](https://microsoft.github.io/autogen/) | MIT | Python | Microsoft's conversational multi-agent framework; supports legal document drafting pipelines | [GitHub](https://github.com/microsoft/autogen) |
| [Agno](https://docs.agno.com/) | MPL-2.0 | Python | Lightweight agent framework with built-in memory, tools, and knowledge; fast multi-agent orchestration | [GitHub](https://github.com/agno-agi/agno) |
| [LlamaIndex](https://www.llamaindex.ai/) | MIT | Python | RAG framework for ingesting, indexing, and querying legal documents (contracts, case law, filings) | [GitHub](https://github.com/run-llama/llama_index) |
| [Haystack](https://haystack.deepset.ai/) | Apache-2.0 | Python | End-to-end NLP pipelines for document search and Q&A; widely used for legal document retrieval | [GitHub](https://github.com/deepset-ai/haystack) |

### 2b - Search engine
| Name | License | Language | Description | Links |
|------|---------|----------|-------------|-------|
| [Meilisearch](https://www.meilisearch.com/) | Search | MIT | Rust | Fast, typo-tolerant full-text search engine; good for building in-house legal knowledge bases | [GitHub](https://github.com/meilisearch/meilisearch) |

### 2c - Data base
| Name | License | Language | Description | Links |
|------|---------|----------|-------------|-------|
| [Weaviate](https://weaviate.io/) | Vector DB | BSD-3 | Go | Open-source vector database for semantic search over legal corpora | [GitHub](https://github.com/weaviate/weaviate) |
| [Qdrant](https://qdrant.tech/) | Vector DB | Apache-2.0 | Rust | High-performance vector search engine; well-suited for contract similarity and case law retrieval | [GitHub](https://github.com/qdrant/qdrant) |
| [Supabase](https://supabase.com/) | Database | Apache-2.0 | TypeScript | Open-source Firebase alternative (Postgres + Auth + Storage); rapid backend for legal AI apps | [GitHub](https://github.com/supabase/supabase) |

### 2d - Model deploymenty
| Name | License | Language | Description | Links |
|------|---------|----------|-------------|-------|
| [Ollama](https://ollama.com/) | LLM Runtime | MIT | Go | Run open-weight LLMs locally; critical for air-gapped legal environments where data cannot leave premises | [GitHub](https://github.com/ollama/ollama) |
| [vLLM](https://docs.vllm.ai/) | LLM Runtime | Apache-2.0 | Python | High-throughput LLM serving; deploy open models for internal legal AI with production performance | [GitHub](https://github.com/vllm-project/vllm) |

### 2e - Model safety
| Name | License | Language | Description | Links |
|------|---------|----------|-------------|-------|
| [Guardrails AI](https://www.guardrailsai.com/) | Apache-2.0 | Python | Validates and corrects LLM outputs against schemas and rules; useful for contract clause extraction | [GitHub](https://github.com/guardrails-ai/guardrails) |
| [Garak](https://garak.ai/) | Apache-2.0 | Python | LLM vulnerability scanner; red-teaming tool to probe legal AI systems for hallucination and bias | [GitHub](https://github.com/NVIDIA/garak) |
| [NeMo Guardrails](https://github.com/NVIDIA/NeMo-Guardrails) | Apache-2.0 | Python | NVIDIA's toolkit for adding programmable guardrails (topical, safety, factual) to LLM applications | [GitHub](https://github.com/NVIDIA/NeMo-Guardrails) |

### 2f - Self-Hosted AI Workspaces

General-purpose, self-hostable AI chat platforms with RAG, agents, and document intelligence — deployable on-premises for data-sensitive legal environments.

| Name | License | Language | Description | Links |
|------|---------|----------|-------------|-------|
| [Onyx (FOSS)](https://github.com/onyx-dot-app/onyx-foss) | MIT | Python / TypeScript | Feature-rich self-hostable AI chat platform; RAG with hybrid search + knowledge graph, 40+ connectors, custom agents, MCP, deep research, web search, code interpreter, and RBAC — fully air-gap compatible | [GitHub](https://github.com/onyx-dot-app/onyx-foss) · [Docs](https://docs.onyx.app) |
| [AnythingLLM](https://github.com/Mintplex-Labs/anything-llm) | MIT | JavaScript | All-in-one desktop & Docker AI app; RAG over any document type, no-code agent builder, MCP compatibility, multi-user permissions, 30+ LLM providers, and embeddable chat widget — runs fully locally | [GitHub](https://github.com/Mintplex-Labs/anything-llm) · [Site](https://anythingllm.com) |

---

## Notes

- **License legend:** MIT / Apache-2.0 = permissive · GPL / AGPL = copyleft · Fair-code = source-available with usage restrictions
- Add new entries by duplicating a row and filling in all columns.
