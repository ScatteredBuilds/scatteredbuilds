# ScatteredBuilds

I am moving toward AI evaluation and agent reliability engineering, building on enterprise experience in testing, release readiness, infrastructure validation, governance, and production systems.

My strongest current AI work is evaluation: designing small test sets, defining pass/fail criteria, automating checks, analyzing regressions, and iterating on prompts and data quality. I am also developing deeper independent Python and software engineering skills through small, inspectable projects.

## Current work

- [agent-eval-lab](https://github.com/ScatteredBuilds/agent-eval-lab) — active build. A trajectory evaluation harness for tool-using agents: hand-written trajectory fixtures, metrics for tool selection and loop detection, pytest coverage, then baseline-vs-candidate regression checks as a CI gate. Core code in this repo is written by hand; AI is used as tutor and reviewer, not author.
- [context-engine](https://github.com/ScatteredBuilds/context-engine) — local semantic retrieval with threshold-based refusal and documented retrieval evals.
- [claude-tool-assistant](https://github.com/ScatteredBuilds/claude-tool-assistant) — a controlled tool-calling workflow with schema validation, logging, retry/fallback handling, and a small eval runner.
- [interp-notebooks](https://github.com/ScatteredBuilds/interp-notebooks) — beginner study notes and toy experiments on transformer internals and mechanistic interpretability.

context-engine and claude-tool-assistant were built earlier in my learning with heavier AI assistance. They run and I can walk through them, but agent-eval-lab is where I am proving independent implementation.

## Focus

- AI evaluation and regression testing
- Agent and tool-use reliability
- Testing, observability, and production readiness
- Retrieval and AI systems fundamentals
- Python and software engineering practice
- Longer-term study of mechanistic interpretability

These repositories are learning projects, not claims of production-scale AI systems or interpretability expertise. I try to keep the evidence visible: runnable code, explicit checks, saved failures, and clearly stated limitations.

## Working principles

- Define expected behavior before calling a result successful.
- Preserve failures as evidence for the next iteration.
- Separate small evaluation checks from benchmark claims.
- Prefer reproducible artifacts over broad capability claims.

[LinkedIn](https://www.linkedin.com/in/adamvaldezio)
