# Workflow: Review Code

Review for correctness and risk, not personal style preferences.

## Check
- Does the change meet the request and acceptance criteria?
- Are edge cases, failures, and concurrency handled correctly?
- Are inputs validated and access controls enforced?
- Could secrets or sensitive data leak?
- Are tests meaningful and sufficient for the risk?
- Are dependency, Docker, CI/CD, and deployment changes reasonable?
- Does documentation match the implementation?

## Report
List findings from highest to lowest severity. Include file/line references when available, user impact, and the smallest sensible fix. Separate confirmed bugs from possible risks. Do not rewrite code unless asked to fix it.
