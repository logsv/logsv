# 🚀 Vikas Kumar’s AI & Engineering Projects

A curated selection of projects demonstrating my work across **GenAI product engineering, agentic systems, LLM infrastructure, developer productivity, and distributed backend architecture**.

The portfolio is intentionally centered on systems I have designed and built rather than a generic technology list.

---

## 🏥 Gauze.md

**AI-native Clinical Decision Platform**

Gauze.md is a cardiovascular AI product I launched at Fynd and built from scratch with a team of 5 engineers across ML, backend, and data. It applies **LLMs, RAG, agentic workflows, and ECG/ECHO analysis** to clinical decision support.

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

- Automated approximately **75% of support workflows** using LLMs and LangGraph over commerce APIs.
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

## 🎬 LLM Video Editor

**Prompt-Driven Video Editing for YouTube and Shorts**

**Repo:** [llm-video-editor](https://github.com/logsv/llm-video-editor)

Point it at a clip or a folder of raw footage and describe the cut you want. An LLM plans the edit; a deterministic, checkpointed pipeline audits, renders, and publishes it. Footage never leaves the machine: only text (and optionally still frames) goes to the model.

### Key Capabilities

- **Staged pipeline:** `watch → plan → b-roll → graphics / music / colour → cut-audit → take-geometry → review-gate → render → publish`, each stage writing a JSON checkpoint so re-runs reuse finished work.
- **LLM picks segment ids, never timestamps**; a deterministic cut audit snaps to word edges, completes sentences, enforces the duration budget, and applies jump-cut pacing.
- **Word-level transcription** with faster-whisper (chunked and parallel for long recordings).
- **Face-aware layout** with MediaPipe: crops, caption bands, and picture-in-picture placed to avoid faces.
- **Production render:** colour matching and looks, motion graphics, ducked licensed music, optional local AI narration, two-pass loudness normalisation to -14 LUFS, embedded chapters.
- **Upload pack:** SEO title, description, tags, and three thumbnails.
- **Two modes:** one-command `llmve auto`, or **agent mode** where Claude edits through an MCP tool server; planners via Claude, Ollama, Anthropic, or OpenAI with validated Pydantic outputs.

**Tech Stack:** Python · FFmpeg · faster-whisper · MediaPipe · Pydantic · MCP · LangGraph · Claude Code / Ollama

---

## 📊 India Stock Analyzer (long-ledger)

**Claude Code Workspace for Long-Term Indian Equity Investors**

**Repo:** [long-ledger](https://github.com/logsv/long-ledger)

A personal analysis workspace for NSE/BSE investors built on a simple principle: **code decides, Claude explains.** Claude fetches broker records, reads company documents, and explains results; a small deterministic Python core stores the data and computes every number.

### Key Capabilities

- **Read-only broker sync** via the official **Zerodha Kite and INDmoney MCP servers** and a read-only 5paisa client, with cross-broker reconciliation and no double counting.
- **Company research subagent** that reads official filings first, records each fact's source and origin, and runs fact checks (unit errors, EPS vs PAT, impossible ratios) before anything is confirmed.
- **Deterministic engine** for labels, confidence, risk flags, allocation limits, market regime (NIFTY trend, India VIX, breadth), and tax-lot views.
- **Safety by design:** order tools denied in settings, untrusted data never treated as instructions, secrets kept out of chat, restricted sites blocked.
- Trade-history imports (splits, transfers, demergers), audit log, and a local dashboard.

**Tech Stack:** Python (standard library only) · SQLite · MCP · Claude Code slash commands & subagents

---

## 🧩 Engineering Themes

Across these projects, the common engineering themes are:

- **Production GenAI:** moving beyond API integrations toward complete AI-powered systems.
- **Agentic Architecture:** tool calling, bounded agents, orchestration, fallbacks, and workflow execution.
- **RAG:** hybrid retrieval, reranking, semantic caching, and domain-grounded generation.
- **Deterministic + LLM hybrids:** LLMs plan and explain while deterministic code audits, computes, and enforces rules.
- **AI Safety by design:** read-only integrations, denied tools, untrusted-data handling, and validated structured outputs.
- **Local-first AI:** privacy-preserving inference and smaller-model optimization with Ollama.
- **Distributed Systems:** asynchronous workflows, service isolation, event-driven architecture, and fault tolerance.

---

> *I build AI systems as production software — with architecture, reliability, security, observability, and measurable business impact.*

Connect on [LinkedIn](https://www.linkedin.com/in/logsv/) or via email: [vikas.mca.jnu@gmail.com](mailto:vikas.mca.jnu@gmail.com)
