# Security Policy

## Reporting Vulnerabilities

AitherOS is currently in pre-alpha. If you discover a security vulnerability, please **do not** open a public issue.

Instead, email: **security@aitheros.ai**

We take security seriously and will respond within 48 hours.

## Current Security Measures

- All secrets managed via AitherSecrets (never in environment variables or code)
- Service-to-service authentication
- Pain system detects anomalous behavior
- Circuit breakers prevent cascade failures
- No default credentials shipped

## Scope

This policy applies to all AitherOS components:
- AitherOS microservices
- AitherZero automation framework
- AitherVeil dashboard
- Docker deployment configurations
- Genesis bootloader

---

*Full security documentation will ship with the alpha release.*
