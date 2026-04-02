<p align="center">
  <img src="https://img.shields.io/badge/Framework-DISA%20STIGs-003366?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbD0id2hpdGUiIGQ9Ik0xMiAyTDMgN3Y2YzAgNS41NSAzLjg0IDEwLjc0IDkgMTIgNS4xNi0xLjI2IDktNi40NSA5LTEyVjdMMTIgMnoiLz48L3N2Zz4=&logoColor=white" alt="DISA STIGs"/>
  <img src="https://img.shields.io/badge/Platform-Windows%20Server-0078D6?style=for-the-badge&logo=windows&logoColor=white" alt="Windows"/>
  <img src="https://img.shields.io/badge/Automation-PowerShell-5391FE?style=for-the-badge&logo=powershell&logoColor=white" alt="PowerShell"/>
</p>

# STIG Implementation and Remediation

> **Security Technical Implementation Guide (STIG) hardening** — applying DISA STIGs to Windows systems to meet Department of Defense security baselines and achieve compliance readiness.

## Objective

Implement and document DISA STIG configurations for Windows environments, transforming default system configurations into hardened, audit-ready baselines. This project demonstrates the ability to interpret STIG requirements, apply technical controls, and verify compliance.

## What Are STIGs?

Security Technical Implementation Guides (STIGs) are configuration standards developed by the Defense Information Systems Agency (DISA) for DoD information systems. They define how operating systems, applications, and network devices must be configured to minimize security risk.

## Scope

| Category | Details |
|----------|---------|
| **STIG Benchmark** | Windows Server 2019 / Windows 10 |
| **Tool** | DISA STIG Viewer, PowerShell |
| **Assessment Method** | Manual review + automated scripting |
| **Compliance Target** | CAT I (Critical), CAT II (High), CAT III (Medium) findings |

## Methodology

```
Download STIG Benchmark → Review Findings in STIG Viewer → Assess Current State → Apply Remediations → Document Evidence → Verify Compliance
```

1. **Benchmark Selection** — Download applicable STIG from DISA's public library
2. **Gap Assessment** — Use STIG Viewer to identify non-compliant settings (Open findings)
3. **Remediation Planning** — Prioritize by severity category (CAT I first)
4. **Implementation** — Apply registry changes, GPO settings, and security configurations
5. **Verification** — Re-assess to confirm findings are closed
6. **Documentation** — Record findings, remediation steps, and evidence for audit trail

## STIG Severity Categories

| Category | Severity | Description |
|----------|----------|-------------|
| **CAT I** | High | Vulnerabilities that could directly result in loss of confidentiality, availability, or integrity |
| **CAT II** | Medium | Vulnerabilities that could result in degraded security posture |
| **CAT III** | Low | Vulnerabilities that could slightly degrade security measures |

## Key Areas Addressed

- Account and password policies
- Audit and logging configurations
- User rights assignments
- Registry security settings
- Service and feature hardening
- Windows Firewall configuration
- Remote access restrictions

## Tools Used

| Tool | Purpose |
|------|---------|
| DISA STIG Viewer | Review and track STIG findings |
| PowerShell | Automate configuration changes |
| Group Policy Editor | Apply security policies |
| Windows Security Baselines | Reference configurations |
| Event Viewer | Verify audit logging compliance |
