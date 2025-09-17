# Records Management and Archiving Policy

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** WEvans Director

## Purpose

This policy establishes requirements for records management and archiving to protect organizational assets and ensure compliance with applicable laws and regulations.

## Scope

This policy applies to all employees, contractors, and third parties who access or manage company resources related to records management and archiving.

## Policy

### Record Retention
| Record Type                | Retention Period | Storage Location                |
|---------------------------|-----------------|---------------------------------|
| Financial records         | 7 years         | Secure accounting system and encrypted archive storage |
| HR personnel files        | 6 years after employment ends | HR management system with encrypted backups |
| Security logs             | 1 year unless required for investigations | Centralised logging platform |
| Customer contracts        | Contract term + 7 years | Document management system with version control |

### Storage and Protection
- Electronic records are stored in SharePoint Online or the approved document management system with versioning and access controls.
- Physical records are kept in locked cabinets within secure areas. Removal of physical records requires a checkout log.
- All Confidential and Restricted records must be classified and handled in line with the [Data Classification and Handling Policy](../information-security/data-classification-and-handling-policy.md) and protected under the [Data Protection and Privacy Policy](../cyber-security/data-protection-and-privacy-policy.md).

### Archiving and Disposal
- Records exceeding their retention period shall be securely destroyed via cross-cut shredding for paper or cryptographic wipe for electronic media.
- Archival copies required for legal or contractual purposes are stored in encrypted, offsite storage with quarterly integrity checks.
- Departments must review their records annually and confirm destruction or continued retention to the Information Security Manager.

## Technical Controls

- Access to archives is restricted using role-based permissions and multi-factor authentication.
- Audit logs for record access and deletion are retained for a minimum of three years.
- Backup systems are tested quarterly to ensure recoverability of archived records.

## Roles and Responsibilities

- **Employees and Contractors:** Follow records management and archiving procedures and report issues or non-compliance.
- **Management:** Provide resources and enforce this policy within their areas of responsibility.
- **Security and Compliance Teams:** Monitor records management and archiving controls, provide guidance, and coordinate improvements.

## Accountable Roles and Decision Authority

- **Policy Owner (General Counsel):** Maintains this policy, coordinates updates, and ensures alignment with the Document Control Policy and Cyber Governance Policy.
- **Chief Information Security Officer (CISO):** Validates security implications and approves exceptions affecting information assets per the Information Security Policy.
- **Risk and Compliance Committee:** Oversees regulatory risk treatment decisions consistent with the Risk Management Policy.
- **Executive Leadership Team:** Ratifies significant legal or contractual commitments in line with the Cyber Governance Policy.

Exception requests must follow the exception management process described in the Cyber Governance Policy and all approvals must be recorded in accordance with the Document Control Policy.

## Compliance

Failure to adhere to this policy may result in disciplinary action, up to and including termination, and may expose the organization to legal or regulatory penalties.

## Review

This policy will be reviewed at least annually and updated as necessary to remain effective and compliant with relevant requirements.

## Revision History

| Version | Date       | Description                                                                 | Author |
| ------- | ---------- | --------------------------------------------------------------------------- | ------ |
| 1.0     | 2023-01-01 | Initial policy release                                                      | WEvans Director |
| 1.1     | 2025-09-10 | Added retention schedule, storage requirements and archiving procedures | ChatGPT |
| 2.0     | 2025-09-10 | Implementation guidelines added | Policy Team |

## Implementation Guidelines
- All requests and approvals must be tracked in the ServiceDesk system.
- Data at rest must use AES-256 encryption; data in transit must use TLS 1.2+ with perfect forward secrecy.
- Security events shall log to the central SIEM and be retained for 12 months.
- Control owners perform quarterly self-assessments; Information Security conducts annual audits.
- Exceptions require written CISO approval and must include compensating controls.

