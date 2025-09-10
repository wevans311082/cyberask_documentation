# Scope of the ISMS

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** WEvans Director

This document defines the boundaries and applicability of the Information Security Management System (ISMS) in accordance with ISO 27001.

## Boundaries

- Covers all business processes, information systems, and physical locations used to deliver core services to customers.
- Excludes personal devices not used for company business and third-party infrastructure outside contractual control.

## Interfaces and Dependencies

- Relies on cloud service providers for hosting and follows their shared responsibility models.
- Integrates with corporate HR and legal functions for personnel and contractual controls.

## Assumptions

- All personnel accessing in-scope systems are subject to company security policies and training.

## Approval

Senior management approves this scope statement and reviews it annually or when significant organizational changes occur.

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
