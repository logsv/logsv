# 🚀 Vikas Kumar’s Open Source Projects

A curated selection of my active open-source repositories focused on AI-driven engineering productivity and GenAI tooling.

---

## 🛠️ EM TaskFlow AI

**Repo:** [em-taskflow-ai](https://github.com/logsv/em-taskflow-ai)

**Overview:**
An AI-powered productivity tool that integrates Retrieval-Augmented Generation (RAG) with your own PDF documents. Upload PDFs to build a knowledge base and chat with your documents using a local LLM (Ollama).

**Key Features:**

* **PDF Chat:** Ask questions grounded in your uploaded documents.
* **Local-first Architecture:** Uses Ollama for embeddings & LLM, ChromaDB for vector storage—no cloud dependencies.
* **Toggle UI:** Seamlessly switch between PDF Upload and Chat views.

**Quickstart:**

1. **Prerequisites:** Node.js v16+, Python 3.8+, Ollama, ChromaDB.
2. **Install:**

   ```bash
   cd backend && npm install
   cd ../frontend && npm install
   pip install chromadb
   ```
3. **Run Services:**

   * Start Ollama: `./start-ollama.sh` (ensure `deepseek-v1` models pulled)
   * Start ChromaDB: `chromadb run --path ./chroma-data`
   * Start Backend: `cd backend && npm start`
   * Start Frontend: `cd ../frontend && npm start`

**Tech Stack:** Node.js, Python, FastAPI, React, Ollama, ChromaDB

---

## 🤖 EM Agentic Code Reviewer

**Repo:** [em-agentic-code-reviewer](https://github.com/logsv/em-agentic-code-reviewer)

**Overview:**
An autonomous LLM-driven code review assistant tailored for engineering teams. It analyzes diffs, generates actionable comments, and produces strategic PR summaries.

**Key Features:**

* **Automated Diff Generation:** Pull diffs from git branches, staged changes, or specific commits.
* **Multi-Provider Support:** OpenAI, Google Gemini, Anthropic Claude, plus local models (DeepSeek R1, CodeLlama, Llama3, etc.).
* **Strategic Summaries:** “What/Why/Risks/Actions” style PR overviews.
* **GitHub Actions Integration:** Automate reviews on PR events.
* **Customizable Rules:** Define anti-pattern checks and team-specific review points.

**Usage Snippet:**

```bash
# Combined auto-review (branch vs main)
python auto_review.py --provider openai --model gpt-4

# Staged changes via local model
python auto_review.py --mode staged --provider local --model deepseek-r1
```

**Tech Stack:** Python, Ollama, LangGraph, GitHub Actions

---

## 🔗 EM Tools MCP Server

**Repo:** [em-tools-mcp-server](https://github.com/logsv/em-tools-mcp-server)

**Overview:**
A Model Context Protocol (MCP) server that provides unified LLM-friendly context from Jira, Google Calendar, and Notion for GenAI clients and automation scripts.

**Key Features:**

* **Jira Integration:** Fetch and manage issues, projects, and sprints via JSON-RPC.
* **Calendar Integration:** Query and schedule events from Google Calendar.
* **Notion Integration:** Access pages, databases, and updates from Notion.
* **Session-based Protocol:** Initialize an MCP session, then use JSON-RPC or `mcp-remote` client.

**Quickstart:**

```bash
git clone https://github.com/logsv/em-tools-mcp-server.git
cd em-tools-mcp-server
npm install
cp .env.example .env
# Set API keys in .env
npm start
```

**Tech Stack:** Node.js, JSON-RPC, Express, Jira API, Google Calendar API, Notion API

---

> *Feel free to open issues or contribute!*
> Connect on [LinkedIn](https://www.linkedin.com/in/logsv/) or via email: [vikas.mca.jnu@gmail.com](mailto:vikas.mca.jnu@gmail.com)
