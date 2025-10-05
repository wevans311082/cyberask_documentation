# Cyber Ask Ltd Cyber Security Risk Treatment Plan 2025

## Overview

This plan details mitigation activities arising from the 2025 enterprise cyber security risk assessment. Actions align with the Risk Management Policy, ISO/IEC 27001 control objectives, and applicable cyber security and information security policies. Progress is reviewed monthly by the Director with evidence retained for a minimum of six years.

## Treatment Summary

| Risk ID | Action ID | Description | Policy Alignment | Resources / Budget | Owner | Target Completion | Success Criteria | Status |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| R1 | R1-A1 | Design and implement conditional access policies enforcing compliant devices, location restrictions, and MFA number matching | Multi-Factor Authentication Policy; Microsoft 365 Security Policy; Risk Management Policy | 2 days configuration time; no additional licence cost | Director | 2025-03-15 | Policies deployed and tested; audit logs evidencing enforcement | Planned |
| R1 | R1-A2 | Procure phishing detection capability (Defender for Office P1 or equivalent) and schedule quarterly phishing simulations | Monitoring and Threat Intelligence Policy; Security Metrics and Reporting Policy | £1,200 annual subscription | Director | 2025-06-30 | Solution live with alert triage runbook; phishing simulation reports stored | Planned |
| R2 | R2-A1 | Enable Microsoft Defender Attack Surface Reduction (ASR) rules and Windows Defender Application Control on domain controller and laptop | Endpoint Security and Malware Protection Policy; Network Security Policy | 3 days engineering effort | Director | 2025-04-15 | ASR policies deployed with documented exceptions; WDAC policy enforced | In Progress |
| R2 | R2-A2 | Subscribe to immutable cloud backup service for domain controller and key data repositories; integrate with backup schedule | Backup and Data Retention Policy; Business Continuity Policy | £150/month subscription | Director | 2025-05-31 | Immutable backups running with daily success alerts; quarterly restore test evidence | Planned |
| R3 | R3-A1 | Automate backup verification reporting and alerting into monitoring dashboard | Logging and Monitoring Policy; Backup and Data Retention Policy | 2 days scripting effort | Director | 2025-04-30 | Daily verification emails stored; alerts reviewed and logged | Planned |
| R3 | R3-A2 | Conduct quarterly restore tests with documented results and approvals | Change Management Policy; Risk Assessment Report requirements | Internal effort (0.5 day per quarter) | Director | 2025-06-30 (first cycle) | Restore evidence captured; lessons logged in CAPA register | Planned |
| R4 | R4-A1 | Implement supplier security due diligence questionnaire and annual attestation workflow | Third-Party Access Control Policy; Outsourcing and MSP Policy | 1 day to develop questionnaire; optional external review £500 | Director | 2025-07-31 | Questionnaire issued to all suppliers; responses stored and reviewed | Planned |
| R4 | R4-A2 | Deploy secure file transfer mechanism (encrypted workspace or M365 sensitivity labels) for subcontractor collaboration | Data Protection and Privacy Policy; Cloud Security Policy | Potential £600 annual licence | Director | 2025-07-31 | Secure sharing enabled; access logged; usage guidance issued | Planned |
| R5 | R5-A1 | Contract trusted partner for quarterly peer review of high-risk changes and incident response readiness | Change Management Policy; Incident Response Policy | £1,200 annually | Director | 2025-08-31 | Peer review reports filed; action items tracked | Planned |
| R5 | R5-A2 | Deploy lightweight ticketing workflow (e.g., Microsoft Lists) for change and risk action tracking | Risk Management Policy; Security Metrics and Reporting Policy | Internal effort (1 day) | Director | 2025-03-31 | Ticketing board live; all changes logged with approvals | In Progress |
| R6 | R6-A1 | Document configuration baselines and automate compliance checks using scripts aligned with CIS benchmarks | Cloud Security Policy; Network Security Policy; Risk Management Policy | 3 days development time | Director | 2025-06-30 | Baseline repository created; monthly compliance reports stored | Planned |
| R6 | R6-A2 | Monitor Microsoft Secure Score monthly and document remediation decisions | Security Metrics and Reporting Policy; Monitoring and Threat Intelligence Policy | Internal effort (0.5 day/month) | Director | 2025-03-31 (first review) | Monthly Secure Score reports with action logs | Planned |

## Communication and Reporting

- Monthly updates summarised in the security metrics pack shared with stakeholders.
- Deviations or delays reported within 24 hours as required by the Risk Management Policy.
- Evidence (screenshots, logs, contracts) stored within the central document repository with access restricted per least-privilege principles.

## Review Schedule

- Treatment progress formally reviewed at quarterly management meetings.
- Plan updated after completion of each action, discovery of new risks, or material change in threat landscape.

