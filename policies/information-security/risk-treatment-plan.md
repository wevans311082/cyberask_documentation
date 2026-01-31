# Risk Treatment Plan

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** Wayne Evans (Director)

This plan documents actions to address identified information security risks, fulfilling ISO 27001 requirements.

## Cyber Ask Operating Context

1. Cyber Ask Ltd operates with a single employee who also serves as the sole director responsible for governance, risk, and compliance decisions.
2. Cyber Ask Ltd maintains professional liability insurance covering its consulting and advisory services.
3. A dedicated virtual machine functions as the single Windows Server domain controller and is synchronized with Microsoft Entra ID for identity management.
4. The organisation holds a standard Microsoft 365 licence; Microsoft Purview and Microsoft Defender add-ons are not deployed, and Windows Defender provides endpoint protection.
5. Customer data is stored on BitLocker-encrypted drives to protect information at rest.
6. Cyber Ask Ltd assets are vulnerability-assessed weekly and patched promptly according to remediation guidance.
7. Cyber Ask Ltd has not yet achieved Cyber Essentials, Cyber Essentials Plus, or ISO 27001 certification but aligns its controls with those standards where practicable.
8. The Director personally fulfils HR, IT administration, and compliance duties, engaging specialist suppliers when additional expertise is required.



## Plan Details

1. **Risk ID:** Reference to Risk Assessment Report.
2. **Selected Controls:** Controls implemented or planned to mitigate the risk.
3. **Responsible Owner:** Individual accountable for implementing the treatment.
4. **Target Date:** Expected completion date for treatment activities.
5. **Residual Risk:** Level of risk remaining after treatment and acceptance decision.

## Treatment Actions

| Risk ID | Treatment Actions | Selected Controls (SoA) | Owner | Target Date | Residual Risk | Status |
| --- | --- | --- | --- | --- | --- | --- |
| R1 | Require supplier assurance evidence for AI model updates, document AI supplier risk reviews, and introduce validation checks on outputs before client delivery. | A.5.19, A.5.21, A.8.25 | Director | 2025-05-10 | L2/I4 (Medium) | In Progress |
| R2 | Enable immutable backup policies where available, document offline export cadence, and test restoration quarterly. | A.5.24, A.8.13, A.8.16 | Director | 2025-05-20 | L2/I4 (Medium) | In Progress |
| R3 | Roll out phishing-resistant MFA, enforce conditional access for risky sign-ins, and increase session monitoring. | A.5.17, A.8.5, A.8.16 | Director | 2025-04-30 | L2/I3 (Medium) | Planned |
| R4 | Publish AI prompt hygiene guidance, segregate client datasets, and add review checklist for AI-assisted outputs. | A.5.10, A.5.12, A.8.11 | Director | 2025-05-15 | L2/I3 (Medium) | Planned |
| R5 | Establish configuration baselines, weekly drift reviews, and alerting for public sharing changes. | A.8.9, A.8.16, A.8.20 | Director | 2025-05-05 | L2/I3 (Medium) | Planned |
| R6 | Maintain rapid patch SLA for Teams add-ins and monitor vendor security advisories weekly. | A.8.8, A.8.19, A.8.20 | Director | 2025-04-15 | L2/I3 (Medium) | Monitoring |
| R7 | Implement dual-approval for invoices and require out-of-band verification for changes to payment details. | A.5.2, A.5.15, A.8.2 | Director | 2025-04-22 | L2/I2 (Low) | Planned |
| R8 | Complete annual supplier assurance review and restrict shared admin access to time-bound sessions. | A.5.19, A.5.22, A.8.21 | Director | 2025-06-01 | L2/I4 (Medium) | Planned |
| R9 | Require signed scripts, introduce integrity checks in CI, and segregate dev/test automation. | A.8.28, A.8.31, A.8.32 | Director | 2025-05-25 | L1/I3 (Low) | Planned |
| R10 | Approve PQC migration roadmap, classify long-term archives, and reduce retention where contractual allowances permit. | A.8.24, A.8.13, A.8.27 | Director | 2025-07-15 | L1/I4 (Medium) | Planned |
| R11 | Document deputy coverage, cross-train suppliers for incident response, and add escalation criteria. | A.5.2, A.5.24, A.6.3 | Director | 2025-05-01 | L2/I2 (Low) | In Progress |
| R12 | Implement evidence tracker with monthly checkpoints and standardised templates for client reporting. | A.5.33, A.5.37, A.8.15 | Director | 2025-05-12 | L1/I2 (Low) | Planned |
| R14 | Add secondary connectivity option, document continuity checklist, and conduct semi-annual outage drills. | A.5.29, A.5.30, A.8.14 | Director | 2025-06-10 | L2/I2 (Low) | Planned |

## Accountable Roles and Decision Authority

1. **Director:** Owns and maintains this policy, coordinates updates, and ensures alignment with the Cyber Governance Policy and Document Control Policy.
2. **Director (Risk Owner):** Reviews and approves exceptions, risk acceptances, and material control changes, documenting rationale in line with the Risk Management Policy.
3. **Director (Service Owner):** Oversees day-to-day execution of this policy, vendor engagement, and customer communications when actions affect external parties.


## Monitoring

Risk owners provide status updates monthly until treatments are complete.

## Approval

Management approves the plan and residual risk levels.

**Approval Date:** 2025-03-15  
**Approved By:** Wayne Evans (Director)

## Implementation Guidelines
1. The Director records policy-related approvals and evidence in the central document repository and retains them for audit purposes.
2. BitLocker-encrypted storage protects customer data on company systems, and Windows Defender telemetry is reviewed weekly.
3. Weekly vulnerability scans and monthly patch reviews are led by the Director, with remediation actions tracked to completion.
4. Microsoft 365 security settings rely on features provided within the standard licence; compensating controls are documented when advanced tooling is unavailable.
5. Exceptions require written approval from the Director, including compensating controls and a defined review date.


## Revision History

| Version | Date | Description | Author |
| ------- | ---------- | ----------------------- | ------ |
| 2.0     | 2025-09-10 | Implementation guidelines added | Policy Team |
| 2.1     | 2025-10-05 | Author attribution updated | Wayne Evans (Director) |
| 2.2     | 2025-03-15 | Populated treatment actions with risk IDs, controls, and dates | Wayne Evans (Director) |
