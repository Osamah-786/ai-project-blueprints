# Shared Coding Agent Rules

These are the shared engineering rules for projects that adopt this file. Follow the user's request and the target project's own instructions, while preserving safety and existing work.

## 1. Understand before changing
- Read relevant instructions and inspect the repository before coding.
- For a new project, clarify requirements, constraints, setup, and success criteria before major implementation.
- Ask focused questions when an unanswered decision materially changes cost, security, architecture, user experience, or scope.
- Do not ask questions already answered in the conversation or repository.
- For low-risk unknowns, choose a sensible default, state the assumption briefly, and continue.

## 2. Minimal, token-efficient code
- Solve the request with the smallest clear and maintainable implementation.
- Reuse suitable project patterns and existing dependencies.
- Avoid duplicate logic, needless abstraction, speculative features, excessive comments, and unnecessary files.
- Do not rewrite working code only because another style is possible.
- Inspect targeted files and summarize relevant findings. Avoid repeating whole files or long outputs when a short summary is enough.

## 3. Keep changes in scope
- For bug fixes, find the root cause and edit only the smallest safe area.
- Do not do unrelated refactoring, redesign, formatting sweeps, dependency upgrades, or renames.
- Preserve user changes and uncommitted work. Never reset, overwrite, or discard them without explicit permission.
- Explain significant or risky changes before making them.
- Inspect the final diff for unrelated edits.

## 4. Plan setup before major implementation
Identify what is actually needed: runtime and versions, package manager, APIs and providers, database, authentication, environment variables, external tools, hosting, Docker, CI/CD, and expected costs.

For each external service, record its purpose, whether it is required, setup steps, relevant costs/quotas, and a fallback when useful. Verify changing information from official sources. Do not invent capabilities, prices, or free tiers. Clearly separate required setup from optional setup.

## 5. Architecture and diagrams
Before substantial implementation, explain how components fit together. Use a Mermaid flowchart for system flow and an ER diagram when relationships between entities matter. Keep diagrams consistent with the actual proposed or implemented system and label planned parts honestly.

## 6. Security and privacy
- Keep real secrets, tokens, passwords, private keys, and sensitive user data out of source control, documentation, examples, and logs.
- Use environment variables or a proper secret manager and a safe `.env.example`.
- Validate untrusted input and enforce authentication and authorization on the server.
- Use least privilege, safe defaults, timeouts, and bounded retries.
- Avoid exposing stack traces or sensitive content to users.
- Report what security checks did and did not cover. Never promise perfect security.

## 7. Testing and verification
- Read existing test instructions before choosing commands.
- Add or update focused tests for new behavior and bug fixes when practical.
- Run the smallest useful check first, then broader tests/build/lint/type checks based on risk and availability.
- Verify Docker, CI/CD, health checks, and deployed integrations when the task calls for them and access is available.
- Never claim a command, integration, scan, or deployment passed unless it was actually run and passed.
- If a check cannot run, state why and list what remains unverified.

## 8. UI and UX
Before designing a significant UI, understand the audience, purpose, primary actions, content, devices, references, and constraints. Ask only about missing decisions that matter.

Define a small design system before building multiple screens: named color tokens, typography, spacing, layout, component behavior, and responsive rules. Choose colors intentionally for the product and audience. Avoid random gradients, excessive glass effects, generic AI-looking themes, repetitive cards, and decoration that does not improve usability.

Plan loading, empty, error, success, focus, keyboard, accessibility, and responsive states. Use realistic content when possible.

## 9. Documentation and checklist
After meaningful work:
- Update the README or relevant architecture, setup, testing, or deployment document when the change affects it.
- Update the project's work-completion checklist.
- Confirm docs match the actual code and commands.
- Inspect changed files and the final diff.
- Report changes, checks run, actual results, and outstanding issues in simple English.

Do not rewrite documentation that has not become necessary. Keep it concise and useful.

## 10. Final response
Report what changed, why it solves the request, commands run and their real results, and what remains unverified. Be honest about failures. Prefer a short summary over a large code dump.
