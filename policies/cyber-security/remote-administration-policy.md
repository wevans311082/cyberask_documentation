# Remote Administration Policy

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** WEvans Director

## Purpose

This policy establishes requirements for remote administration to protect organizational assets and ensure compliance with applicable laws and regulations.

## Scope

This policy applies to all employees, contractors, and third parties who access or manage company resources related to remote administration.

## Policy
1. The organization shall define and document procedures for remote administration.
2. Controls for remote administration must align with industry best practices and regulatory obligations.
3. Activities related to remote administration shall be reviewed and updated regularly to address emerging risks.
4. Records demonstrating compliance with this policy shall be maintained.

- All aspects of Remote Administration Policy must align with ISO/IEC 27001:2022 controls and the NCSC Cyber Assessment Framework.
- Procedures shall be documented, communicated, and reviewed at least annually by the Information Security Manager.
- Staff and contractors must receive training on Remote Administration Policy before being granted related responsibilities.
- Access and activities associated with Remote Administration Policy shall be logged and monitored to detect and respond to unauthorised actions.
- Deviations from this policy must be reported within 24 hours and remedied within 30 days.
- Technology configurations supporting Remote Administration Policy must follow relevant CIS Benchmarks and vendor hardening guides.
- Third parties engaged in Remote Administration Policy processes shall have contractual obligations to meet equivalent security standards.
- Records demonstrating compliance with this policy shall be retained for audit for a minimum of six years.
- The Information Security Manager must approve exceptions in writing, including scope, duration, and compensating controls.
- Failure to comply with this policy may result in disciplinary action, removal of access, or termination of contract.

- Systems processing Remote Administration Policy shall enforce least privilege and role-based access controls.
- Changes affecting Remote Administration Policy configurations must follow the Change Management Policy and receive formal approval.
- Monitoring tools shall generate alerts for Remote Administration Policy violations and designated staff must review these alerts daily.
- Internal audits shall verify adherence to Remote Administration Policy at least annually and report findings to senior management.
- Data associated with Remote Administration Policy must be protected in accordance with GDPR and UK statutory requirements.
- Users shall acknowledge and accept this policy annually to retain relevant access rights.

## Technical Controls

- Configure and maintain systems to enforce the requirements of the Remote Administration Policy, using appropriate tools and automation.
- Enable logging, monitoring, and alerting to detect and respond to deviations from the Remote Administration Policy.
- Apply encryption, access controls, and regular audits to ensure compliance with this policy.

## Roles and Responsibilities

- **Employees and Contractors:** Follow remote administration procedures and report issues or non-compliance.
- **Management:** Provide resources and enforce this policy within their areas of responsibility.
- **Security and Compliance Teams:** Monitor remote administration controls, provide guidance, and coordinate improvements.

## Accountable Roles and Decision Authority

- **Policy Owner (Information Security Manager):** Maintains this policy, coordinates updates, and ensures alignment with the Cyber Governance Policy and Document Control Policy.
- **Chief Information Security Officer (CISO):** Approves exceptions, risk acceptances, and material control changes in line with the Information Security Policy and Risk Management Policy.
- **Risk and Compliance Committee:** Reviews escalated risks, endorses significant remediation decisions, and provides oversight consistent with the Risk Management Policy.
- **Executive Leadership Team:** Ratifies budgetary or strategic decisions related to this policy as defined in the Cyber Governance Policy.

Exception requests must follow the exception management process described in the Cyber Governance Policy and all approvals must be recorded in accordance with the Document Control Policy.

## Compliance

Failure to adhere to this policy may result in disciplinary action, up to and including termination, and may expose the organization to legal or regulatory penalties.

## Review

This policy will be reviewed at least annually and updated as necessary to remain effective and compliant with relevant requirements.

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
