# ScatteredBuilds

I build retrieval systems, tool-calling workflows, and interpretability learning projects focused on testing, evaluation, and verification.

I learn AI engineering by building systems, documenting failures, and studying how they behave.

Current focus areas:

- Retrieval systems
- Evaluation
- Tool calling
- Validation
- Logging
- Transformer fundamentals
- Mechanistic interpretability

# Current Projects

## Context Engine

[Context Engine](https://github.com/ScatteredBuilds/context-engine) is a local retrieval system for markdown notes.

What it does:

- Loads markdown notes recursively.
- Splits notes into word-based chunks.
- Embeds chunks with `sentence-transformers`.
- Retrieves top-k chunks with cosine similarity.
- Prints source filenames.
- Refuses when the top retrieval score is below a threshold.

What was tested:

- The basic retrieval check set passed 3/3 documented checks.
- The expanded retrieval check set passed 19/20 documented checks.
- The expanded run documents one ambiguous-query failure where the expected source was not retrieved above threshold.

Known limitations:

- The current corpus uses one sample markdown note.
- The system retrieves context but does not generate a final answer.
- The confidence threshold is simple and not calibrated against a larger corpus.
- Embeddings are recomputed on each run.
- The evaluation checks retrieval behavior only, not answer quality.

## Claude Tool Assistant

[Claude Tool Assistant](https://github.com/ScatteredBuilds/claude-tool-assistant) is a command-line tool-calling assistant using Anthropic models and one local risk-classification tool.

What it does:

- Accepts a user request from the command line.
- Calls Claude through the Anthropic API.
- Exposes one local `classify_risk` tool.
- Asks for structured JSON output.
- Validates the final result with Pydantic.
- Saves raw API responses.
- Logs runs to JSONL.
- Handles retries and model fallback.

What was tested:

- Runtime output is documented in `outputs/example_run.md`.
- Model fallback behavior is documented in `outputs/model_fallback_example.md`.
- The evaluation runner checks tool execution, schema validation, output structure, retry use, and failures.
- The saved evaluation run passed 4/5 sample cases and documents one irrelevant-input failure.

Known limitations:

- The local tool uses keyword-based risk classification.
- The assistant has one local tool.
- The sample cases are not benchmark results.
- A passing eval case means the structure and tool flow worked; it does not prove answer quality.
- The current prompt and parser can fail on non-incident-style input.

## Interp Notebooks

[Interp Notebooks](https://github.com/ScatteredBuilds/interp-notebooks) contains learning notes, a notebook, and a small toy experiment focused on transformer internals.

What it contains:

- Notes on attention heads.
- Notes on the residual stream.
- A beginner notebook on attention-head intuition.
- A toy attention-routing experiment with saved output.

What it does not claim:

- It does not claim interpretability expertise.
- It does not claim research results.
- It does not inspect real model activations yet.
- It does not prove how a trained model behaves.

Known limitations:

- The current notebook and experiment use toy examples.
- Some model-specific claims are marked `TODO: VERIFY`.
- The repository does not yet include reproducible code for inspecting a trained model.
- The current artifacts are beginner-oriented learning materials.

## ai-systems-lab

[ai-systems-lab](https://github.com/ScatteredBuilds/ai-systems-lab) is an early scratchpad for smaller AI systems notes and experiments.

What it contains:

- Placeholder areas for Python foundations.
- Transformer basics.
- Retrieval experiments.
- Evaluation design.
- Inference notes.
- Interpretability notebooks.

Known limitations:

- The repository is in early buildout.
- Current evidence is mostly structure and direction.
- It should not be treated as a finished project.

# Current Focus

- Retrieval evaluation
- Tool calling
- Observability
- Reliability
- Transformer internals

# Principles

- Test assumptions.
- Document failures.
- Verify behavior.
- Prefer evidence over speculation.

# Portfolio Links

- [LinkedIn](https://www.linkedin.com/in/adamvaldezio)
- [Context Engine](https://github.com/ScatteredBuilds/context-engine)
- [Claude Tool Assistant](https://github.com/ScatteredBuilds/claude-tool-assistant)
- [Interp Notebooks](https://github.com/ScatteredBuilds/interp-notebooks)
