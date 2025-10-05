# Cyber Ask Ltd Technical Controls Implementation Roadmap

## Purpose

This roadmap enumerates technical controls selected to mitigate identified cyber security risks while adhering to Cyber Ask Ltd policies and regulatory expectations. Controls are mapped to key policies and standards (ISO/IEC 27001, NCSC CAF) and prioritised for implementation over the next two quarters.

## Control Catalogue

| Priority | Control | Description | Policy Alignment | Dependencies | Implementation Steps | Evidence Required |
| --- | --- | --- | --- | --- | --- | --- |
| P1 | Conditional Access Hardening | Enforce device compliance, geolocation restrictions, and MFA number matching for all sign-ins | MFA Policy; Microsoft 365 Security Policy; Risk Management Policy | Updated asset inventory; documented baseline | 1) Document conditions; 2) Pilot with admin account; 3) Roll out tenant-wide; 4) Monitor sign-in logs | Screenshots of policies; export of sign-in risk report |
| P1 | Immutable Backup Integration | Configure immutable cloud backup storage for domain controller and critical data repositories | Backup and Data Retention Policy; Business Continuity Policy | Supplier contract; network bandwidth assessment | 1) Select provider; 2) Integrate with current schedule; 3) Test restores; 4) Document runbook | Backup configuration report; restore test results |
| P1 | Attack Surface Reduction Rules | Enable Microsoft Defender ASR rules and Windows Defender Application Control on server and endpoint | Endpoint Security and Malware Protection Policy; Network Security Policy | Updated application inventory; change approval | 1) Evaluate impact in audit mode; 2) Approve via change control; 3) Enforce; 4) Monitor alerts weekly | GPO/Intune policy export; alert review logs |
| P2 | Automated Backup Verification | Script daily backup verification and alerting integrated with monitoring dashboard | Logging and Monitoring Policy; Security Metrics and Reporting Policy | Ticketing workflow; email distribution list | 1) Develop script; 2) Configure scheduled task; 3) Route alerts to Director; 4) Store reports | Script repository; alert notifications; monthly summary |
| P2 | Supplier Security Questionnaire | Deploy digital form capturing supplier controls, certifications, and attestations | Third-Party Access Control Policy; Outsourcing and MSP Policy | Supplier contact list; NDA updates | 1) Draft questionnaire; 2) Issue to suppliers; 3) Track responses; 4) Log corrective actions | Completed questionnaires; review notes |
| P2 | Configuration Baseline Automation | Implement configuration-as-code baselines and monthly compliance scans aligned to CIS benchmarks | Cloud Security Policy; Network Security Policy; Risk Management Policy | Secure repository; PowerShell modules | 1) Document baseline; 2) Develop scripts; 3) Schedule scans; 4) Review deviations monthly | Baseline documents; scan reports; remediation tickets |
| P3 | Secure Collaboration Enhancements | Apply sensitivity labels and secure sharing processes for subcontractor engagement | Data Protection and Privacy Policy; Cloud Security Policy | Licence assessment; user guidance materials | 1) Define labels; 2) Publish label policy; 3) Train users; 4) Monitor sharing events | Sensitivity label policy export; training acknowledgement |
| P3 | Ticketing and Metrics Workflow | Implement Microsoft Lists or equivalent for change, incident, and risk action tracking with integrated dashboards | Change Management Policy; Security Metrics and Reporting Policy | Microsoft 365 configuration; reporting templates | 1) Build list structure; 2) Define forms; 3) Automate reminders; 4) Generate dashboards | List export; dashboard screenshots; monthly metrics |

## Monitoring and Continuous Improvement

- Review control effectiveness monthly and log results in the security metrics report.
- Integrate alerts with the monitoring stack to meet daily review requirements.
- Capture lessons learned during change reviews to refine baselines and automation scripts.

## Governance

- Director approves control changes per the Change Management Policy and documents exceptions with compensating controls.
- Internal audit validates control operation annually, providing evidence for ISO/IEC 27001 alignment and client assurance.

