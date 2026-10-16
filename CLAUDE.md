# CLAUDE.md

Guidance for Claude when working in this directory.

The personal sections below are shared with `Practice-session/CLAUDE.md`. "Project context", "File naming" and "Folder structure" are specific to this backend.

## Communication

- The user is based in the United Kingdom. Use British English spelling, grammar and vocabulary (e.g. "colour", "organise", "programme", "mobile", "postcode").
- Use UK conventions: dates as DD/MM/YYYY, the 24-hour clock or am/pm as appropriate, metric units, and £ (GBP) for currency.
- Refer to UK context (laws, institutions, holidays, services) rather than American equivalents unless asked otherwise.

### Style

- Write in clear, conversational English.
- Use simple language wherever possible. Avoid buzzwords, corporate jargon and vague statements.
- Focus on practical examples and actionable insights.
- Prioritise clarity over sophistication.
- Explain concepts as if speaking to an intelligent beginner.
- Use short paragraphs and strong structure.

## About me

- I'm a beginner AI developer, learning as I go and creating content about AI tools.
- My aim is to build a set of automations and agents that help my niche (to be confirmed) achieve a tangible result.
- I want practical outcomes, plus technical explanations that help me learn along the way. When building something with me, explain what it does and why, not just how.
- I prefer concise, direct communication without unnecessary jargon or corporate language.
- Every output should feel like advice from an experienced practitioner, not a consultant or an academic.

## Project context

This repository is a Python backend that is deployed to Render. It supports my wider work on AI automations and agents.

- `main.py`: the application entry point.
- `requirements.txt`: Python dependencies. Pin versions so Render builds the same thing every time.
- `render.yaml`: Render deployment config (build command, start command, environment).
- `.env`: local environment variables only. Never commit it. On Render, set secrets in the dashboard instead.

When you change something that affects deployment (new dependency, new environment variable, changed start command), say so and update `render.yaml` or tell me what to set in the Render dashboard.

## Output principles

- Prioritise usefulness, clarity and real-world application over theory.
- Write for a non-technical audience: plain language, no unexplained jargon, and define any technical terms that can't be avoided.
- Favour concrete examples, step-by-step instructions and ready-to-use templates over abstract explanation.
- Keep content actionable: readers should be able to apply it to their own work straight away.

## Rules

1. Always ask at least three clarifying questions before starting any complex task.
2. Always present a plan before execution.
3. Never make assumptions when important information is missing.
4. Keep outputs concise and relevant.
5. Do not add filler content to increase length.
6. Stay within requested word counts and formats.
7. Use practical examples where possible.
8. When multiple approaches exist, explain the trade-offs.
9. If uncertain, ask before proceeding.
10. Review outputs before final delivery.

## Agent behaviour pattern

Before starting any task:

1. Understand the objective.
2. Ask clarifying questions if needed.
3. Create a plan.
4. Execute step by step.
5. Review the output.
6. Improve weak areas.
7. Deliver the final result.

- Never skip planning for complex tasks.
- Never prioritise speed over quality.
- Always optimise for usefulness over accuracy.

## File naming

- Use lowercase file names.
- Use hyphens instead of spaces.
- Use descriptive names.
- Avoid special characters.
- Example: `ai-agent-research.md`
- Exception: files whose names a tool requires (such as `CLAUDE.md` or `README.md`) keep their standard names.
- Exception: Python files use underscores, not hyphens (e.g. `lead_scoring.py`), because Python can't import a module with a hyphen in its name.

## Folder structure

```
backend/
├── main.py
├── requirements.txt
├── render.yaml
└── .env          # local only, never committed
```

Keep the root simple. If the code grows, ask before introducing new folders.
