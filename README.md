# AI-Agents

Monorepo for the **AI Software Engineer Agent** — an event-driven multi-agent system that automates software engineering tasks through natural language interaction.

| Project | Stack | Docs |
|---|---|---|
| `ai_software_agent/` | Python 3.12 · LangGraph · FastAPI · ChromaDB | [README](ai_software_agent/README.md) |
| `ai_software_web/` | Next.js 14 · TypeScript · Material UI (MUI v6) | [README](ai_software_web/README.md) |

## Quickstart

```bash
# Terminal 1 — backend API (http://localhost:8000)
cd ai_software_agent
python3.12 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
cp .env.example .env
python -m app.main --serve --port 8000

# Terminal 2 — web UI (http://localhost:3000)
cd ai_software_web
npm install
cp .env.example .env.local
npm run dev
```

See each project's README for full installation, configuration, API contract (`GET /health`, `POST /v1/run` SSE), testing, deployment, and troubleshooting.
