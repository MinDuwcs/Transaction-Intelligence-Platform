# Agent Instructions

This repository uses production-grade engineering workflows.

## Primary rules

- Understand the task before changing code.
- Prefer simple, direct solutions.
- Make small, reviewable changes.
- Do not refactor unrelated code.
- Do not add dependencies without justification.
- Do not touch secrets or production configuration unless required.
- Verify every meaningful change.

## Workflow

For new features:

1. Write or clarify the spec.
2. Break the work into small tasks.
3. Implement one vertical slice at a time.
4. Add or update tests.
5. Run verification.
6. Review the diff before completion.

For bug fixes:

1. Reproduce the bug.
2. Identify the smallest failing case.
3. Fix the root cause.
4. Add a regression test if possible.
5. Verify the fix.

For code review:

- Check correctness.
- Check readability.
- Check security.
- Check tests.
- Check whether the change is smaller than it could be.