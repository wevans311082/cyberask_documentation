# Encryption Policy

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** Wayne Evans (Director)

This policy defines the requirements for encrypting sensitive information to protect confidentiality and integrity in line with CE/CE+ and ISO 27001 controls.

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

Ensure appropriate cryptographic safeguards are applied to data at rest and in transit.

## Scope

All systems, applications, and devices that store or transmit company data.

## Policy
1. **Standards:** Use industry-accepted algorithms such as AES-256 for data at rest and TLS 1.2 or higher for data in transit.
2. **Key Management:** Encryption keys must be stored securely, rotated annually, and access limited to authorized personnel.
3. **Mobile Devices:** Portable media and laptops must employ full-disk encryption.
4. **Cloud Services:** Enable encryption features provided by cloud vendors and manage keys under company control.
5. **Exception Handling:** Any deviations require documented approval and compensating controls.

1. All aspects of Encryption Policy must align with ISO/IEC 27001:2022 controls and the NCSC Cyber Assessment Framework.
2. Procedures shall be documented, communicated, and reviewed at least annually by the Director.
3. Staff and contractors must receive training on Encryption Policy before being granted related responsibilities.
4. Access and activities associated with Encryption Policy shall be logged and monitored to detect and respond to unauthorised actions.
5. Deviations from this policy must be reported within 24 hours and remedied within 30 days.
6. Technology configurations supporting Encryption Policy must follow relevant CIS Benchmarks and vendor hardening guides.
7. Third parties engaged in Encryption Policy processes shall have contractual obligations to meet equivalent security standards.
8. Records demonstrating compliance with this policy shall be retained for audit for a minimum of six years.
9. The Director must approve exceptions in writing, including scope, duration, and compensating controls.
10. Failure to comply with this policy may result in disciplinary action, removal of access, or termination of contract.

1. Systems processing Encryption Policy shall enforce least privilege and role-based access controls.
2. Changes affecting Encryption Policy configurations must follow the Change Management Policy and receive formal approval.
3. Monitoring tools shall generate alerts for Encryption Policy violations and designated staff must review these alerts daily.
4. Internal audits shall verify adherence to Encryption Policy at least annually and report findings to senior management.
5. Data associated with Encryption Policy must be protected in accordance with GDPR and UK statutory requirements.
6. Users shall acknowledge and accept this policy annually to retain relevant access rights.

## Roles and Responsibilities

1. **IT Security:** Defines approved cryptographic standards and manages key infrastructure.
2. **System Owners:** Implement encryption according to this policy.
3. **Users:** Protect passwords and report potential compromises.

## Accountable Roles and Decision Authority

1. **Director:** Owns and maintains this policy, coordinates updates, and ensures alignment with the Cyber Governance Policy and Document Control Policy.
2. **Director (Risk Owner):** Reviews and approves exceptions, risk acceptances, and material control changes, documenting rationale in line with the Risk Management Policy.
3. **Director (Service Owner):** Oversees day-to-day execution of this policy, vendor engagement, and customer communications when actions affect external parties.


## Review

This policy is reviewed annually or when new cryptographic standards emerge.

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
