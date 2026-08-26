# 🚀 Vikas Kumar’s AI & Engineering Projects

A curated selection of projects demonstrating my work across **GenAI product engineering, agentic systems, LLM infrastructure, developer productivity, and distributed backend architecture**.

The portfolio is intentionally centered on systems I have designed and built rather than a generic technology list.

---

## 🏥 Gauze.md

**AI-native Clinical Decision Platform**

Gauze.md is an AI-native healthcare platform focused on applying **LLMs, RAG, agentic workflows, and multimodal AI** to clinical decision support.

### Architecture & Capabilities

- **LLM-powered clinical workflows** orchestrated with LangGraph.
- **RAG-based clinical intelligence** grounded in domain knowledge.
- **FHIR integration** for interoperable healthcare data.
- **PACS and DICOM** integration for medical imaging workflows.
- **Multimodal AI workflows** using MedLM and Vertex AI.
- Backend architecture designed for privacy, reliability, and healthcare-oriented compliance requirements.

**Focus:** Clinical AI · RAG · Agentic Workflows · FHIR · DICOM · PACS · Multimodal AI · LangGraph · Vertex AI

---

## 🛒 Commerce Copilot

**Agentic Commerce & Payment Operations Platform**

Commerce Copilot applies LLMs and agentic workflows to automate operational workflows around **payments, orders, and commerce support**.

### Engineering Impact

- Automated approximately **90% of payment and order-support workflows**.
- Uses LLM-powered reasoning combined with domain-specific tools and workflows.
- Designed around asynchronous and fault-tolerant backend services.
- Integrates operational context and transaction data to support automated resolution and actions.

**Focus:** AI Agents · Agentic Commerce · Payments · Order Management · Tool Calling · Automation · Distributed Systems

---

## ⚡ EM TaskFlow AI

**Full-Stack, Local-First Engineering Management Intelligence Platform**

**Repo:** [em-taskflow-ai](https://github.com/logsv/em-taskflow-ai)

EM TaskFlow AI combines **local LLM inference, hybrid RAG, multi-agent orchestration, MCP integrations, and engineering-management intelligence** into a single productivity platform.

### Key Architecture

- **100% local LLM inference** using Ollama for data sovereignty and privacy.
- **Hybrid RAG** using HyDE, Reciprocal Rank Fusion (RRF), HNSW vector search, and keyword retrieval.
- **Redis semantic caching** for low-latency repeated queries.
- **LangGraph multi-agent supervisor** routing work to specialized engineering-management agents.
- **Python AI/RAG service** separated from the Node.js API/backend layer.
- **MCP integrations** across Jira, Notion, GitHub, Slack, and Google Calendar.
- **Per-service database isolation** for backend, AI/RAG, workflow, and observability workloads.
- Bounded tool scopes designed to improve execution reliability with smaller local models.

**Tech Stack:** Node.js · Python · FastAPI · React · LangGraph · Ollama · PostgreSQL/pgvector · Redis · MCP · Temporal · Langfuse

---

## 🧭 LLM Router

**Provider-Agnostic LLM Routing Infrastructure**

**Repo:** [llm-router](https://github.com/logsv/llm-router)

A TypeScript-based routing layer designed to abstract multiple LLM providers and make model selection a first-class infrastructure concern.

### Key Capabilities

- **Multi-provider routing** across supported LLM backends.
- **Cost-aware model selection** for controlling inference spend.
- **Rate limiting and concurrency controls** for provider protection.
- **Retries and circuit breakers** for resilient inference.
- **Fallback routing** when providers or models become unavailable.
- **Metrics and observability** for latency, failures, usage, and routing behavior.

**Focus:** LLM Infrastructure · Model Routing · Reliability · Cost Optimization · Multi-Provider AI

---

## 🛡️ LLM Guardrails

**LLM Security, Safety & Governance SDK**

**Repo:** [llmguardrails](https://github.com/logsv/llmguardrails)

An LLM security and governance layer designed to enforce application policies around prompts, model responses, and tool execution.

### Key Capabilities

- **PII detection and masking** before sensitive data reaches model providers.
- **Secret and credential detection** to prevent accidental leakage.
- **Prompt and output validation** for configurable security policies.
- **Tool-call controls** to constrain agent capabilities.
- **Schema validation** for structured model outputs.
- **Policy-as-code** for repeatable application-level guardrails.
- Designed to be usable as an **in-process security layer** around LLM applications and agents.

**Focus:** LLM Security · AI Governance · PII Protection · Agent Security · Tool Controls · Policy Enforcement

---

## 🤖 EM Agentic Code Reviewer

**Repo:** [em-agentic-code-reviewer](https://github.com/logsv/em-agentic-code-reviewer)

An autonomous LLM-driven code review assistant for engineering teams. It analyzes diffs, generates actionable comments, and produces strategic PR summaries.

### Key Features

- Automated diff analysis from branches, staged changes, and commits.
- Multi-provider support including OpenAI, Gemini, Anthropic, and local models.
- Strategic **What / Why / Risks / Actions** PR summaries.
- GitHub Actions integration for automated review workflows.
- Customizable anti-pattern and team-specific review rules.

**Tech Stack:** Python · Ollama · LangGraph · GitHub Actions

---

## 🔗 EM Tools MCP Server

**Repo:** [em-tools-mcp-server](https://github.com/logsv/em-tools-mcp-server)

A Model Context Protocol server providing unified LLM-friendly context and actions across **Jira, Google Calendar, and Notion**.

### Key Features

- Jira issue, project, and sprint access through JSON-RPC.
- Google Calendar querying and scheduling.
- Notion page and database access.
- Session-based MCP protocol support.

**Tech Stack:** Node.js · JSON-RPC · Express · Jira API · Google Calendar API · Notion API

---

## 🧩 Engineering Themes

Across these projects, the common engineering themes are:

- **Production GenAI:** moving beyond API integrations toward complete AI-powered systems.
- **Agentic Architecture:** tool calling, bounded agents, orchestration, fallbacks, and workflow execution.
- **RAG:** hybrid retrieval, reranking, semantic caching, and domain-grounded generation.
- **LLM Infrastructure:** routing, resilience, cost optimization, observability, and provider abstraction.
- **AI Security:** PII protection, secret detection, output validation, tool governance, and policy enforcement.
- **Local-first AI:** privacy-preserving inference and smaller-model optimization with Ollama.
- **Distributed Systems:** asynchronous workflows, service isolation, event-driven architecture, and fault tolerance.

---

> *I build AI systems as production software — with architecture, reliability, security, observability, and measurable business impact.*

Connect on [LinkedIn](https://www.linkedin.com/in/logsv/) or via email: [vikas.mca.jnu@gmail.com](mailto:vikas.mca.jnu@gmail.com)
