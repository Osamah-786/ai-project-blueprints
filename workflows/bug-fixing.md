# Workflow: Fix a Bug with Minimal Changes

## 1. Understand the failure
Read the error, stack trace, command, and expected behavior. Ask for missing information only if it blocks diagnosis. Remind the user to redact secrets.

## 2. Inspect the relevant area
Open the failing file and nearby code/configuration. Check runtime and dependency versions when relevant. Review recent changes if available.

## 3. Find the cause
Separate the symptom from the root cause. Use a small reproduction or focused diagnostic command when practical.

## 4. Make the smallest safe fix
- Change only the relevant lines and directly necessary tests/configuration.
- Preserve unrelated changes.
- Do not reformat whole files, upgrade packages, or redesign components unless evidence shows it is required.
- Explain any unavoidable wider change.

## 5. Verify
Run the narrowest useful check, then broader tests/builds based on risk. Inspect the final diff.

## 6. Report
State the cause, files changed, why the fix should work, commands and actual results, and remaining uncertainty. If not verified, say so.

## 7. Document
Update the work checklist. Add a troubleshooting entry only for a reusable, verified fix. Update README or architecture only if setup, behavior, or design changed.
