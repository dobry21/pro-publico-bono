# Legal AI & Open Source Programs

A curated list of interesting tools, frameworks, and open-source projects at the intersection of legal practice and AI. Divided into two sections: dedicated Legal AI infrastructure tools (orchestration, data, Word/DOCX) and general-purpose open-source projects useful in legal contexts.

---

## Part 1 — Dedicated Legal AI Tools

### 1a — Orchestration

Agent frameworks and pipeline coordination for multi-step legal AI workflows.




### 1b — Data

Ingestion, parsing, RAG, NLP, and output validation for legal document corpora.

| Name | License | Language | Description | Links |
|------|---------|----------|-------------|-------|




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

| Name | Category | License | Language | Description | Links |
|------|----------|---------|----------|-------------|-------|

### 2a - Agentic capapilites 
| [LangGraph](https://langchain-ai.github.io/langgraph/) | MIT | Python | Stateful, graph-based agent orchestration; ideal for multi-step legal research and review workflows | [GitHub](https://github.com/langchain-ai/langgraph) |
| [CrewAI](https://www.crewai.com/) | MIT | Python | Multi-agent framework for assembling specialist legal AI agents (researcher, drafter, reviewer) | [GitHub](https://github.com/crewAIInc/crewAI) |
| [AutoGen](https://microsoft.github.io/autogen/) | MIT | Python | Microsoft's conversational multi-agent framework; supports legal document drafting pipelines | [GitHub](https://github.com/microsoft/autogen) |
| [Agno](https://docs.agno.com/) | MPL-2.0 | Python | Lightweight agent framework with built-in memory, tools, and knowledge; fast multi-agent orchestration | [GitHub](https://github.com/agno-agi/agno) |
| [LlamaIndex](https://www.llamaindex.ai/) | MIT | Python | RAG framework for ingesting, indexing, and querying legal documents (contracts, case law, filings) | [GitHub](https://github.com/run-llama/llama_index) |
| [Haystack](https://haystack.deepset.ai/) | Apache-2.0 | Python | End-to-end NLP pipelines for document search and Q&A; widely used for legal document retrieval | [GitHub](https://github.com/deepset-ai/haystack) |

### 2b - Search engine
| [Meilisearch](https://www.meilisearch.com/) | Search | MIT | Rust | Fast, typo-tolerant full-text search engine; good for building in-house legal knowledge bases | [GitHub](https://github.com/meilisearch/meilisearch) |

### 2c - Data base
| [Weaviate](https://weaviate.io/) | Vector DB | BSD-3 | Go | Open-source vector database for semantic search over legal corpora | [GitHub](https://github.com/weaviate/weaviate) |
| [Qdrant](https://qdrant.tech/) | Vector DB | Apache-2.0 | Rust | High-performance vector search engine; well-suited for contract similarity and case law retrieval | [GitHub](https://github.com/qdrant/qdrant) |
| [Supabase](https://supabase.com/) | Database | Apache-2.0 | TypeScript | Open-source Firebase alternative (Postgres + Auth + Storage); rapid backend for legal AI apps | [GitHub](https://github.com/supabase/supabase) |

### 2d - Model deploymenty
| [Ollama](https://ollama.com/) | LLM Runtime | MIT | Go | Run open-weight LLMs locally; critical for air-gapped legal environments where data cannot leave premises | [GitHub](https://github.com/ollama/ollama) |
| [vLLM](https://docs.vllm.ai/) | LLM Runtime | Apache-2.0 | Python | High-throughput LLM serving; deploy open models for internal legal AI with production performance | [GitHub](https://github.com/vllm-project/vllm) |

### 2e - Model safety
| [Guardrails AI](https://www.guardrailsai.com/) | Apache-2.0 | Python | Validates and corrects LLM outputs against schemas and rules; useful for contract clause extraction | [GitHub](https://github.com/guardrails-ai/guardrails) |
| [Garak](https://garak.ai/) | Apache-2.0 | Python | LLM vulnerability scanner; red-teaming tool to probe legal AI systems for hallucination and bias | [GitHub](https://github.com/NVIDIA/garak) |
| [NeMo Guardrails](https://github.com/NVIDIA/NeMo-Guardrails) | Apache-2.0 | Python | NVIDIA's toolkit for adding programmable guardrails (topical, safety, factual) to LLM applications | [GitHub](https://github.com/NVIDIA/NeMo-Guardrails) |

---

## Notes

- **Part 1 subsections:** `1a Orchestration` = agent/pipeline coordination · `1b Data` = ingestion, parsing, RAG, guardrails · `1c Word (DOCX)` = document generation and templating
- **License legend:** MIT / Apache-2.0 = permissive · GPL / AGPL = copyleft · Fair-code = source-available with usage restrictions
- Add new entries by duplicating a row and filling in all columns.
