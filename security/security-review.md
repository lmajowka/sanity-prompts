# Security Review

Review this repository for security vulnerabilities. Examine authentication and authorization, input validation, injection risks (SQL, command, template, XSS), secrets handling, session and token management, file uploads, SSRF, CORS and CSP configuration, dependency advisories, and exposure of sensitive data in logs, errors, or responses.

For each finding:
- Cite the relevant files, symbols, and the full data flow from untrusted input to the vulnerable sink.
- Explain the attack scenario, required preconditions, and realistic impact.
- Rate severity based on exploitability and impact, not theoretical worst case.
- Recommend a concrete fix that preserves existing behavior for legitimate users, and describe how to verify it.

Trace each issue to confirm it is reachable; account for existing middleware, framework protections, validation layers, and deployment configuration before reporting it. Separate confirmed vulnerabilities from hardening recommendations. Do not include working exploit payloads beyond what is needed to demonstrate the issue.

Do not modify the repository. If no meaningful vulnerabilities are supported by the evidence, say so.
