# Project Agent Instructions

Use Addy Osmani Agent Skills from `.gemini/skills` when working in this repository.

## Default workflow

- Use `spec-driven-development` for new features.
- Use `planning-and-task-breakdown` before multi-file changes.
- Use `incremental-implementation` when building features.
- Use `test-driven-development` when changing behavior or fixing bugs.
- Use `debugging-and-error-recovery` when tests fail or runtime behavior is wrong.
- Use `code-review-and-quality` before finalizing changes.
- Use `security-and-hardening` when touching authentication, user input, APIs, database access, secrets, or deployment configuration.

## Rules

- Do not code before understanding the task.
- Do not refactor unrelated code.
- Do not add dependencies without justification.
- Do not modify secrets or production configuration unless explicitly required.
- Always verify meaningful changes with tests, type checks, linters, or manual runtime checks.
- Summarize what changed and what was verified.
