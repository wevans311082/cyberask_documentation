# Encryption Policy

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** WEvans Director

This policy defines the requirements for encrypting sensitive information to protect confidentiality and integrity in line with CE/CE+ and ISO 27001 controls.

## Purpose

Ensure appropriate cryptographic safeguards are applied to data at rest and in transit.

## Scope

All systems, applications, and devices that store or transmit company data.

## Policy
- **Standards:** Use industry-accepted algorithms such as AES-256 for data at rest and TLS 1.2 or higher for data in transit.
- **Key Management:** Encryption keys must be stored securely, rotated annually, and access limited to authorized personnel.
- **Mobile Devices:** Portable media and laptops must employ full-disk encryption.
- **Cloud Services:** Enable encryption features provided by cloud vendors and manage keys under company control.
- **Exception Handling:** Any deviations require documented approval and compensating controls.

- All aspects of Encryption Policy must align with ISO/IEC 27001:2022 controls and the NCSC Cyber Assessment Framework.
- Procedures shall be documented, communicated, and reviewed at least annually by the Information Security Manager.
- Staff and contractors must receive training on Encryption Policy before being granted related responsibilities.
- Access and activities associated with Encryption Policy shall be logged and monitored to detect and respond to unauthorised actions.
- Deviations from this policy must be reported within 24 hours and remedied within 30 days.
- Technology configurations supporting Encryption Policy must follow relevant CIS Benchmarks and vendor hardening guides.
- Third parties engaged in Encryption Policy processes shall have contractual obligations to meet equivalent security standards.
- Records demonstrating compliance with this policy shall be retained for audit for a minimum of six years.
- The Information Security Manager must approve exceptions in writing, including scope, duration, and compensating controls.
- Failure to comply with this policy may result in disciplinary action, removal of access, or termination of contract.

- Systems processing Encryption Policy shall enforce least privilege and role-based access controls.
- Changes affecting Encryption Policy configurations must follow the Change Management Policy and receive formal approval.
- Monitoring tools shall generate alerts for Encryption Policy violations and designated staff must review these alerts daily.
- Internal audits shall verify adherence to Encryption Policy at least annually and report findings to senior management.
- Data associated with Encryption Policy must be protected in accordance with GDPR and UK statutory requirements.
- Users shall acknowledge and accept this policy annually to retain relevant access rights.

## Roles and Responsibilities

- **IT Security:** Defines approved cryptographic standards and manages key infrastructure.
- **System Owners:** Implement encryption according to this policy.
- **Users:** Protect passwords and report potential compromises.

## Review

This policy is reviewed annually or when new cryptographic standards emerge.

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
