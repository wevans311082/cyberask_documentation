# Microsoft 365 Security Policy

## Purpose

This policy defines security and compliance requirements for the organization's Microsoft 365 (M365) environment to protect data, manage risk, and meet regulatory obligations.

## Scope

This policy applies to all Microsoft 365 services, accounts, and devices used to access corporate data.

## Policy
1. The organization shall configure the Microsoft 365 tenant in accordance with Microsoft's security baseline and review Secure Score at least quarterly.
2. Conditional Access policies shall enforce multi-factor authentication and device compliance for all M365 access.
3. Data loss prevention, retention, and sensitivity labels shall be implemented using Microsoft Purview.
4. Microsoft Defender for Office 365 and Microsoft Defender for Endpoint shall be enabled and integrated with central monitoring.
5. Audit logs from Microsoft 365 shall be collected and retained in accordance with the Logging and Monitoring Policy.

- All aspects of Microsoft 365 Security Policy must align with ISO/IEC 27001:2022 controls and the NCSC Cyber Assessment Framework.
- Procedures shall be documented, communicated, and reviewed at least annually by the Information Security Manager.
- Staff and contractors must receive training on Microsoft 365 Security Policy before being granted related responsibilities.
- Access and activities associated with Microsoft 365 Security Policy shall be logged and monitored to detect and respond to unauthorised actions.
- Deviations from this policy must be reported within 24 hours and remedied within 30 days.
- Technology configurations supporting Microsoft 365 Security Policy must follow relevant CIS Benchmarks and vendor hardening guides.
- Third parties engaged in Microsoft 365 Security Policy processes shall have contractual obligations to meet equivalent security standards.
- Records demonstrating compliance with this policy shall be retained for audit for a minimum of six years.
- The Information Security Manager must approve exceptions in writing, including scope, duration, and compensating controls.
- Failure to comply with this policy may result in disciplinary action, removal of access, or termination of contract.

- Systems processing Microsoft 365 Security Policy shall enforce least privilege and role-based access controls.
- Changes affecting Microsoft 365 Security Policy configurations must follow the Change Management Policy and receive formal approval.
- Monitoring tools shall generate alerts for Microsoft 365 Security Policy violations and designated staff must review these alerts daily.
- Internal audits shall verify adherence to Microsoft 365 Security Policy at least annually and report findings to senior management.
- Data associated with Microsoft 365 Security Policy must be protected in accordance with GDPR and UK statutory requirements.
- Users shall acknowledge and accept this policy annually to retain relevant access rights.

## Technical Controls

- Enable Microsoft Entra ID Conditional Access to require MFA and block legacy authentication.
- Use Intune to manage and enforce device compliance for endpoints accessing M365.
- Configure Microsoft Purview DLP, retention, and sensitivity labels to protect and govern data.
- Integrate Microsoft Defender for Office 365 and Defender for Endpoint for threat protection and automatic response.
- Forward M365 audit logs and alerts to the centralized logging platform.

## Roles and Responsibilities

- **Employees and Contractors:** Use Microsoft 365 services in accordance with this policy and report security issues.
- **Management:** Provide resources to implement and maintain required Microsoft 365 controls.
- **Security and Compliance Teams:** Configure, monitor, and improve Microsoft 365 security settings and respond to incidents.

## Compliance

Failure to comply with this policy may result in disciplinary action and could expose the organization to legal or regulatory penalties.

## Review

This policy will be reviewed at least annually or upon significant changes to Microsoft 365 services or organizational requirements.

## Implementation Guidelines
- All requests and approvals must be tracked in the ServiceDesk system.
- Data at rest must use AES-256 encryption; data in transit must use TLS 1.2+ with perfect forward secrecy.
- Security events shall log to the central SIEM and be retained for 12 months.
- Control owners perform quarterly self-assessments; Information Security conducts annual audits.
- Exceptions require written CISO approval and must include compensating controls.

## Revision History

| Version | Date | Description | Author |
| ------- | ---------- | ----------------------- | ------ |
| 2.0     | 2025-09-10 | Implementation guidelines added | Policy Team |
