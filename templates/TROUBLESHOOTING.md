# Troubleshooting Notes

Record verified problems and fixes so the same issue is easier to diagnose later. Never include secrets, tokens, private user data, or sensitive logs.

## Issue template

### [SHORT ERROR TITLE]
- **Symptom:** What did the user or terminal show?
- **Environment:** Runtime, OS, package versions, and relevant service.
- **Likely cause:** [CAUSE OR UNKNOWN]
- **Evidence:** Relevant error lines or command output, with sensitive data removed.
- **Minimal fix:** Exact file or setting changed and why.
- **Verification:** Command run and actual result.
- **Prevention:** Test or configuration change that could catch it earlier.

---

## Debugging rules
1. Read the full relevant error, not only the last line.
2. Inspect the failing code and nearby configuration before editing.
3. Reproduce or isolate the problem when practical.
4. Identify the root cause and make the smallest safe change.
5. Avoid unrelated refactors, formatting sweeps, or dependency upgrades.
6. Review the diff and run focused tests; expand checks when risk requires it.
7. If the fix is uncertain, state the uncertainty rather than pretending it is proven.
