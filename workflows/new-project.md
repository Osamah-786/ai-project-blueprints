# Workflow: Start a New Project

Keep the process proportional to the project's size.

## 1. Understand the goal
Read the request and ask only questions needed to settle important unknowns. Identify users, problem, scope, constraints, and testable acceptance criteria.

## 2. Inspect the repository
Check existing files, package manager, runtime, instructions, Git status, and tests. Do not overwrite existing work or assume the repository is empty.

## 3. Decide setup
List required and optional tools, API providers, databases, authentication, environment variable names, local services, hosting, and CI/CD. Verify current provider capabilities, prices, quotas, and setup from official sources when relevant. Never store secrets in tracked docs.

## 4. Design architecture
Create a Mermaid diagram for the proposed components and data flow. Add an ER diagram when useful. Explain important choices and trade-offs briefly.

## 5. Prepare docs
Copy only useful templates: project brief, architecture, implementation plan, testing/deployment guides, and work checklist. Fill them with confirmed facts. Mark unknown choices as open rather than inventing details.

## 6. Establish a runnable baseline
Set up runtime, dependencies, formatting, tests, configuration, and a safe example environment file. Run an initial startup or build check and record its actual result.

## 7. Implement in phases
Make small, reviewable changes. After each phase, run appropriate checks, inspect the diff, and update relevant docs and checklist.

## 8. Prepare UI when needed
Clarify audience and primary actions. Define design tokens, layout, component rules, responsive behavior, and important interface states before complex UI implementation.

## 9. Prepare release
Use the pre-release checklist. Verify Docker, CI/CD, security checks, deployment configuration, health checks, and rollback where applicable.

## 10. Handover
Summarize changes, commands and actual results, manual setup still required, known risks, and unverified work.
