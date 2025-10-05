# Cyber Ask Ltd Cyber Security Risk Treatment Plan 2025

## Overview

This plan details mitigation activities arising from the 2025 enterprise cyber security risk assessment. Actions align with the Risk Management Policy, ISO/IEC 27001 control objectives, NCSC Cyber Assessment Framework, and AI assurance guidance. Progress is reviewed monthly by the Director with evidence retained for a minimum of six years.

## Action Plan with Deadlines

| Risk ID | Action ID | Description | Deadline | Owner | Resources / Budget | Status | Success Criteria |
| --- | --- | --- | --- | --- | --- | --- | --- |
| R1 | R1-A1 | Issue annual security attestations and software bill of materials requirements to AI/ML suppliers before model updates. | 2025-05-31 (Q2) | Director | Supplier engagement time (2 days) | Planned | Signed attestations stored; SBOM received for each model release. |
| R1 | R1-A2 | Build automated sandbox to hash-validate and behaviour-test third-party AI models prior to production release. | 2025-07-31 (Q3) | Director | £1,200 for GPU cloud credits | Planned | Sandbox runbook approved; validation reports archived for each deployment. |
| R2 | R2-A1 | Subscribe to immutable backup storage and integrate with Microsoft 365 and Azure recovery workflows. | 2025-05-15 (Q2) | Director | £150/month subscription | In Progress | Immutable backups verified daily; quarterly restore evidence filed. |
| R2 | R2-A2 | Enable Microsoft Defender Attack Surface Reduction (ASR) rules and document ransomware-specific response playbook. | 2025-06-30 (Q2) | Director | 3 days engineering effort | Planned | ASR policies enforced; response playbook tested via tabletop exercise. |
| R3 | R3-A1 | Expand conditional access to enforce device compliance, geographic restrictions, and sign-in risk policies. | 2025-06-30 (Q2) | Director | Internal configuration effort | Planned | Conditional access policies published; sign-in risk alerts triaged weekly. |
| R3 | R3-A2 | Pilot phishing-resistant authentication (FIDO2 keys) for privileged accounts and automate session revocation script. | 2025-08-31 (Q3) | Director | £600 for security keys | Planned | FIDO2 enforced for admins; revocation script executed after simulated compromise. |
| R4 | R4-A1 | Deploy AI prompt security guardrails including input/output filtering and rate limiting. | 2025-08-31 (Q3) | Director | £900 for AI security tooling | Planned | Guardrail policies logged; blocked prompt attempts reviewed monthly. |
| R4 | R4-A2 | Conduct quarterly AI red-team exercises to validate defences and document remediation tasks. | 2025-09-30 (Q3) | Director | Internal effort (1 day/quarter) | Planned | Red-team reports filed; remediation tasks tracked to closure. |
| R5 | R5-A1 | Automate Microsoft 365 configuration baseline checks using scripts aligned to CIS benchmarks. | 2025-06-30 (Q2) | Director | 3 days scripting effort | Planned | Baseline scripts scheduled weekly; deviations logged to ticketing board. |
| R5 | R5-A2 | Integrate Infrastructure-as-Code validation into change workflow with documented remediation SLAs. | 2025-07-31 (Q3) | Director | Internal effort (2 days) | Planned | IaC validation checklist live; SLA breaches escalated within 24 hours. |
| R6 | R6-A1 | Subscribe to rapid threat intelligence feeds for Microsoft ecosystem zero-days and integrate alert routing. | 2025-07-31 (Q3) | Director | £900 annual subscription | Planned | Feed integrated with monitoring; zero-day alerts acknowledged within 4 hours. |
| R6 | R6-A2 | Expand attack surface reduction and application allow-listing coverage across managed endpoints. | 2025-08-31 (Q3) | Director | 2 days engineering effort | Planned | ASR/allow-listing baselines documented; exceptions approved via change control. |
| R7 | R7-A1 | Enforce DMARC with quarantine policy and implement finance mailbox rule monitoring. | 2025-05-31 (Q2) | Director | Internal effort (1 day) | Planned | DMARC aggregate reports reviewed weekly; unauthorised rule changes alerted. |
| R7 | R7-A2 | Roll out deepfake-aware social engineering training and voice callback procedures for payment changes. | 2025-07-31 (Q3) | Director | £500 awareness content | Planned | Training completion 100%; voice callbacks evidenced for each payment change. |
| R8 | R8-A1 | Launch third-party security assurance programme including questionnaires, attestations, and risk scoring. | 2025-09-30 (Q3) | Director | 2 days design effort | Planned | Assurance register maintained; high-risk suppliers tracked with corrective actions. |
| R8 | R8-A2 | Implement just-in-time privileged access for external administrators and revoke unused delegated permissions. | 2025-10-31 (Q4) | Director | Internal effort (2 days) | Planned | Delegated rights reduced; JIT approval logs retained for 12 months. |
| R9 | R9-A1 | Inventory cryptographic assets, classify algorithms, and identify systems requiring post-quantum migration. | 2025-12-31 (Q4) | Director | 3 days assessment effort | Planned | Crypto inventory baselined; migration roadmap approved. |
| R9 | R9-A2 | Implement quantum-resistant cryptography pilot for secure data exchange workflows. | 2026-03-31 (Q1) | Director | £2,500 pilot licensing | Planned | Pilot PQC solution operational; interoperability and performance test results captured. |
| R10 | R10-A1 | Update and test SaaS outage playbooks including offline work kits and alternate communications. | 2025-05-31 (Q2) | Director | Internal effort (1 day) | Planned | Playbook signed-off; outage simulation demonstrates <2 hour recovery for critical tasks. |
| R10 | R10-A2 | Implement ticketing workflow to track continuity tasks, metrics, and dependency health checks. | 2025-06-30 (Q2) | Director | Internal effort (1 day) | In Progress | Ticketing board active; continuity metrics reviewed monthly. |

## Communication and Reporting

- Monthly updates summarised in the security metrics pack shared with stakeholders.
- Deviations or delays reported within 24 hours as required by the Risk Management Policy.
- Evidence (screenshots, logs, contracts) stored within the central document repository with access restricted per least-privilege principles.

## Review Schedule

- Treatment progress formally reviewed at quarterly management meetings.
- Plan updated after completion of each action, discovery of new risks, or material change in threat landscape.
