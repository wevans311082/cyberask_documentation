# Risk Treatment Plan

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** WEvans Director

This plan documents actions to address identified information security risks, fulfilling ISO 27001 requirements.

## Plan Details

- **Risk ID:** Reference to Risk Assessment Report.
- **Selected Controls:** Controls implemented or planned to mitigate the risk.
- **Responsible Owner:** Individual accountable for implementing the treatment.
- **Target Date:** Expected completion date for treatment activities.
- **Residual Risk:** Level of risk remaining after treatment and acceptance decision.

## Monitoring

Risk owners provide status updates monthly until treatments are complete.

## Approval

Management approves the plan and residual risk levels.

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
