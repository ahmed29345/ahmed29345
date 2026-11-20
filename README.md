## Muhammad Ahmed Raza Memon

**Senior AI Engineer (Agentic AI & RAG) · Software Architect · Full-Stack & Mobile Engineer**
Al-Madinah Al-Munawwarah, Saudi Arabia · 10+ years building SaaS, B2B and government-sector platforms

I build production-grade agentic AI in Python (RAG over Arabic and English documents, LangGraph multi-agent workflows with human approval, LLM evaluation, guardrails and observability) and I design and ship complete products: backend and database, Flutter apps for iOS and Android, React front ends, cloud deployment, and LLM assistants that act on live data under role-based permissions. Most of my work is private client code; the repositories below are small open-source pieces of the same ideas.

### Featured: Mizan, an agentic AI compliance copilot

[**Mizan**](https://github.com/ahmed29345/mizan) is an Arabic/English assistant for Saudi financial regulations (SAMA, ZATCA, PDPL; fictional demo data). It answers questions with verified citations and runs a multi-agent compliance review that a human officer approves.

- **RAG:** semantic search with bge-m3 embeddings and pgvector (HNSW); English questions find Arabic articles; citations are checked against what was actually retrieved.
- **Agents:** LangGraph agent with tool calling, plus a multi-agent review (document reader → 3 parallel regulation checkers → report writer) that pauses for human approval, with a Postgres checkpointer.
- **Evaluation and safety:** 26-question golden set including Arabic and prompt-injection attacks: 26/26 passing, 100% retrieval recall, 0 hallucinated citations; code-level guardrails that fail closed.
- **Production practice:** FastAPI, 95 tests, GitHub Actions CI, self-hosted Langfuse tracing, non-root Docker image, Kubernetes with zero-downtime rolling updates, bilingual web UI, open-source models running locally.

### Products I built

| Product | What it is | Stack |
| --- | --- | --- |
| [mi day](https://mi-day.net) | Multi-tenant SaaS for nurseries, schools and academies in Saudi Arabia, with an AI assistant, ZATCA-ready finance and a parents' app | Laravel, MySQL, Flutter, React SSR, OpenAI/Ollama |
| [AlMasjidi](https://almasjidi.com) | Prayer and iqama times for 335,000+ mosques worldwide, azan alerts, mosque committee SaaS, 18 languages | Laravel, Filament, Flutter, DuckDB |
| [Shababe apps](https://shababe.com) | Urdu, Bangla, Hindi and Saudi news and Urdu recipes apps: 75,000+ downloads, rated 4.1–4.2 | Flutter, Laravel, Firebase |
| Faaya | Multi-store e-commerce platform with local payment gateways and courier APIs | Laravel, MySQL, Flutter |

### Open source

| Repository | What it shows |
| --- | --- |
| [mizan](https://github.com/ahmed29345/mizan) | Agentic AI compliance copilot in Python: RAG with pgvector, LangGraph multi-agent review with human approval, evaluation, guardrails and Langfuse tracing, deployed with Docker and Kubernetes. |
| [llm-tool-calling-php](https://github.com/ahmed29345/llm-tool-calling-php) | An LLM agent loop where the model only sees, and can only run, the tools the user is allowed to use. OpenAI and Ollama drivers. |
| [laravel-tenant-rbac](https://github.com/ahmed29345/laravel-tenant-rbac) | Multi-tenant roles and permissions for Laravel: one user, different roles per organization, data that never crosses tenants. |
| [zatca-qr](https://github.com/ahmed29345/zatca-qr) | Typed TypeScript encoder and decoder for the ZATCA e-invoice QR (TLV + Base64), with correct Arabic byte lengths. |
| [laravel-wathq](https://github.com/ahmed29345/laravel-wathq) | Laravel client for Wathq commercial registration checks, with a validation rule, caching and an artisan command. |

### Stack

**Backend:** Laravel, PHP 8, NestJS, Node.js, REST/B2B APIs, multi-tenant SaaS
**Mobile & web:** Flutter, Firebase, React, Next.js, Angular, TypeScript, Arabic/RTL UI
**Data:** MySQL, PostgreSQL, Oracle, MongoDB, Redis, Prisma
**AI:** Python, FastAPI, LangGraph (multi-agent, human-in-the-loop), RAG, embeddings (bge-m3), pgvector, LLM evaluation, guardrails, Langfuse, LLM tool calling, OpenAI, Ollama, speech-to-text
**Saudi integrations:** ZATCA e-invoicing, Wathq, local payment gateways, WhatsApp/SMS
**Cloud:** AWS, STC Cloud / Alibaba Cloud, Docker, Kubernetes, GitHub Actions

### Contact

[LinkedIn](https://www.linkedin.com/in/ahmedrazayounus/) · [arymatic.com](https://arymatic.com) · Saudi Council of Engineers member
