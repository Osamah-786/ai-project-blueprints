# Project Guide: Agentic AI Systems

## Decide before coding
- Define allowed tasks and explicit boundaries.
- Choose the simplest suitable model and tools; verify current capabilities and costs.
- Decide whether a deterministic function or workflow is enough before introducing an agent.
- Define state, memory, tool contracts, retries, timeouts, and execution limits.
- Decide which actions require human approval.
- Plan tracing, evaluation, failure recovery, and fallback behavior.

## Architecture
Draw the orchestrator, agents or workflow steps, tools, external services, state store, and approval boundaries. Mark which components can make external changes.

## Safety and reliability
- Apply least privilege to every tool.
- Validate tool inputs and outputs.
- Require approval for destructive, costly, or externally visible actions when appropriate.
- Use idempotency and bounded retries for repeatable operations.
- Set budget, step, and time limits.
- Test failure paths and prompt-injection attempts.
- Do not treat a simulated tool call as proof that the live integration works.
