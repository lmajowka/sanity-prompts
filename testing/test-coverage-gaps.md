# Test Coverage Gaps

Review this repository's test suite for meaningful gaps. Map the critical code paths — core business logic, data mutations, authentication and permissions, payment or billing flows, integrations, and error handling — and compare them with what the existing tests actually exercise.

Look for untested critical paths, missing edge cases and failure modes, tests that assert too little to catch regressions, over-mocking that hides real behavior, flaky or order-dependent tests, and tests that no longer match the code they claim to cover. Run the suite and coverage tooling where available, but do not treat coverage percentage as the goal.

For each gap:
- Cite the untested files, functions, and branches, and the tests closest to them.
- Explain the realistic regression or bug that could slip through.
- Rate priority by business risk and likelihood of change.

Then write a separate, self-contained implementation prompt for each recommended group of tests. Each prompt should describe the behavior to cover, the cases to include, where the tests belong, which existing fixtures and conventions to follow, and how to confirm the tests fail when the behavior breaks.

Do not modify the repository.
