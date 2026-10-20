# Project Guide: DevOps and Delivery

## Decide before coding
- Identify runtime, dependency manager, build/start commands, and port.
- Define local and production environments and their configuration differences.
- Decide whether Docker is needed and what it should package.
- Select CI checks: formatting, linting, tests, build, dependency scan, and image scan as suitable.
- Define deployment triggers, permissions, secrets, health checks, logs, monitoring, and rollback.
- Estimate resource needs and costs.

## Docker
- Use trusted base images and pin versions where appropriate.
- Run as non-root when practical.
- Never bake secrets into image layers or build arguments.
- Keep build context small and exclude local secrets.
- Check signals, process behavior, health, ports, and file permissions.
- Build and run the image to verify it, not just the Dockerfile syntax.

## CI/CD and security
- Give pipelines only the permissions they need.
- Pin external actions and dependencies based on risk and maintenance needs.
- Fail required checks when tests or builds fail.
- Treat scan results as evidence, not a guarantee of safety.
- Triage findings and update vulnerable dependencies responsibly.
- Avoid automatic production deploys unless intended.
- Verify deployed health and document rollback.
