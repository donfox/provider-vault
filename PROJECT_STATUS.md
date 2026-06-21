# provider_vault - Project Status

## Status: ✅ OPERATIONAL

**Purpose**: Educational polyglot microservices demonstrating AI engineering patterns

## Architecture
```
Phoenix Web (Elixir, Port 4000)
         ↓ HTTP
FastAPI Service (Python, Port 8000)
         ↓ SQL
PostgreSQL (localhost:5432)
```

## Components

### Phoenix Web App (Elixir/Erlang)
- Framework: Phoenix 1.7+ with LiveView
- Status: Compiled successfully, running on localhost:4000
- Dependencies: All resolved (heroicons, bandit, etc.)

### AI Service (Python FastAPI)
- Framework: FastAPI 0.128+ with Uvicorn
- Port: 8000
- Features: 6 AI functions using OpenAI gpt-4o-mini
  * Specialty descriptions
  * Related specialties finder
  * Provider distribution analysis
  * Symptom triage
  * Semantic search
  * FAQ chatbot with RAG
- Status: Fully operational with all dependencies installed

## Dependencies

**Python** (in venv): fastapi, uvicorn, openai, psycopg2-binary, python-dotenv

**Services**: PostgreSQL on localhost:5432, OpenAI API key in `.env`

## Run Command
```bash
./start.sh
```
