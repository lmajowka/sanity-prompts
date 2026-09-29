# Dependency Health Check

Review this repository's dependencies across all package manifests and lockfiles. Identify outdated packages, known security advisories, deprecated or unmaintained libraries, duplicated or overlapping packages that serve the same purpose, dependencies declared in the wrong group (runtime versus development), unpinned or overly loose version ranges, and license concerns.

For each finding:
- Cite the manifest, the package, current and target versions, and where it is used in the code.
- Explain the risk of leaving it as is and the risk of changing it, including breaking changes from changelogs or migration guides.
- Estimate the upgrade effort and note any packages that must be upgraded together.

Verify advisories against how the package is actually used before rating severity. Group findings into safe patch-level updates, updates that need code changes, and replacements.

Then write a separate, self-contained implementation prompt for each independent upgrade or group of coupled upgrades, including the steps, the code that must change, and how to validate with builds, tests, and manual checks.

Do not modify the repository.
