# Security Policy

## Supported Versions

| Version | Supported |
| ------- | --------- |
| 1.x.x   | ✅ Yes     |
| < 1.0   | ❌ No      |

## Reporting a Vulnerability

**Please do not open public issues for security vulnerabilities.**

Report vulnerabilities privately via GitHub Security Advisories:

👉 [Report a vulnerability](https://github.com/effectorHQ/.github/security/advisories/new)

Or email: **jydu_seven@outlook.com** *(monitored, response within 72 hours)*

### What to include

- Package name and version affected
- Description of the vulnerability
- Steps to reproduce
- Potential impact
- Any suggested fix (optional)

### What to expect

1. **Acknowledgement** within 72 hours
2. **Assessment** within 7 days — we'll confirm scope and severity
3. **Fix and disclosure** — we coordinate a release and CVE if applicable, then publish a security advisory

We follow [Responsible Disclosure](https://en.wikipedia.org/wiki/Responsible_disclosure) and will credit researchers who report valid vulnerabilities (unless you prefer to remain anonymous).

## Scope

All packages under the `@effectorhq` npm scope and repositories in the [effectorHQ GitHub organization](https://github.com/effectorHQ) are in scope.

Note: effectorHQ packages are **static analysis tools** — they parse and validate files but do not execute agent tools or make network requests at runtime. The primary threat surface is path traversal and malicious input in parsed files.
