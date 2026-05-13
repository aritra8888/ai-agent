# AI Agent Learning Monorepo

This repository tracks my 6-month AI-native engineering curriculum.

## Goal

Build real AI-native engineering skill through daily implementation, failure notes, Git commits, and weekly working artifacts.

The target is to become strong at:

- LLM APIs
- Structured outputs
- Tool calling
- RAG
- Agents
- MCP
- Evals
- Observability
- AI security
- Production AI architecture

## Repo Structure

- apps/web: frontend app for chat UI, traces, dashboards, and approvals
- apps/api-node: Node/TypeScript API gateway
- apps/ai-python: Python/FastAPI AI service
- packages/shared: shared schemas, types, and validation
- packages/tool-gateway: tool execution, policy, audit, and approval layer
- datasets/evals: evaluation datasets and test cases
- docs: architecture notes, diagrams, setup notes, and threat models
- logs: daily learning logs
- problems: daily practice problems
- progress: compact learning state used by the mentor GPT
- summaries: weekly summaries and compression notes

## Daily Workflow

1. Start the day with the mentor GPT.
2. Paste the current `progress/learning_state.json`.
3. Read the day plan.
4. Learn the required concept.
5. Build the required artifact.
6. Write failure notes.
7. End the day with the mentor GPT.
8. Copy generated files into this repo.
9. Commit and push.

## Progress Tracking

The file `progress/learning_state.json` is the source of truth for progress tracking.

The Custom GPT does not directly write to GitHub yet. It generates files, and I manually copy them into the repo.

## Rules

- Day 0 is setup only.
- Curriculum Day 1 starts after setup is complete.
- Every learning day must end with a Git commit.
- Do not commit secrets.
- Use `.env.example`, never `.env`.
- Keep progress state compact.
- Keep failure notes honest.
