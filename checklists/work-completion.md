# Work Completion Checklist

Use this after each meaningful task or phase. A checklist records evidence; it does not replace tests or review.

## Before work
- [ ] The task and expected behavior are clear.
- [ ] Relevant source files, instructions, and existing changes were inspected.
- [ ] Important open questions are resolved.
- [ ] Affected architecture, security, data, and UI decisions are understood.

## After implementation
- [ ] The change solves the requested problem.
- [ ] Only necessary files and lines were changed.
- [ ] Error cases and input validation were considered.
- [ ] Tests were added or updated where appropriate.
- [ ] Focused tests and relevant build/lint/type checks were run.
- [ ] The final diff was reviewed for unrelated edits and secrets.
- [ ] No check is marked as passed unless it actually passed.

## Documentation
- [ ] README updated if setup, usage, features, or commands changed.
- [ ] Architecture updated if components or data flow changed.
- [ ] Setup/deployment docs updated if configuration changed.
- [ ] Troubleshooting notes added for reusable, verified fixes.
- [ ] This checklist reflects the actual status.

## Handover
- **Changed:** [FILES AND PURPOSE]
- **Checks run:** [COMMANDS]
- **Results:** [PASSED / FAILED / NOT RUN]
- **Not verified:** [ITEMS]
- **Risks or follow-up:** [ITEMS]
