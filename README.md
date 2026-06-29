# AI Learning Notes

This repository stores my AI Engineering from Scratch learning notes and
practice files.

## Continue on a New Computer

1. Install Git and Node.js.
2. Clone this repository:

```powershell
git clone https://github.com/zhj-bot/AI-learning_zhj.git
cd AI-learning_zhj
```

3. Install the course navigation skills:

```powershell
npx.cmd --yes skills add rohitg00/ai-engineering-from-scratch
```

4. Restart Codex.
5. Ask Codex to continue from the latest lesson notes in this repository.

## Daily Learning Workflow

At the end of every study session, remember to upload local changes to GitHub.
Local files are not synced automatically. GitHub updates only after `git push`.

## End-of-Lesson Workflow

At the end of each lesson, Codex should help create or update:

- A detailed, beginner-friendly lesson note for the completed lesson.
- The `Current Progress` section in this README.
- The after-class exercises for that lesson.
- Feedback on my exercise answers, including mistakes and corrections.
- A short learning progress summary that explains what I understand well,
  what still needs review, and what lesson to study next.

After editing notes or adding practice files:

```powershell
git status
git add .
git commit -m "Update learning notes"
git push
```

## Current Progress

- Current lesson: Phase 0 Lesson 4: APIs & Keys
- Status: In progress
- Completed skills: Git basics, GitHub remote workflow, basic CPU/GPU/cloud GPU
  decision rules, API request-response basics, endpoint/API key/request
  body/response body, environment variables for API keys
- Latest exercise feedback: Correctly identified endpoint, API key, request
  body, and response body; correctly chose environment variables over hardcoded
  API keys to avoid exposing secrets on GitHub.
- Learning preference: Explain every new technical term for a zero-basis learner
  with a plain-language definition, analogy, AI engineering use case, and small
  example.
- Next step: Answer Phase 0 Lesson 4 Exercise 3 about HTTP and SDK, then
  continue to the first hands-on API call.

## Useful Commands

```powershell
git status
git log --oneline --decorate
git pull
git push
```

## Remote Repository

https://github.com/zhj-bot/AI-learning_zhj.git
