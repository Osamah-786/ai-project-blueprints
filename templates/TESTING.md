# Testing Guide

## Setup
- Runtime and version: [VERSION]
- Package manager: [TOOL]
- Test dependencies: [DEPENDENCIES]
- Required test environment variable names: [NAMES ONLY]

## Test commands

| Check | What it checks | Command | Status |
|---|---|---|---|
| Unit tests | A function or component in isolation | [COMMAND] | [STATUS] |
| Integration tests | Components working together | [COMMAND] | [STATUS] |
| End-to-end tests | Main user journey | [COMMAND] | [STATUS] |
| Lint/type checks | Common code and type errors | [COMMAND] | [STATUS] |
| Production build | App can produce deployable output | [COMMAND] | [STATUS] |

Remove checks that do not apply and fill in real commands.

## Testing rules
- Cover new behavior and important failure cases.
- Add a regression test for a bug when practical.
- Do not present mocked integration tests as proof that a live service works.
- Never use production secrets or destructive production data for tests.
- Keep tests repeatable and isolated where possible.
- Report exact commands and real results. If a check was not run, say so.

## Test record

| Date | Command | Result | Notes |
|---|---|---|---|
| [DATE] | [COMMAND] | Passed / Failed / Not run | [DETAILS] |
