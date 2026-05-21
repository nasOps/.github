# Security Policy

## Supported versions

| Version | Supported |
|---|---|
| Latest release | Yes |
| Older releases | No |

## Reporting a vulnerability

If you discover a security vulnerability in any nasOps repository, please report it responsibly:

1. **Do not** open a public GitHub issue
2. Email **keamonk@stud.kea.dk** with a description of the vulnerability
3. Include steps to reproduce if possible
4. We will acknowledge receipt within 48 hours and aim to resolve critical issues within 7 days

## Security practices

- Passwords hashed with bcrypt
- Session cookies: `httponly`, `samesite=strict`, `secure` in production
- HTTPS enforced via Nginx with HSTS
- Automated scanning in CI: Trivy (container CVEs), Brakeman (static analysis), Bundler Audit (dependency CVEs), OWASP ZAP (baseline scan)
