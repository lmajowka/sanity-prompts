# Frontend Performance Review

Review this app for worthwhile frontend performance improvements. Measure key pages in the running app and inspect the source for bundle size, code splitting, render-blocking resources, image and font loading, unnecessary re-renders, expensive effects, long tasks, layout shifts, memory leaks, and over-fetching or waterfall requests.

For each finding:
- Cite the relevant files, components, and the page or interaction where it shows up.
- Provide the measurement that supports it (Core Web Vitals, bundle analysis, performance trace, or network waterfall), including device and network conditions.
- Recommend a concrete improvement, including tradeoffs and risks.
- Describe how to measure the impact and confirm nothing regressed visually or functionally.

Prioritize by user-facing impact, confidence, and implementation effort. Test on throttled mobile conditions, not just a fast desktop. Distinguish measured problems from opportunities that need real-user data, and avoid speculative micro-optimizations.

Do not modify the repository. If no meaningful optimizations are supported by the evidence, say so.
