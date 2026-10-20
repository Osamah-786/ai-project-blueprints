# Workflow: Audit an Existing Project

The goal is to understand the project and report useful findings without changing code unnecessarily.

## Steps
1. Read the README, agent instructions, dependency manifests, environment examples, and relevant configuration.
2. Inspect structure, Git status, tests, build scripts, Docker files, CI workflows, and deployment settings as relevant.
3. Map the actual architecture. Use a Mermaid diagram and mark uncertain areas.
4. Identify setup gaps, reliability/security risks, missing tests, outdated instructions, and delivery gaps.
5. Separate confirmed findings from guesses and include file paths or evidence.
6. Prioritize by impact and effort.
7. Recommend focused next steps.

## Rules
- Do not edit files unless asked to make changes.
- Do not print or copy secrets discovered in local files.
- Do not run destructive commands or migrations against shared environments.
- Do not claim an integration or deployment was tested if it was only inspected.
- Keep the report concise and in simple English.
