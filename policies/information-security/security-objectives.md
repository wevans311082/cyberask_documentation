# Information Security Objectives

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** WEvans Director

This document establishes measurable objectives to guide the Information Security Management System and comply with ISO 27001.

## Objectives

- Maintain 99.9% availability for customer-facing services.
- Ensure all employees complete annual security awareness training.
- Remediate critical vulnerabilities within 14 days of discovery.
- Achieve zero successful phishing attacks through simulated testing each quarter.

## Accountable Roles and Decision Authority

- **Policy Owner (Information Security Manager):** Maintains this policy, coordinates updates, and ensures alignment with the Cyber Governance Policy and Document Control Policy.
- **Chief Information Security Officer (CISO):** Approves exceptions, risk acceptances, and material control changes in line with the Information Security Policy and Risk Management Policy.
- **Risk and Compliance Committee:** Reviews escalated risks, endorses significant remediation decisions, and provides oversight consistent with the Risk Management Policy.
- **Executive Leadership Team:** Ratifies budgetary or strategic decisions related to this policy as defined in the Cyber Governance Policy.

Exception requests must follow the exception management process described in the Cyber Governance Policy and all approvals must be recorded in accordance with the Document Control Policy.


## Monitoring and Review

The Information Security Officer tracks progress and reports results to management quarterly. Objectives are reviewed annually and updated as business needs evolve.

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
