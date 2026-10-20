# Example: Task Instructions for a Coding Agent

## Goal
Add a health endpoint to the existing backend.

## Before editing
- Inspect the framework, route structure, and any existing health checks.
- Find the current test pattern.
- Do not change unrelated files.

## Expected behavior
- Return a simple success response when the service is ready.
- Do not expose secrets, stack traces, or internal configuration.
- If readiness depends on another service, define that behavior explicitly instead of silently adding dependencies.

## Implementation
- Reuse existing patterns and keep the change minimal.
- Add a focused test.
- Update the README only if the endpoint affects setup, operations, or user-facing documentation.

## Verification
Run the focused test and available checks. Report exact commands and actual results. Do not claim the endpoint was tested in production unless that happened.
