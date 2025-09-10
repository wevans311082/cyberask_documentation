# Statement of Applicability

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** WEvans Director

The Statement of Applicability (SoA) lists ISO 27001 Annex A controls and their implementation status within the organization.

## Structure

- **Control Reference:** Identifier from Annex A.
- **Implementation Status:** Implemented, Planned, or Not Applicable.
- **Justification:** Reason for selection or exclusion of the control.
- **Related Documents:** Policies, procedures, or records supporting the control.

## Maintenance

- Updated whenever new controls are implemented or risks change.
- Reviewed and approved by management annually.

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
