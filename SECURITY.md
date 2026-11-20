# Hacknation security

Report vulnerabilities privately through [GitHub Security Advisories](https://github.com/OjciecChrzestny/Hacknation/security/advisories/new). Describe the affected component and impact. Redact credentials and personal information from reports, logs, screenshots, and examples.

## Development

Keep tokens, SSH private keys, and real environment files outside Git. Use placeholder values in `.env.example`. Before pushing, review staged files with `git diff --cached`. If a credential is exposed, revoke or rotate it immediately, including when the commit has since been deleted.

Treat code from public pull requests as untrusted. Review it before running it on a development machine with credentials. Use isolated GitHub-hosted runners for public contributions. Keep write tokens, deployment secrets, and VPS access out of jobs that execute contributor-controlled code.
