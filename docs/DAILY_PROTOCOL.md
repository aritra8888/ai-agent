# Daily Protocol

## Start

Message:

```text
Today is Day X. Start my learning session.
```

GPT must produce:

- topics
- why it matters
- 2-hour plan
- first concept teaching
- checkpoint questions
- build/exercise
- done condition

## During the day

Use the same chat for questions, explanations, debugging, and problem solving.

## End

Message:

```text
End Day X.
```

GPT must ask for completion details, then produce updated repo files and a commit message.

## Commit

```bash
git add progress logs summaries problems artifacts
git commit -m "Complete Day X learning session"
git push origin main
```
