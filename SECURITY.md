# Security Policy

## Reporting

Please do not open a public issue for suspected security problems.

Report vulnerabilities privately to the project maintainers with:

- a short description of the issue
- affected files or commands
- reproduction steps
- whether any credentials, sessions, or personal data may be exposed

## Sensitive Data Handling

The following should never be committed to the repository:

- `.env`
- `.playwright/` browser profiles
- raw `reports/*_debug_*` artifacts
- tokens, session ids, cookies, or account-specific URLs

If you need to share a debugging sample, sanitize it first.
