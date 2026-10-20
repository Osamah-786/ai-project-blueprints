# Pre-Release Checklist

Only mark an item complete after checking the evidence. Remove items that do not apply and explain important exceptions.

## Code and tests
- [ ] Requirements and acceptance criteria are met.
- [ ] Relevant unit/integration tests passed.
- [ ] Linting, type checks, and production build passed where configured.
- [ ] Known failures and untested paths are documented.
- [ ] Final Git diff contains no unrelated changes.

## Security and reliability
- [ ] No secrets or sensitive data are committed.
- [ ] Authentication and authorization were checked.
- [ ] Input validation and error handling were checked.
- [ ] Dependencies and container images were scanned where applicable.
- [ ] Findings were reviewed and dispositioned.
- [ ] Logs do not expose secrets or sensitive data.
- [ ] Health checks, timeouts, and resource limits were reviewed.

## Deployment
- [ ] Required environment variables are set in the target environment.
- [ ] Migrations and backups are handled safely.
- [ ] Docker image builds and runs, if applicable.
- [ ] CI/CD checks and permissions were reviewed.
- [ ] Smoke tests pass in the target environment.
- [ ] Monitoring and rollback steps are known.

## Documentation and handover
- [ ] README setup and commands match reality.
- [ ] Architecture and deployment docs match reality.
- [ ] Work checklist is up to date.
- [ ] Release summary separates verified results from assumptions.
