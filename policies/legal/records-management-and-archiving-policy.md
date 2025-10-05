# Records Management and Archiving Policy

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
1. Electronic records are stored in SharePoint Online or the approved document management system with versioning and access controls.
2. Physical records are kept in locked cabinets within secure areas. Removal of physical records requires a checkout log.
3. All Confidential and Restricted records must be classified and handled in line with the [Data Classification and Handling Policy](../information-security/data-classification-and-handling-policy.md) and protected under the [Data Protection and Privacy Policy](../cyber-security/data-protection-and-privacy-policy.md).

### Archiving and Disposal
1. Records exceeding their retention period shall be securely destroyed via cross-cut shredding for paper or cryptographic wipe for electronic media.
2. Archival copies required for legal or contractual purposes are stored in encrypted, offsite storage with quarterly integrity checks.
3. Departments must review their records annually and confirm destruction or continued retention to the Director.

## Technical Controls

1. Access to archives is restricted using role-based permissions and multi-factor authentication.
2. Audit logs for record access and deletion are retained for a minimum of three years.
3. Backup systems are tested quarterly to ensure recoverability of archived records.

## Roles and Responsibilities

1. **Employees and Contractors:** Follow records management and archiving procedures and report issues or non-compliance.
2. **Management:** Provide resources and enforce this policy within their areas of responsibility.
3. **Security and Compliance Teams:** Monitor records management and archiving controls, provide guidance, and coordinate improvements.

## Accountable Roles and Decision Authority

1. **Director:** Owns and maintains this policy, coordinates updates, and ensures alignment with the Cyber Governance Policy and Document Control Policy.
2. **Director (Risk Owner):** Reviews and approves exceptions, risk acceptances, and material control changes, documenting rationale in line with the Risk Management Policy.
3. **Director (Service Owner):** Oversees day-to-day execution of this policy, vendor engagement, and customer communications when actions affect external parties.


## Compliance

Failure to adhere to this policy may result in disciplinary action, up to and including termination, and may expose the organization to legal or regulatory penalties.

## Review

This policy will be reviewed at least annually and updated as necessary to remain effective and compliant with relevant requirements.

## Revision History

| Version | Date       | Description                                                                 | Author |
| ------- | ---------- | --------------------------------------------------------------------------- | ------ |
| 1.0     | 2023-01-01 | Initial policy release                                                      | Wayne Evans (Director) |
| 1.1     | 2025-09-10 | Added retention schedule, storage requirements and archiving procedures | ChatGPT |
| 2.0     | 2025-09-10 | Implementation guidelines added | Policy Team |
| 2.1     | 2025-10-05 | Author attribution updated | Wayne Evans (Director) |

## Implementation Guidelines
1. The Director records policy-related approvals and evidence in the central document repository and retains them for audit purposes.
2. BitLocker-encrypted storage protects customer data on company systems, and Windows Defender telemetry is reviewed weekly.
3. Weekly vulnerability scans and monthly patch reviews are led by the Director, with remediation actions tracked to completion.
4. Microsoft 365 security settings rely on features provided within the standard licence; compensating controls are documented when advanced tooling is unavailable.
5. Exceptions require written approval from the Director, including compensating controls and a defined review date.

