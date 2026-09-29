# Unnecessary Code Review

Review this repository for unnecessary code, including unused files, imports, dependencies, dead branches, redundant abstractions, and duplicated logic.

For each finding:
- Verify it against references, entry points, configuration, and tests. Account for dynamic usage and public APIs.
- Explain why it appears unnecessary, cite relevant file paths and symbols, and describe any removal risks.

Exclude speculative findings and avoid treating personal style preferences as unnecessary code.

Then write a separate, self-contained implementation prompt for each independent finding. Each prompt should describe the problem, the specific cleanup to perform, constraints to preserve existing behavior, and appropriate validation. Group related changes when they must be handled together, and flag dependencies or conflicts between prompts.

Order findings by confidence and expected value. Do not modify the repository.
