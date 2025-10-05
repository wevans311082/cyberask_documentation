# Regulatory and Legal Compliance Policy

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
This policy establishes requirements for regulatory and legal compliance to protect organizational assets and ensure compliance with applicable laws and regulations.

## Scope
This policy applies to all employees, contractors, and third parties who access or manage company resources related to regulatory and legal compliance.

## Policy

### Regulatory Landscape
1. The company maintains a register of applicable laws and regulations including, but not limited to, the UK Data Protection Act 2018, UK GDPR, Computer Misuse Act 1990, PCI DSS, and relevant industry guidance from the FCA and NCSC.
2. Each regulation within the register is assigned an owner responsible for monitoring changes and ensuring that business processes remain compliant.

### Compliance Management
1. A Data Protection Officer (DPO) oversees adherence to privacy legislation and coordinates responses to data subject requests in line with the [Records of Processing Policy](records-of-processing-policy.md) and the [Data Protection and Privacy Policy](../cyber-security/data-protection-and-privacy-policy.md).
2. Compliance obligations are reviewed quarterly. Evidence such as audit reports, training records, and contracts are stored in the compliance management system for a minimum of six years.
3. Significant regulatory changes trigger a risk assessment and updates to affected policies and procedures via the Change Management process.
4. Third parties providing services on behalf of the company must evidence compliance with applicable laws through contractual clauses and regular attestations.

### Reporting and Escalation
1. Suspected legal or regulatory breaches must be reported to the Compliance Manager within one business day.
2. Non-compliance issues are logged in the ticketing system, assigned to control owners, and tracked until closure.
3. Serious breaches are escalated to the board and, where required, reported to the Information Commissioner’s Office within 72 hours.

## Technical Controls
1. Compliance management tools track regulatory obligations, map them to controls, and produce audit-ready evidence.
2. Access to compliance records is restricted based on least privilege and protected with multi-factor authentication.
3. Automated alerts notify the Compliance Manager when regulatory deadlines or contract renewals approach.

## Roles and Responsibilities
1. **Employees and Contractors:** Follow regulatory and legal compliance procedures and report issues or non-compliance.
2. **Management:** Provide resources and enforce this policy within their areas of responsibility.
3. **Security and Compliance Teams:** Monitor regulatory and legal compliance controls, provide guidance, and coordinate improvements.

## Accountable Roles and Decision Authority

1. **Director:** Owns and maintains this policy, coordinates updates, and ensures alignment with the Cyber Governance Policy and Document Control Policy.
2. **Director (Risk Owner):** Reviews and approves exceptions, risk acceptances, and material control changes, documenting rationale in line with the Risk Management Policy.
3. **Director (Service Owner):** Oversees day-to-day execution of this policy, vendor engagement, and customer communications when actions affect external parties.


## Compliance
Failure to adhere to this policy may result in disciplinary action, up to and including termination, and may expose the organization to legal or regulatory penalties.

## Review
This policy will be reviewed at least annually and updated as necessary to remain effective and compliant with relevant requirements.

## Revision History

| Version | Date       | Description                                                       | Author |
| ------- | ---------- | ----------------------------------------------------------------- | ------ |
| 1.0     | 2023-01-01 | Initial policy release                                            | Wayne Evans (Director) |
| 1.1     | 2025-09-10 | Detailed regulatory register, compliance process and cross-references added | ChatGPT |
| 2.0     | 2025-09-10 | Implementation guidelines added | Policy Team |
| 2.1     | 2025-10-05 | Author attribution updated | Wayne Evans (Director) |

## Implementation Guidelines
1. The Director records policy-related approvals and evidence in the central document repository and retains them for audit purposes.
2. BitLocker-encrypted storage protects customer data on company systems, and Windows Defender telemetry is reviewed weekly.
3. Weekly vulnerability scans and monthly patch reviews are led by the Director, with remediation actions tracked to completion.
4. Microsoft 365 security settings rely on features provided within the standard licence; compensating controls are documented when advanced tooling is unavailable.
5. Exceptions require written approval from the Director, including compensating controls and a defined review date.

