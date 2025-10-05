# Account Separation Policy

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** WEvans Director

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

This policy establishes requirements for account separation to protect organizational assets and ensure compliance with applicable laws and regulations.

## Scope

This policy applies to all employees, contractors, and third parties who access or manage company resources related to account separation.

## Policy

### Account Types
1. **Standard User Accounts:** Issued to individual staff for everyday work. Users must not run administrative tasks with these accounts.
2. **Privileged Administrative Accounts:** Separate credentials with elevated rights, protected by multi-factor authentication and used solely for system administration.
3. **Service Accounts:** Non-interactive accounts used by applications or integrations. Passwords must be at least 24 characters, rotated every 90 days and stored in the privileged access management (PAM) vault. Interactive logon is disabled.

### Access Request and Approval
1. New accounts or privilege changes shall be requested through the ServiceDesk ticketing system and approved by the requestor’s line manager and the Director.
2. Shared accounts are prohibited. Any exception must be documented, time-bound, and approved by the CTO with compensating controls.
3. HR must notify IT within one working day of staff changes so that accounts can be created, modified, or revoked promptly in accordance with the [Access Control Policy](../cyber-security/access-control-policy.md).

### Review and Monitoring
1. Privileged accounts are reviewed quarterly; standard user accounts are reviewed annually. Reviews verify necessity, correct privilege level and appropriate ownership.
2. Logs recording account creation, privilege escalation, and deletion are retained for a minimum of twelve months and reviewed weekly for unauthorised activity.
3. Non-compliance or suspicious activity must be escalated to the Director within one hour of detection.

## Technical Controls

1. Identity and access management (IAM) tools enforce separation of duties and least privilege.
2. Automated monitoring alerts on creation or modification of privileged accounts.
3. The PAM system enforces credential rotation for service and administrative accounts and provides session recording for elevated activities.

## Roles and Responsibilities

1. **Employees and Contractors:** Follow account separation procedures and report issues or non-compliance.
2. **Management:** Provide resources and enforce this policy within their areas of responsibility.
3. **Security and Compliance Teams:** Monitor account separation controls, provide guidance, and coordinate improvements.

## Accountable Roles and Decision Authority

1. **Director:** Owns and maintains this policy, coordinates updates, and ensures alignment with the Cyber Governance Policy and Document Control Policy.
2. **Director (Risk Owner):** Reviews and approves exceptions, risk acceptances, and material control changes, documenting rationale in line with the Risk Management Policy.
3. **Director (Service Owner):** Oversees day-to-day execution of this policy, vendor engagement, and customer communications when actions affect external parties.


## Compliance

Failure to adhere to this policy may result in disciplinary action, up to and including termination, and may expose the organization to legal or regulatory penalties.

## Review

This policy will be reviewed at least annually and updated as necessary to remain effective and compliant with relevant requirements.

## Revision History

| Version | Date       | Description                                                        | Author |
| ------- | ---------- | ------------------------------------------------------------------ | ------ |
| 1.0     | 2023-01-01 | Initial policy release                                             | WEvans Director |
| 1.1     | 2025-09-10 | Added account types, request workflow and monitoring requirements | ChatGPT |
| 2.0     | 2025-09-10 | Implementation guidelines added | Policy Team |

## Implementation Guidelines
1. The Director records policy-related approvals and evidence in the central document repository and retains them for audit purposes.
2. BitLocker-encrypted storage protects customer data on company systems, and Windows Defender telemetry is reviewed weekly.
3. Weekly vulnerability scans and monthly patch reviews are led by the Director, with remediation actions tracked to completion.
4. Microsoft 365 security settings rely on features provided within the standard licence; compensating controls are documented when advanced tooling is unavailable.
5. Exceptions require written approval from the Director, including compensating controls and a defined review date.

