# Regulatory and Legal Compliance Policy

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** WEvans Director

## Purpose
This policy establishes requirements for regulatory and legal compliance to protect organizational assets and ensure compliance with applicable laws and regulations.

## Scope
This policy applies to all employees, contractors, and third parties who access or manage company resources related to regulatory and legal compliance.

## Policy

### Regulatory Landscape
- The company maintains a register of applicable laws and regulations including, but not limited to, the UK Data Protection Act 2018, UK GDPR, Computer Misuse Act 1990, PCI DSS, and relevant industry guidance from the FCA and NCSC.
- Each regulation within the register is assigned an owner responsible for monitoring changes and ensuring that business processes remain compliant.

### Compliance Management
- A Data Protection Officer (DPO) oversees adherence to privacy legislation and coordinates responses to data subject requests in line with the [Records of Processing Policy](records-of-processing-policy.md) and the [Data Protection and Privacy Policy](../cyber-security/data-protection-and-privacy-policy.md).
- Compliance obligations are reviewed quarterly. Evidence such as audit reports, training records, and contracts are stored in the compliance management system for a minimum of six years.
- Significant regulatory changes trigger a risk assessment and updates to affected policies and procedures via the Change Management process.
- Third parties providing services on behalf of the company must evidence compliance with applicable laws through contractual clauses and regular attestations.

### Reporting and Escalation
- Suspected legal or regulatory breaches must be reported to the Compliance Manager within one business day.
- Non-compliance issues are logged in the ticketing system, assigned to control owners, and tracked until closure.
- Serious breaches are escalated to the board and, where required, reported to the Information Commissioner’s Office within 72 hours.

## Technical Controls
- Compliance management tools track regulatory obligations, map them to controls, and produce audit-ready evidence.
- Access to compliance records is restricted based on least privilege and protected with multi-factor authentication.
- Automated alerts notify the Compliance Manager when regulatory deadlines or contract renewals approach.

## Roles and Responsibilities
- **Employees and Contractors:** Follow regulatory and legal compliance procedures and report issues or non-compliance.
- **Management:** Provide resources and enforce this policy within their areas of responsibility.
- **Security and Compliance Teams:** Monitor regulatory and legal compliance controls, provide guidance, and coordinate improvements.

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

| Version | Date       | Description                                                       | Author |
| ------- | ---------- | ----------------------------------------------------------------- | ------ |
| 1.0     | 2023-01-01 | Initial policy release                                            | WEvans Director |
| 1.1     | 2025-09-10 | Detailed regulatory register, compliance process and cross-references added | ChatGPT |
| 2.0     | 2025-09-10 | Implementation guidelines added | Policy Team |

## Implementation Guidelines
- All requests and approvals must be tracked in the ServiceDesk system.
- Data at rest must use AES-256 encryption; data in transit must use TLS 1.2+ with perfect forward secrecy.
- Security events shall log to the central SIEM and be retained for 12 months.
- Control owners perform quarterly self-assessments; Information Security conducts annual audits.
- Exceptions require written CISO approval and must include compensating controls.

