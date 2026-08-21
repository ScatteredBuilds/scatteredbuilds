# ScatteredBuilds

My professional background is technology operations. I am building toward AI systems and platform engineering by learning how to build, integrate, deploy, secure, observe, and evaluate AI-powered systems.

My public repositories are small, inspectable learning projects. They show how I approach engineering questions; they are not claims of professional AI-engineering experience, production scale, or complete independent mastery of every implementation.

## Current public work

- [context-engine](https://github.com/ScatteredBuilds/context-engine) — local semantic retrieval for Markdown notes with threshold-based refusal and retrieval-only evaluation.
- [claude-tool-assistant](https://github.com/ScatteredBuilds/claude-tool-assistant) — a tool-calling learning project with schema validation, logging, retry and fallback handling, and workflow-contract evals.
- [interp-notebooks](https://github.com/ScatteredBuilds/interp-notebooks) — beginner interpretability study notes and toy experiments on transformer internals.

`context-engine` and `claude-tool-assistant` were built earlier in my learning with heavier AI assistance. I keep that context visible so repository polish is not mistaken for proof that I independently implemented or fully understand every detail.

## What I am learning

- Python and software engineering fundamentals
- APIs, tool use, and structured outputs
- Retrieval and data pipelines
- Testing, evaluation, and failure analysis
- Containers, CI, deployment, and observability
- Security and operational reliability for AI systems
- Interpretability as longer-term study work

## Working principles

- Define expected behavior before calling a result successful.
- Prefer deterministic checks when the requirement is deterministic.
- Preserve failures as evidence for the next iteration.
- Separate workflow-contract checks from model-quality claims.
- State what an evaluation measures and what it does not measure.
- Prefer reproducible artifacts over broad capability claims.
