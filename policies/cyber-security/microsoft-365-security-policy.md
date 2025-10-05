# Microsoft 365 Security Policy

## Cyber Ask Operating Context

1. Cyber Ask Ltd operates with a single employee who also serves as the sole director responsible for governance, risk, and compliance decisions.
2. Cyber Ask Ltd maintains professional liability insurance covering its consulting and advisory services.
3. A dedicated virtual machine functions as the single Windows Server domain controller and is synchronized with Microsoft Entra ID for identity management.
4. The organisation holds a standard Microsoft 365 licence; Microsoft Purview and Microsoft Defender add-ons are not deployed, and Windows Defender provides endpoint protection.
5. Customer data is stored on BitLocker-encrypted drives to protect information at rest.
6. Cyber Ask Ltd assets are vulnerability-assessed weekly and patched promptly according to remediation guidance.
7. Cyber Ask Ltd has not yet achieved Cyber Essentials, Cyber Essentials Plus, or ISO 27001 certification but aligns its controls with those standards where practicable.
8. The Director personally fulfils HR, IT administration, and compliance duties, engaging specialist suppliers when additional expertise is required.



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

1. All aspects of Microsoft 365 Security Policy must align with ISO/IEC 27001:2022 controls and the NCSC Cyber Assessment Framework.
2. Procedures shall be documented, communicated, and reviewed at least annually by the Director.
3. Staff and contractors must receive training on Microsoft 365 Security Policy before being granted related responsibilities.
4. Access and activities associated with Microsoft 365 Security Policy shall be logged and monitored to detect and respond to unauthorised actions.
5. Deviations from this policy must be reported within 24 hours and remedied within 30 days.
6. Technology configurations supporting Microsoft 365 Security Policy must follow relevant CIS Benchmarks and vendor hardening guides.
7. Third parties engaged in Microsoft 365 Security Policy processes shall have contractual obligations to meet equivalent security standards.
8. Records demonstrating compliance with this policy shall be retained for audit for a minimum of six years.
9. The Director must approve exceptions in writing, including scope, duration, and compensating controls.
10. Failure to comply with this policy may result in disciplinary action, removal of access, or termination of contract.

1. Systems processing Microsoft 365 Security Policy shall enforce least privilege and role-based access controls.
2. Changes affecting Microsoft 365 Security Policy configurations must follow the Change Management Policy and receive formal approval.
3. Monitoring tools shall generate alerts for Microsoft 365 Security Policy violations and designated staff must review these alerts daily.
4. Internal audits shall verify adherence to Microsoft 365 Security Policy at least annually and report findings to senior management.
5. Data associated with Microsoft 365 Security Policy must be protected in accordance with GDPR and UK statutory requirements.
6. Users shall acknowledge and accept this policy annually to retain relevant access rights.

## Technical Controls

1. Enable Microsoft Entra ID Conditional Access to require MFA and block legacy authentication.
2. Use Intune to manage and enforce device compliance for endpoints accessing M365.
3. Configure Microsoft Purview DLP, retention, and sensitivity labels to protect and govern data.
4. Integrate Microsoft Defender for Office 365 and Defender for Endpoint for threat protection and automatic response.
5. Forward M365 audit logs and alerts to the centralized logging platform.

## Roles and Responsibilities

1. **Employees and Contractors:** Use Microsoft 365 services in accordance with this policy and report security issues.
2. **Management:** Provide resources to implement and maintain required Microsoft 365 controls.
3. **Security and Compliance Teams:** Configure, monitor, and improve Microsoft 365 security settings and respond to incidents.

## Accountable Roles and Decision Authority

1. **Director:** Owns and maintains this policy, coordinates updates, and ensures alignment with the Cyber Governance Policy and Document Control Policy.
2. **Director (Risk Owner):** Reviews and approves exceptions, risk acceptances, and material control changes, documenting rationale in line with the Risk Management Policy.
3. **Director (Service Owner):** Oversees day-to-day execution of this policy, vendor engagement, and customer communications when actions affect external parties.


## Compliance

Failure to comply with this policy may result in disciplinary action and could expose the organization to legal or regulatory penalties.

## Review

This policy will be reviewed at least annually or upon significant changes to Microsoft 365 services or organizational requirements.

## Implementation Guidelines
1. The Director records policy-related approvals and evidence in the central document repository and retains them for audit purposes.
2. BitLocker-encrypted storage protects customer data on company systems, and Windows Defender telemetry is reviewed weekly.
3. Weekly vulnerability scans and monthly patch reviews are led by the Director, with remediation actions tracked to completion.
4. Microsoft 365 security settings rely on features provided within the standard licence; compensating controls are documented when advanced tooling is unavailable.
5. Exceptions require written approval from the Director, including compensating controls and a defined review date.


## Revision History

| Version | Date | Description | Author |
| ------- | ---------- | ----------------------- | ------ |
| 2.0     | 2025-09-10 | Implementation guidelines added | Policy Team |
| 2.1     | 2025-10-05 | Author attribution updated | Wayne Evans (Director) |
