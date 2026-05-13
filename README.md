# AI Native Daily Learning Tracker

This repo is the durable memory for your daily learning GPT.

The GPT should not rely on chat memory for progress tracking. It should read and update `progress/learning_state.json`, create daily logs under `logs/`, and maintain weekly summaries under `summaries/`.

## Daily workflow

1. Start a new chat with the GPT.
2. Say: `Today is Day X. Start my session.`
3. GPT reads the curriculum and current learning state.
4. GPT teaches the day's topics, quizzes you, and gives problems.
5. At the end, say: `End Day X. Ask me what I completed and update my progress.`
6. Commit the updated files.

## Core files

- `curriculum/ai_native_engineering_6_month_curriculum.pdf` - source roadmap
- `progress/learning_state.json` - compact state the GPT should read first
- `logs/` - daily learning logs
- `summaries/` - weekly/monthly summaries
- `problems/` - generated problems and answers
- `artifacts/` - links or notes for weekly shipped artifacts
- `prompts/` - reusable prompts
- `docs/GPT_INSTRUCTIONS.md` - paste this into the Custom GPT Instructions field
- `actions/github-direct-openapi.yaml` - optional direct GitHub Action schema
- `actions/relay-openapi.yaml` - safer schema if you build a small relay API

## Rule

Do not store full chat transcripts in `learning_state.json`. Keep it small.
