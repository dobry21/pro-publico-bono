# Legal AI & Open Source Programs

A curated list of interesting tools, frameworks, and open-source projects at the intersection of legal practice and AI. Divided into two sections: dedicated Legal AI infrastructure tools (orchestration, data, Word/DOCX) and general-purpose open-source projects useful in legal contexts.

---

## Part 1 — Dedicated Legal AI Tools

### 1a — Orchestration

Agent frameworks and pipeline coordination for multi-step legal AI workflows.

| Name | License | Language | Description | Links |
|------|---------|----------|-------------|-------|
| [Claude for Legal](https://github.com/anthropics/claude-for-legal) | Apache-2.0 | Python | Anthropic's reference suite of 13 practice-area plugins and 70+ named agents for legal workflows (commercial, corporate, employment, privacy, IP, litigation, and more); installable as Claude plugins or deployed via Managed Agents API; features cold-start interviews, practice profiles (CLAUDE.md), 20+ MCP connector integrations (Ironclad, DocuSign, iManage, Westlaw), and scheduled monitoring agents for regulatory feeds, renewals, and dockets; all outputs are attorney-review drafts | [GitHub](https://github.com/anthropics/claude-for-legal) |
| [Mike](https://github.com/willchen96/mike) | AGPL-3.0 | TypeScript | Open-source AI legal platform with Next.js frontend and Express backend; integrates Supabase Auth + Postgres, S3-compatible storage, and LibreOffice for DOC/DOCX-to-PDF conversion | [GitHub](https://github.com/willchen96/mike) |
| [Suzie Law](https://github.com/firelex/suzielaw) | MIT | TypeScript | Open-source alternative to Harvey; legal AI workspace with counsel chat, 12 practice-area personas, 160+ agentic prompt recipes, document Q&A, DOCX drafting, RAG knowledge base, CourtListener case-law research, and local model support; built on the Team Suzie agent platform | [GitHub](https://github.com/firelex/suzielaw) · [Site](https://suzielaw.com) |



### 1b — Data

Ingestion, parsing, RAG, NLP, and output validation for legal document corpora.

| Name | License | Language | Description | Links |
|------|---------|----------|-------------|-------|
| [legal-sources](https://github.com/worldwidelaw/legal-sources) | AGPL-3.0 | Python | 243 collection scripts for open legal data from 50+ countries (EU, EFTA, UK, US, CA and more); standardized scrapers for legislation and case law from official government portals and APIs; normalizes to a common schema; powers the Legal Data Hunter search API (6M+ documents indexed) | [GitHub](https://github.com/worldwidelaw/legal-sources) · [Dashboard](https://legaldatahunter.com) |
| [Water Law Dataset](https://github.com/jrklaus8/water-law-dataset) | MIT | Python | 83,596 water law judicial decisions from Brazil (27 state courts), Canada (CanLII API), and the Netherlands (Rechtspraak); includes scrapers, a regex-based jurimetric coding engine (21 categories, 4 languages), and merge utilities; academic research dataset 2016–2026 | [GitHub](https://github.com/jrklaus8/water-law-dataset) · [Dashboard](https://jrklaus8.github.io/water-law-dataset/) · [Zenodo](https://doi.org/10.5281/zenodo.19836413) |



### 1c — Word (DOCX)

Libraries for generating, editing, and templating Word documents.

| Name | License | Language | Description | Links |
|------|---------|----------|-------------|-------|
| [Adeu](https://github.com/dealfluence/adeu) | MIT | Python / TypeScript | Bidirectional docx ↔ LLM translator that converts Word documents to Markdown for AI editing and applies changes back as native Track Changes; preserves existing formatting, fonts, and layout; available as an MCP server for Claude, Gemini, and Cursor; supports live Word integration on Windows and optional Adeu Cloud integration | [GitHub](https://github.com/dealfluence/adeu) |
| [Docling](https://ds4sd.github.io/docling/) | MIT | Python | IBM document parsing library; converts PDF, DOCX, PPTX, XLSX, HTML, images, LaTeX, and audio to Markdown, HTML, or lossless JSON; advanced PDF understanding (layout, reading order, tables via TableFormer, formulas, image classification); also available as a REST API via docling-serve | [GitHub](https://github.com/docling-project/docling) |
| [python-docx](https://python-docx.readthedocs.io/) | MIT | Python | Create, read, and modify Word 2007+ (.docx) files programmatically; supports paragraphs, headings, tables, images, styles, headers, and footers | [GitHub](https://github.com/python-openxml/python-docx) |
| [docxtpl](https://docxtpl.readthedocs.io/) | MIT | Python | Uses a .docx file as a Jinja2 template; supports variables, loops, conditionals, inline images, table cell merging (colspan), subdocuments, and custom Jinja2 filters; templates are authored directly in Word | [GitHub](https://github.com/elapouya/python-docx-template) |
| [Mammoth](https://github.com/mwilliamson/mammoth.py) | BSD-2 | Python / JS | Converts .docx to clean semantic HTML or Markdown by mapping Word paragraph styles to HTML elements; supports customizable style mappings, inline or file-based image export, and raw text extraction; available in Python, JavaScript, Java, and .NET | [GitHub](https://github.com/mwilliamson/mammoth.py) |
| [OfficeCLI](https://github.com/iOfficeAI/OfficeCLI) | Apache-2.0 | C# | Self-contained CLI tool for AI agents to create, read, and modify .docx, .xlsx, and .pptx files without Microsoft Office; path-based element addressing, JSON output, `{{key}}` template merge, 150+ Excel formula evaluation, pivot table generation, native HTML/PNG rendering, MCP server integration, and batch atomic transactions; single binary with embedded .NET runtime; cross-platform | [GitHub](https://github.com/iOfficeAI/OfficeCLI) |


---

## Part 2 — General Open Source (Useful in Legal Contexts)



### 2a — Agentic Capabilities
| Name | License | Language | Description | Links |
|------|---------|----------|-------------|-------|
| [LangGraph](https://langchain-ai.github.io/langgraph/) | MIT | Python | Low-level orchestration framework for building stateful, long-running agents as graphs (inspired by Pregel); features durable execution with automatic resume after failure, human-in-the-loop state inspection, first-class streaming (token-by-token and intermediate steps), and fully customizable primitives — usable without LangChain | [GitHub](https://github.com/langchain-ai/langgraph) |
| [CrewAI](https://www.crewai.com/) | MIT | Python | Framework for orchestrating role-playing, autonomous AI agents that collaborate in crews; agents are assigned roles, goals, and tools; supports sequential and hierarchical task execution, inter-agent delegation, and 100+ tool integrations | [GitHub](https://github.com/crewAIInc/crewAI) |
| [AutoGen](https://microsoft.github.io/autogen/) | MIT | Python | Microsoft's event-driven, scalable multi-agent framework (v0.4); includes AgentChat (conversational single/multi-agent apps), AutoGen Studio (no-code GUI for rapid prototyping), and modular components for memory, tools, and custom agents — note: being merged into Microsoft Agent Framework | [GitHub](https://github.com/microsoft/autogen) |
| [Agno](https://docs.agno.com/) | MPL-2.0 | Python | Full-stack runtime for building and deploying multi-agent systems; agents support memory, knowledge bases, structured I/O schemas, guardrails, MCP, and 100+ toolkits; includes a stateless FastAPI backend, channel integrations (Slack, Telegram, WhatsApp, Discord), cron scheduling, and an AgentOS control plane for monitoring | [GitHub](https://github.com/agno-agi/agno) |
| [LlamaIndex](https://www.llamaindex.ai/) | MIT | Python | Framework for building LLM-powered agents and document pipelines; covers parsing (LlamaParse), RAG ingestion and indexing, structured data extraction, and deployed document agents; 300+ integration packages for LLMs, embeddings, and vector stores via LlamaHub | [GitHub](https://github.com/run-llama/llama_index) |
| [Haystack](https://haystack.deepset.ai/) | Apache-2.0 | Python | AI orchestration framework for building production-ready LLM pipelines and agent workflows with explicit control over retrieval, routing, memory, and generation; modular components with conditional logic and branching; model-agnostic (OpenAI, Anthropic, Mistral, HuggingFace, AWS Bedrock, local models); exposes pipelines via HTTP or MCP through Hayhooks | [GitHub](https://github.com/deepset-ai/haystack) |

### 2b — Search Engines
| Name | License | Language | Description | Links |
|------|---------|----------|-------------|-------|
| [Meilisearch](https://www.meilisearch.com/) | MIT | Rust | Fast, typo-tolerant search engine API; supports hybrid search (semantic + full-text), filtering, sorting, geosearch, and faceting; sub-50ms search-as-you-type; replicated sharding for horizontal scaling | [GitHub](https://github.com/meilisearch/meilisearch) |

### 2c — Databases
| Name | License | Language | Description | Links |
|------|---------|----------|-------------|-------|
| [Weaviate](https://weaviate.io/) | BSD-3 | Go | Open-source vector database storing objects and vectors together; supports hybrid search (BM25 + semantic), built-in generative search (RAG), automatic vectorization or pre-computed embeddings, multi-tenancy, RBAC, and vector quantization for memory efficiency | [GitHub](https://github.com/weaviate/weaviate) |
| [Qdrant](https://qdrant.tech/) | Apache-2.0 | Rust | Vector search engine supporting dense, sparse, and multivector representations; rich JSON payload filtering (keyword, full-text, numeric, geo, boolean); hybrid search with RRF/DBSF fusion; quantization reducing RAM usage up to 97%; zero-downtime scaling with sharding and replication | [GitHub](https://github.com/qdrant/qdrant) |
| [Supabase](https://supabase.com/) | Apache-2.0 | TypeScript | Postgres development platform bundling a hosted database, auto-generated REST and GraphQL APIs, Auth, Realtime subscriptions, file storage, and an AI/vector toolkit (pgvector); self-hostable; data API built on PostgREST | [GitHub](https://github.com/supabase/supabase) |

### 2d — Model Deployment
| Name | License | Language | Description | Links |
|------|---------|----------|-------------|-------|
| [Ollama](https://ollama.com/) | MIT | Go | Run open-weight LLMs locally via a single command; manages model quantization and GPU memory automatically; exposes an OpenAI-compatible REST API at localhost; supports Docker deployment and a wide model library (Llama, Qwen, DeepSeek, Gemma, and more) | [GitHub](https://github.com/ollama/ollama) |
| [vLLM](https://docs.vllm.ai/) | Apache-2.0 | Python | High-throughput, memory-efficient LLM inference engine; features PagedAttention, continuous batching, prefix caching, and quantization (GPTQ/AWQ/INT4/INT8/FP8); supports tensor, pipeline, and expert parallelism; runs on NVIDIA/AMD GPUs, CPUs, TPUs, and Apple Silicon; OpenAI-compatible API; 200+ Hugging Face model architectures | [GitHub](https://github.com/vllm-project/vllm) |
| [LiteLLM](https://docs.litellm.ai/) | MIT | Python | AI Gateway and Python SDK providing a unified OpenAI-compatible interface to 100+ LLM providers (Anthropic, Bedrock, Azure, Vertex AI, HuggingFace, vLLM, NVIDIA NIM, and more); features load balancing, fallback/retry logic, virtual keys, per-user/team spend tracking, guardrails, caching, and an admin dashboard; deployable as a self-hosted proxy server | [GitHub](https://github.com/BerriAI/litellm) · [Agent Platform](https://github.com/BerriAI/litellm-agent-platform) |

### 2e — Model Safety
| Name | License | Language | Description | Links |
|------|---------|----------|-------------|-------|
| [Guardrails AI](https://www.guardrailsai.com/) | Apache-2.0 | Python | Framework for adding input/output validation to LLM applications; uses a RAIL (Reliable AI Markup Language) spec to define structure, types, and validators; Guardrails Hub provides pre-built validators for jailbreak detection, PII anonymization, hallucination detection, prompt-leakage checks, and output schema conformance | [GitHub](https://github.com/guardrails-ai/guardrails) |
| [Garak](https://garak.ai/) | Apache-2.0 | Python | LLM vulnerability scanner using static, dynamic, and adaptive probes; sends targeted prompts to models, collects stochastic generations, and runs detectors (keyword-based or classifier-based) to identify failure modes such as broken alignment, harmful output, and prompt injection; includes automated attack generation via a red-teaming LLM; produces JSONL reports with full prompt/response/score tracing | [GitHub](https://github.com/NVIDIA/garak) |
| [NeMo Guardrails](https://github.com/NVIDIA-NeMo/Guardrails) | Apache-2.0 | Python | Toolkit for adding programmable guardrails to LLM applications using Colang, a Python-like domain-specific language for dialogue flow design; supports input rails, dialog rails, retrieval rails (for RAG), and output rails; IORails engine enables parallel execution; integrates with LangChain and major LLM providers | [GitHub](https://github.com/NVIDIA-NeMo/Guardrails) |

### 2f — Self-Hosted AI Workspaces

General-purpose, self-hostable AI chat platforms with RAG, agents, and document intelligence — deployable on-premises for data-sensitive environments.

| Name | License | Language | Description | Links |
|------|---------|----------|-------------|-------|
| [Onyx (FOSS)](https://github.com/onyx-dot-app/onyx-foss) | MIT | Python / TypeScript | Self-hostable AI chat platform (100% MIT auto-sync of the main Onyx repo); features agentic RAG with hybrid search, deep research (multi-step), custom agents, 50+ connectors, MCP, web search, code execution, voice mode, image generation, SSO (OAuth/OIDC/SAML), RBAC, and usage analytics; deployable via Docker, Kubernetes, or Helm | [GitHub](https://github.com/onyx-dot-app/onyx-foss) · [Docs](https://docs.onyx.app) |
| [AnythingLLM](https://github.com/Mintplex-Labs/anything-llm) | MIT | JavaScript | All-in-one desktop and Docker AI application; RAG over any document type, native multi-step tool-calling agents, multi-user support with per-user access controls, 30+ LLM provider integrations, Telegram bot integration, and a browser extension; runs fully locally with no mandatory cloud dependency | [GitHub](https://github.com/Mintplex-Labs/anything-llm) · [Site](https://anythingllm.com) |

---

## Notes

- **License legend:** MIT / Apache-2.0 = permissive · GPL / AGPL = copyleft · Fair-code = source-available with usage restrictions
- Add new entries by duplicating a row and filling in all columns.
