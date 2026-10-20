<<<<<<< HEAD
# AI Project Blueprints

Reusable documentation templates and coding-agent rules for building software with clear plans, minimal code, and verifiable results.

## What this toolkit helps with

- Define project requirements and decide setup before major implementation.
- Plan APIs, databases, AI providers, environment variables, hosting, and expected costs.
- Draw architecture diagrams with Mermaid.
- Keep code changes small and focused.
- Diagnose terminal errors with minimal, targeted fixes.
- Plan thoughtful, premium UI/UX rather than generic designs.
- Prepare testing, Docker, CI/CD, security checks, and deployment.
- Keep documentation and completion checklists aligned with the real code.

## Repository map

- `templates/`: project and technical documentation.
- `agent-configs/`: shared and tool-specific coding-agent instructions.
- `project-types/`: guidance for common software project types.
- `workflows/`: repeatable ways to start work, audit a repository, fix bugs, and review code.
- `checklists/`: checks before coding, after tasks, and before release.
- `examples/`: short examples of project documentation and agent instructions.

## Start a new project

1. Read `workflows/new-project.md`.
2. Inspect the target repository before copying any templates.
3. Copy only the files that fit the project's needs.
4. Copy or adapt `agent-configs/AGENTS.md` into the target project's root as `AGENTS.md` when your coding agent supports it.
5. Adapt the other agent files to the configuration format currently supported by that tool. Files in this repository are templates; they are not automatically loaded just because they exist here.
6. Resolve important setup, cost, security, and architecture decisions before major implementation.
7. Work in small phases, run relevant checks, inspect the Git diff, and update relevant documents and checklists.

For an existing terminal error, start with `workflows/bug-fixing.md`.

## Core principles

- Use simple, natural English.
- Prefer the smallest maintainable solution and avoid unrelated edits.
- Ask focused questions when an important decision is unclear.
- Use Mermaid diagrams when they improve understanding.
- Never commit real secrets or claim a check passed unless it actually passed.
- Treat security scans as useful evidence, not a guarantee of safety.
- Keep documentation consistent with the actual implementation.

See [CONTRIBUTING.md](CONTRIBUTING.md) before changing templates.
=======

>>>>>>> 9d6fd3961ede143c4363937d78c85dc19a99993e
