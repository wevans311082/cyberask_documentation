# Account Separation Policy

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** WEvans Director

## Purpose

This policy establishes requirements for account separation to protect organizational assets and ensure compliance with applicable laws and regulations.

## Scope

This policy applies to all employees, contractors, and third parties who access or manage company resources related to account separation.

## Policy

### Account Types
- **Standard User Accounts:** Issued to individual staff for everyday work. Users must not run administrative tasks with these accounts.
- **Privileged Administrative Accounts:** Separate credentials with elevated rights, protected by multi-factor authentication and used solely for system administration.
- **Service Accounts:** Non-interactive accounts used by applications or integrations. Passwords must be at least 24 characters, rotated every 90 days and stored in the privileged access management (PAM) vault. Interactive logon is disabled.

### Access Request and Approval
- New accounts or privilege changes shall be requested through the ServiceDesk ticketing system and approved by the requestor’s line manager and the Information Security Manager.
- Shared accounts are prohibited. Any exception must be documented, time-bound, and approved by the CTO with compensating controls.
- HR must notify IT within one working day of staff changes so that accounts can be created, modified, or revoked promptly in accordance with the [Access Control Policy](../cyber-security/access-control-policy.md).

### Review and Monitoring
- Privileged accounts are reviewed quarterly; standard user accounts are reviewed annually. Reviews verify necessity, correct privilege level and appropriate ownership.
- Logs recording account creation, privilege escalation, and deletion are retained for a minimum of twelve months and reviewed weekly for unauthorised activity.
- Non-compliance or suspicious activity must be escalated to the Information Security Manager within one hour of detection.

## Technical Controls

- Identity and access management (IAM) tools enforce separation of duties and least privilege.
- Automated monitoring alerts on creation or modification of privileged accounts.
- The PAM system enforces credential rotation for service and administrative accounts and provides session recording for elevated activities.

## Roles and Responsibilities

- **Employees and Contractors:** Follow account separation procedures and report issues or non-compliance.
- **Management:** Provide resources and enforce this policy within their areas of responsibility.
- **Security and Compliance Teams:** Monitor account separation controls, provide guidance, and coordinate improvements.

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
- All requests and approvals must be tracked in the ServiceDesk system.
- Data at rest must use AES-256 encryption; data in transit must use TLS 1.2+ with perfect forward secrecy.
- Security events shall log to the central SIEM and be retained for 12 months.
- Control owners perform quarterly self-assessments; Information Security conducts annual audits.
- Exceptions require written CISO approval and must include compensating controls.

