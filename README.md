# Harsh Gavand

**Full-stack, backend & AI engineering**

I build Python and TypeScript applications: backend APIs, data workflows, web interfaces, and AI features with application-controlled state and permissions. My work includes internal quotation, invoice, and email automation tools, community platforms, retrieval systems, and agents with deterministic execution rules.

Mumbai, India · **Open to remote Full-Stack Developer, Backend Engineer, and AI Engineer roles.**

[Portfolio](https://harshgavand.dev/) · [LinkedIn](https://www.linkedin.com/in/harsh-gavand) · [Email](mailto:harsh.gavand.tech@gmail.com)

[![XERJ Corpus Hub contributor](https://hub.xerj.org/contributors/harshgavandit/badge.svg)](https://hub.xerj.org/contributors/harshgavandit)

**Selected for the XERJ Corpus Hub:** Agri Samaj's bilingual AI chat and voice implementation is included as a searchable reference for AI coding agents. [View the selection](https://hub.xerj.org/contributors/harshgavandit) · [Explore the repository corpus](https://hub.xerj.org/corpus/harshgavandit--agri-samaj-community-platform).

Start with **[Docwise](https://github.com/harshgavandit/rag-documentation-assistant)** for retrieval and AI evaluation, the **[backend scaling lab](https://github.com/harshgavandit/Advanced-System-Design-Implementation-/tree/main/season-1/2.vertical-vs-horizontal-scaling)** for durable jobs and failure recovery, or **[Agri Samaj](https://github.com/harshgavandit/agri-samaj-community-platform)** for community product delivery. The scaling lab is a local study implementation; cloud deployment and a sustained production SLO remain open.

## Selected engineering work

| Project | What to inspect | Try it |
| --- | --- | --- |
| [Banking Agent Harness](https://github.com/harshgavandit/banking-agent-harness) | Python policy checks and explicit later-turn confirmation around agent-selected mock transfers; isolated Redis-backed sessions and regression tests. | [Mock banking demo](https://banking-agent-harness.vercel.app) |
| [Symposium RAG & Semantic Cache](https://github.com/harshgavandit/RAG-Semantic-Cache-Symposium-Bot) | Document-grounded answers with page references, exact and semantic Redis caching, and source-aware cache namespaces. | [PDF assistant](https://symposium-rag-bot.vercel.app) |
| [Docwise — Hybrid RAG](https://github.com/harshgavandit/rag-documentation-assistant) | BM25 and ONNX MiniLM retrieval combined through reciprocal rank fusion, followed by cited OpenAI answers. | [Documentation assistant](https://rag-documentation-assistant.vercel.app) |
| [Agri Samaj Community Platform](https://github.com/harshgavandit/agri-samaj-community-platform) | Marathi–English business discovery and entrepreneur registration, with Next.js, Prisma/PostgreSQL, private application workflows, and community-led requirements. | [Community platform](https://agri-samaj-community-platform.vercel.app) |
| [AgriConnect](https://github.com/harshgavandit/Agri-Connect) | Full-stack contributions to an agricultural marketplace: organisation permissions, checkout validation, administrator workflows, PostgreSQL, and AI assistance. Built on the [upstream project](https://github.com/c-PRESENTS/Agri-Connect). | [Marketplace](https://agri-connect-flame.vercel.app) |
| [Realtime Meetings](https://github.com/harshgavandit/Zoom_Clone) | Browser WebRTC media, screen sharing, room-scoped signaling, and PostgreSQL-backed signaling state with concurrency and isolation tests. | [Meeting application](https://zoom-clone-blue-pi.vercel.app) |

## Contributions you can review

My work on **c-PRESENTS/Agri-Connect** includes these merged pull requests:

- [Organisation RBAC and marketplace workflows — #15](https://github.com/c-PRESENTS/Agri-Connect/pull/15): permission middleware, organisation roles, and relational access rules.
- [Checkout validation and recovery — #19](https://github.com/c-PRESENTS/Agri-Connect/pull/19): request validation, stage-aware error handling, and checkout retry behaviour.
- [Administrator control-centre work — #25](https://github.com/c-PRESENTS/Agri-Connect/pull/25): administrator and security-management interfaces.

All three have upstream maintainer approvals and merges: [#15 review](https://github.com/c-PRESENTS/Agri-Connect/pull/15#pullrequestreview-4910231608), [#19 review](https://github.com/c-PRESENTS/Agri-Connect/pull/19#pullrequestreview-4969400068), [#25 review](https://github.com/c-PRESENTS/Agri-Connect/pull/25#pullrequestreview-5049290461).

Agri Samaj is a community project that I maintain and extend around the community's requests. My previous full-time work at **GlobeTrek Engineering Corporation** included delivering full-stack applications and tools for quotation building, invoice generation, and automated email sending. Earlier work at **HRP Enterprises** involved React, Node.js, Express, REST APIs, and database-backed application features.

## Tech stack

My primary application stack is **Python, TypeScript, React, FastAPI, Node.js, PostgreSQL and Redis**. The repositories also use the broader tools listed here; cloud reference work and local scaling experiments are identified in their documentation.

- **Frontend & interfaces:** React, Next.js, TypeScript, JavaScript ES6+, HTML, CSS, Tailwind CSS, accessible UI and state management.
- **Backend & APIs:** Python, Node.js, Express, Django, Django REST Framework, Flask, FastAPI, REST APIs, asynchronous tasks and data pipelines.
- **Authentication & realtime:** JWT, Clerk, role-based access control, Socket.IO, WebRTC and webhooks.
- **Databases & persistence:** PostgreSQL, MySQL, MongoDB, Redis, SQLite, SQL, Prisma, Sequelize, Mongoose, SQLAlchemy, vector databases and database migrations.
- **Applied AI & ML:** OpenAI APIs, Google AI / Gemini, Google ADK, LangChain, LangGraph, RAG, embeddings, BM25, ONNX, semantic caching, TensorFlow, Keras, Pandas and NumPy.
- **Cloud & delivery:** Docker, Docker Compose, AWS, Linux, Vercel, Cloudinary, GitHub Actions and CI/CD.
- **Testing & engineering tools:** Git, GitHub, Postman, automated tests, k6, Grafana and application logging.

[Explore the stack and project examples on my portfolio](https://harshgavand.dev/#skills).

## Measurements and failure handling

- **[Docwise evaluation](https://github.com/harshgavandit/rag-documentation-assistant/tree/main/evaluation):** 112 source-labelled intents compare BM25, vector and hybrid retrieval. Separate real-model runs inspect cited answers, refusals, instruction attacks, conflicting evidence and ambiguous questions. Results retain misses, a regex false negative and actual token usage.
- **[Multi-domain diagnostic](https://github.com/harshgavandit/rag-documentation-assistant/blob/main/evaluation/BROADER_RESULTS.md):** five application domains, frozen development/held-out query splits, 60 retrieval cases and 24 additional real-model attempts. The timeout and strict-refusal mismatch remain visible; labels are AI-reviewed, with external human review still open.
- **[Cache workloads and recovery](https://github.com/harshgavandit/RAG-Semantic-Cache-Symposium-Bot/tree/main/benchmarks):** a historical 9,000-operation local SQLite workload and a new 300-operation run with raw timings and an offline percentile verifier. Recovery checks cover TTL, eviction, contention and connection lifetime. A separate bounded live Redis check verifies admission and expiry; SQLite timings do not measure the hosted Redis cache.
- **[Hosted failure-path checks](https://github.com/harshgavandit/rag-documentation-assistant/blob/main/operations/HOSTED_WORKLOAD.md):** 16 requests exercised real Vercel, Redis and ONNX boundaries with an injected model provider. Recorded cases cover concurrent admission, quota expiry, upstream failures and usage accounting; they do not measure live-model latency or sustained service capacity.
- **[Operating Docwise](https://github.com/harshgavandit/rag-documentation-assistant/tree/main/operations):** protected health/schema checks scheduled every six hours, separate synthetic/visitor cohorts, returned-token accounting and optional one-use answer feedback. No question text or visitor identity is retained.

The repositories include the datasets, commands, source fingerprints and recorded outputs. These are controlled development runs; they do not represent customer traffic or a production incident history.

## More work

- [System-design study & scaling lab](https://github.com/harshgavandit/Advanced-System-Design-Implementation-): runnable backend experiments with load generation and observability.
- [UGC Content Studio](https://github.com/harshgavandit/ugc-project): authenticated image-generation workflows, media storage, and credit handling.
- [Stock Prediction Portal](https://github.com/harshgavandit/Stock-Prediction_Portal_Python_ML): Django REST/JWT accounts, personal watchlists, market charts, and NumPy inference from exported LSTM weights.
- [AI News to Email Generator](https://github.com/harshgavandit/AI_News_To_Email_Generator): RSS collection, personalized digest previews, HTML export, and owner-authorized Gmail delivery.
- [Portfolio source](https://github.com/harshgavandit/Harsh-Gavand-PortFolio-Website): the site, case studies, and its AI assistant and tools.

For a remote role or an engineering collaboration, reach me at **[harsh.gavand.tech@gmail.com](mailto:harsh.gavand.tech@gmail.com)**.
