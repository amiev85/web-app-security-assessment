# Web Application Security Assessment

A structured security assessment of a web application conducted using the OWASP Testing Guide (WSTG) methodology.

## Scope & Methodology

| Phase | Coverage |
|-------|----------|
| Reconnaissance | Technology fingerprinting, directory enumeration, endpoint discovery |
| Authentication | Login mechanisms, session management, JWT handling |
| Authorisation | IDOR, privilege escalation, access control |
| Input Validation | SQLi, XSS, CSRF |
| Reporting | Executive summary + technical report with OWASP ASVS remediation |

## Key Findings Summary

| Severity | Count | Examples |
|----------|-------|---------|
| Critical | 3 | SQL Injection, Authentication Bypass |
| High | 7 | Stored XSS, IDOR, JWT misconfiguration |
| Medium | 12 | CSRF, Reflected XSS, Missing security headers |
| Low/Info | 8+ | Information disclosure, verbose errors |

> Full findings and PoC are not published to protect the application. A sanitised report is available on request.

## Tools Used

- **Burp Suite** — traffic interception, manual testing, scanner
- **Gobuster** — directory and endpoint enumeration
- **JWT Debugger / jwt.io** — token analysis and manipulation
- **CyberChef** — encoding/decoding, data analysis
- **Wappalyzer** — technology fingerprinting

## Deliverables

- `executive-report.pdf` — business-facing summary with risk ratings
- `technical-report.pdf` — full finding details with PoC steps and OWASP ASVS remediation

## Methodology Reference

- [OWASP Testing Guide (WSTG)](https://owasp.org/www-project-web-security-testing-guide/)
- [OWASP ASVS](https://owasp.org/www-project-application-security-verification-standard/)
- [CVSS v3.1 Scoring](https://www.first.org/cvss/)
