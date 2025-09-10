# Data Classification and Handling Policy

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** WEvans Director

## Purpose

This policy establishes requirements for data classification and handling to protect organizational assets and ensure compliance with applicable laws and regulations.

## Scope

This policy applies to all employees, contractors, and third parties who access or manage company resources related to data classification and handling.

## Policy

### Classification Levels
| Level      | Description                                                   | Examples                                                 | Minimum Handling Requirements |
|------------|---------------------------------------------------------------|----------------------------------------------------------|-------------------------------|
| **Public** | Approved for general release                                  | Marketing brochures, published blog articles             | May be shared without restriction |
| **Internal** | Business information not intended for external distribution | Internal project plans, routine internal emails          | Store on company-managed systems; share only with employees |
| **Confidential** | Sensitive business or personal data                     | Contract terms, internal financial reports               | Access limited to authorised staff; encrypt at rest using AES-256; transmit via company email/VPN |
| **Restricted** | Highly sensitive data whose compromise could cause severe damage | Customer personal data, financial records, credentials | Access logged and limited to named individuals; encryption using AES-256 at rest and TLS 1.2+ in transit; MFA required; storage only in approved repositories |

### Handling Procedures
- All documents and data repositories must display their classification in the header, footer or metadata.
- Uploading Confidential or Restricted data to personal or unsanctioned cloud services is prohibited.
- Transmission of Restricted data requires TLS 1.2 or higher. Removable media containing Restricted data must be encrypted and registered with IT.
- Retention and disposal shall follow the [Records Management and Archiving Policy](../legal/records-management-and-archiving-policy.md).
- Data owners are responsible for reviewing classifications annually or whenever the sensitivity of data changes.

### Training and Awareness
- Staff receive onboarding training that includes examples of classified data and handling requirements.
- Technical teams must implement data loss prevention controls to prevent exfiltration of Restricted data.

## Technical Controls

- Data loss prevention tools enforce classification tags and block unauthorised transfers.
- Encryption must follow the [Encryption Policy](encryption-policy.md) and use AES-256 for data at rest and TLS 1.2+ in transit.
- Access controls and audit logging must be enabled on systems storing Confidential or Restricted data.

## Roles and Responsibilities

- **Employees and Contractors:** Follow data classification and handling procedures and report issues or non-compliance.
- **Management:** Provide resources and enforce this policy within their areas of responsibility.
- **Security and Compliance Teams:** Monitor data classification and handling controls, provide guidance, and coordinate improvements.

## Compliance

Failure to adhere to this policy may result in disciplinary action, up to and including termination, and may expose the organization to legal or regulatory penalties.

## Review

This policy will be reviewed at least annually and updated as necessary to remain effective and compliant with relevant requirements.

## Revision History

| Version | Date       | Description                                                                | Author |
| ------- | ---------- | -------------------------------------------------------------------------- | ------ |
| 1.0     | 2023-01-01 | Initial policy release                                                     | WEvans Director |
| 1.1     | 2025-09-10 | Added classification levels, handling procedures and technical controls | ChatGPT |
| 2.0     | 2025-09-10 | Implementation guidelines added | Policy Team |

## Implementation Guidelines
- All requests and approvals must be tracked in the ServiceDesk system.
- Data at rest must use AES-256 encryption; data in transit must use TLS 1.2+ with perfect forward secrecy.
- Security events shall log to the central SIEM and be retained for 12 months.
- Control owners perform quarterly self-assessments; Information Security conducts annual audits.
- Exceptions require written CISO approval and must include compensating controls.

