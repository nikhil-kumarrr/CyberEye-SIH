# Security Policy

## 🛡️ Scope and Ethical Assessment Philosophy

**CyberEye / SecureLens (WMSA)** was engineered specifically for safe, authorized, and reproducible security evaluations (developed for **Smart India Hackathon 2026, Problem Statement 26163**).

The framework enforces fail-closed scope confinement:
- **Loopback isolation:** All dynamic scans, probes, and tests strictly target local loopback interfaces (`127.0.0.1` / container network).
- **Non-destructive PoCs:** Automated probes and verification procedures must never cause data destruction, denial of service, or irreversible state changes.
- **Human-in-the-loop verification:** Scanners and AI models flag candidates; human analysts verify actual impact.

---

## 🔒 Supported Versions

Only the latest release on the primary development branch is actively maintained with security updates.

| Version | Supported          |
| ------- | ------------------ |
| 0.1.x   | :white_check_mark: |
| < 0.1.0 | :x:                |

---

## 🚨 Reporting a Vulnerability

If you discover a security vulnerability within CyberEye / SecureLens itself:

1. **Do not create public GitHub issues or discussions** for unpatched vulnerabilities.
2. Please submit a report privately via **[GitHub Private Vulnerability Reporting](https://github.com/nikhil-kumarrr/CyberEye-SIH/security/advisories/new)** or email the maintainers directly at `nikhilkumar.20300@gmail.com`.
3. Include the following details to expedite triage:
   - Clear description of the vulnerability and its potential impact.
   - Exact steps or script to reproduce the issue in an isolated environment.
   - Proof of concept (PoC) adhering to responsible disclosure standards.
   - Any proposed mitigations or code patches.

---

## ⏱️ Response and Disclosure Timeline

- **Initial Response:** Within 48 hours to acknowledge receipt and begin triage.
- **Status Updates:** Every 3–5 business days until a resolution is tested and approved.
- **Coordinated Disclosure:** A fix will be published, followed by a public advisory crediting the reporter (if desired).
