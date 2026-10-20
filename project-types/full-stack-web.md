# Project Guide: Full-Stack Web Application

Use this guide with the shared agent rules and project templates.

## Decide before coding
- User roles, permissions, and main journeys.
- Frontend framework and supported browsers/devices.
- Backend framework, API style, and validation.
- Database, schema, migrations, backup, and restore needs.
- Authentication, session handling, and account recovery.
- File storage, email, payments, or other integrations only when needed.
- Hosting, domain, TLS, CORS, logging, and budget.
- Tests and CI checks.

Do not add a database, authentication provider, or external service unless the requirements justify it.

## Architecture
Draw the browser, frontend, backend, database, and external providers. Mark where authentication and authorization are enforced.

## Implementation checks
- Keep business logic out of UI components where practical.
- Validate data at trust boundaries.
- Use migrations for schema changes.
- Include loading, empty, error, and success states.
- Test authorization, validation, and critical user journeys.
- Document tested local setup and deployment commands.
