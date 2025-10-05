# Data Classification and Handling Policy

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** Wayne Evans (Director)

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

This policy establishes requirements for data classification and handling to protect organizational assets and ensure compliance with applicable laws and regulations.

## Scope

This policy applies to all employees, contractors, and third parties who access or manage company resources related to data classification and handling.

## Policy

### Classification Levels

| Level | Description | Typical Examples | Storage Requirements | Transmission Requirements | Access Controls | Retention & Disposal |
| --- | --- | --- | --- | --- | --- | --- |
| **Public** | Information authorised for disclosure outside the organisation with no adverse impact. | Published marketing content, public case studies, job adverts. | Store on approved collaboration platforms without additional encryption. | No restriction; ensure integrity when publishing. | None beyond standard publishing approvals. | Retain as long as commercially relevant; dispose when obsolete. |
| **Internal** | Operational information not intended for public release; low impact if disclosed. | Internal procedures, project plans, supplier contact lists. | Store on company-managed services (e.g., SharePoint, Teams) with default encryption. | Use company email or Teams; prohibit forwarding to personal accounts. | Limit to employees/contractors with business need; review access quarterly. | Follow Records Management Policy; shred/recycle paper copies securely. |
| **Confidential** | Sensitive business or personal data requiring enhanced protection. | Contract terms, financial reports, employee HR records. | Encrypt at rest (BitLocker, SharePoint encryption); maintain audit trails. | Use TLS 1.2+ channels; apply rights management where available. | Enforce least privilege, MFA, and conditional access; review monthly. | Retain per legal/regulatory schedule; securely erase media using approved tools. |
| **Restricted** | Mission-critical or highly sensitive data whose compromise causes severe harm or regulatory breach. | Client PII, security credentials, incident evidence, privileged legal files. | Store only in approved repositories with encryption, DLP, and logging; no local storage unless explicitly authorised. | Use encrypted channels (TLS 1.2+, SFTP); prohibit removable media unless encrypted and logged. | Limit to named individuals; require explicit approval and monitoring; enable continuous logging and alerting. | Retain only for mandated periods; perform certified destruction (crypto-shredding, secure wipe) and record evidence. |

### Handling Procedures
1. All documents and data repositories must display their classification in the header, footer or metadata.
2. Uploading Confidential or Restricted data to personal or unsanctioned cloud services is prohibited.
3. Transmission of Restricted data requires TLS 1.2 or higher. Removable media containing Restricted data must be encrypted and registered with IT.
4. Retention and disposal shall follow the [Records Management and Archiving Policy](../legal/records-management-and-archiving-policy.md).
5. Data owners are responsible for reviewing classifications annually or whenever the sensitivity of data changes.

### Training and Awareness
1. Staff receive onboarding training that includes examples of classified data and handling requirements.
2. Technical teams must implement data loss prevention controls to prevent exfiltration of Restricted data.

## Technical Controls

1. Data loss prevention tools enforce classification tags and block unauthorised transfers.
2. Encryption must follow the [Encryption Policy](encryption-policy.md) and use AES-256 for data at rest and TLS 1.2+ in transit.
3. Access controls and audit logging must be enabled on systems storing Confidential or Restricted data.

## Roles and Responsibilities

1. **Employees and Contractors:** Follow data classification and handling procedures and report issues or non-compliance.
2. **Management:** Provide resources and enforce this policy within their areas of responsibility.
3. **Security and Compliance Teams:** Monitor data classification and handling controls, provide guidance, and coordinate improvements.

## Accountable Roles and Decision Authority

1. **Director:** Owns and maintains this policy, coordinates updates, and ensures alignment with the Cyber Governance Policy and Document Control Policy.
2. **Director (Risk Owner):** Reviews and approves exceptions, risk acceptances, and material control changes, documenting rationale in line with the Risk Management Policy.
3. **Director (Service Owner):** Oversees day-to-day execution of this policy, vendor engagement, and customer communications when actions affect external parties.


## Compliance

Failure to adhere to this policy may result in disciplinary action, up to and including termination, and may expose the organization to legal or regulatory penalties.

## Review

This policy will be reviewed at least annually and updated as necessary to remain effective and compliant with relevant requirements.

## Revision History

| Version | Date       | Description                                                                | Author |
| ------- | ---------- | -------------------------------------------------------------------------- | ------ |
| 1.0     | 2023-01-01 | Initial policy release                                                     | Wayne Evans (Director) |
| 1.1     | 2025-09-10 | Added classification levels, handling procedures and technical controls | ChatGPT |
| 2.0     | 2025-09-10 | Implementation guidelines added | Policy Team |
| 2.1     | 2025-10-05 | Author attribution updated | Wayne Evans (Director) |

## Implementation Guidelines
1. The Director records policy-related approvals and evidence in the central document repository and retains them for audit purposes.
2. BitLocker-encrypted storage protects customer data on company systems, and Windows Defender telemetry is reviewed weekly.
3. Weekly vulnerability scans and monthly patch reviews are led by the Director, with remediation actions tracked to completion.
4. Microsoft 365 security settings rely on features provided within the standard licence; compensating controls are documented when advanced tooling is unavailable.
5. Exceptions require written approval from the Director, including compensating controls and a defined review date.

