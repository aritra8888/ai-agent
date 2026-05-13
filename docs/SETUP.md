# Setup

## 1. Create GitHub repo

Recommended repo name: `ai-native-learning-tracker`.

CLI path:

```bash
gh auth login
gh repo create ai-native-learning-tracker --private --clone
cd ai-native-learning-tracker
```

Copy this starter pack into the cloned repo, then run:

```bash
git add .
git commit -m "Initialize AI-native learning tracker"
git push origin main
```

## 2. Create Custom GPT

1. Open ChatGPT on web.
2. Go to Explore GPTs.
3. Click Create.
4. Use Configure mode.
5. Paste `docs/GPT_INSTRUCTIONS.md` into Instructions.
6. Upload `curriculum/ai_native_engineering_6_month_curriculum.pdf` as Knowledge.
7. Add conversation starters from the main answer.
8. Test Day 1 in Preview.
9. Save as private.

## 3. Add GitHub linking

Beginner-safe path: no Action. Paste `progress/learning_state.json` into the first message and manually commit GPT outputs.

Automated path: configure a GPT Action using either:

- `actions/github-direct-openapi.yaml` for direct GitHub API access
- `actions/relay-openapi.yaml` if you build a small API relay

Use a fine-grained GitHub token restricted to this repo only. Minimum permissions for direct GitHub action:

- Contents: read/write
- Issues: read/write only if using issue creation

Do not paste the token in chat.
