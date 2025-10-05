# Data Classification Policy (DCC / MOD-Aligned)

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** WEvans Director  
**Applicable Contract:** Defence Cyber Protection Partnership (DCPP) – Dynamic Purchasing System, DCC Level 2  
**Reference Standards:** DEF STAN 05-138 Issue 4, DCC Level 2 Supplier Cyber Protection Guide, ISO/IEC 27001:2022

This policy tailors the corporate Data Classification Policy for engagements requiring Ministry of Defence (MOD) and Defence Cyber
Catalogue (DCC) compliance. It supplements, and does not replace, the corporate policy; where conflicts occur this version prevails
for DCC deliverables.

## Cyber Ask Operating Context

1. Cyber Ask Ltd operates with a single employee who also serves as the sole director responsible for governance, risk, and compliance decisions.
2. Cyber Ask Ltd maintains professional liability insurance covering its consulting and advisory services.
3. A dedicated virtual machine functions as the single Windows Server domain controller and is synchronized with Microsoft Entra ID for identity management.
4. The organisation holds a standard Microsoft 365 licence; Microsoft Purview and Microsoft Defender add-ons are not deployed, and Windows Defender provides endpoint protection.
5. Customer data is stored on BitLocker-encrypted drives to protect information at rest.
6. Cyber Ask Ltd assets are vulnerability-assessed weekly and patched promptly according to remediation guidance.
7. Cyber Ask Ltd has not yet achieved Cyber Essentials, Cyber Essentials Plus, or ISO 27001 certification but aligns its controls with those standards where practicable.
8. The Director personally fulfils HR, IT administration, and compliance duties, engaging specialist suppliers when additional expertise is required.



## Scope

This policy applies to all information assets created, processed, stored, or transmitted in support of DCC contractual obligations,
including subcontractor environments handling Cyber Ask Ltd controlled information.

## Classification Levels and Protective Markings

The following tiers integrate MOD protective markings, ensuring consistency with DEF STAN 05-138 Issue 4 and the DCC Level 2
Supplier Cyber Protection Guide.

| Corporate Tier | MOD Protective Marking | Description | Examples |
| -------------- | ---------------------- | ----------- | -------- |
| Public | Not Official | Information approved for release without restriction. | Published marketing collateral, openly issued RFIs. |
| Internal | OFFICIAL | Routine business information that requires integrity and availability protection but presents low confidentiality risk. | Internal project tracking, approved supplier contact lists. |
| Confidential | OFFICIAL-SENSITIVE | Sensitive business or operational data warranting enhanced controls to mitigate compromise. | DCC bid documentation, MOD commercial-in-confidence data, security architecture diagrams. |
| Restricted | SECRET / TOP SECRET (if contractually required) | Highly sensitive national security or mission-critical data requiring the highest safeguards and MOD authorisation. Cyber Ask Ltd will only process SECRET/TOP SECRET data when explicitly authorised within contract schedules. | Classified design artefacts, threat intelligence, operational plans. |

Data Owners must record both the corporate tier and MOD protective marking on all relevant artefacts, ensuring handling
requirements meet the more stringent requirement when tiers diverge.

## Marking and Labelling Requirements

1. Apply clear text markings (e.g., "OFFICIAL-SENSITIVE") in document headers/footers and on electronic file metadata in accordance
  with DEF STAN 05-138 Issue 4 guidance.
1. Use cover sheets for printed OFFICIAL-SENSITIVE or higher material. Colour coding may be used where compatible with MOD
  direction.
1. Reference the Document Control Policy for versioning, distribution logs, and change control requirements.

## Handling Requirements

### Transmission
1. OFFICIAL and OFFICIAL-SENSITIVE email must use MOD-approved gateways or encrypted channels (TLS 1.2+ end-to-end); use secure
  file transfer solutions for large files in line with the Encryption Policy.
1. SECRET/TOP SECRET material may only be transferred via MOD-accredited networks or couriers authorised by the Security
  Operations Policy and Physical Security Policy.
1. Confirm recipient clearance and need-to-know before release; record transfers in the ServiceDesk system.

### Storage
1. OFFICIAL-SENSITIVE electronic data must reside in segregated environments meeting DCC Level 2 controls, with multi-factor
  authentication and role-based access enforced per the Access Control Policy and PAM Policy.
1. SECRET/TOP SECRET storage requires MOD-accredited facilities and compliance with the Physical Security Policy; use tamper-
  evident containers and offline key storage aligned with the Encryption Policy.
1. Maintain asset registers and configuration baselines in accordance with the Asset Management Policy and Secure Configuration
  Policy.

### Destruction and Media Handling
1. Follow the Media Handling and Equipment Disposal Policy for sanitisation methods commensurate with the highest protective
  marking, ensuring CESG/Cabinet Office approved destruction services for SECRET/TOP SECRET media.
1. Shred OFFICIAL-SENSITIVE paper to cross-cut standard or higher; log destruction events and retain certificates in accordance with
  the Records Management and Archiving Policy.

### Subcontractor and Third-Party Obligations
1. Subcontractors handling OFFICIAL-SENSITIVE or above must demonstrate compliance with DCC Level 2 controls, sign NDAs, and be
  onboarded through the Supplier Security Policy and Outsourcing Governance Policy.
1. Contracts must require immediate notification of incidents, cooperation with MOD authorities, and adherence to the Incident
  Response Policy and Forensics and Evidence Handling Policy.
1. Perform annual assurance reviews of subcontractor controls and retain evidence per the Internal Audit Policy.

## Evidence Retention and Auditability

1. Retain classification registers, distribution logs, and handling attestations for a minimum of seven (7) years or the period
  specified by MOD/DCC directives, whichever is longer.
1. Preserve incident and investigation records for at least seven (7) years and until all MOD-directed actions are closed, aligning
  with the Incident Response Policy and Records Management and Archiving Policy.
1. Maintain destruction certificates, transfer receipts, and subcontractor assurance reports for audit review and MOD inspection.

## Roles and Responsibilities

1. **Data Owners:** Determine classification and protective marking, ensuring records align with contractual security requirements.
2. **Users:** Handle data according to this policy, complete MOD/DCC awareness training, and report breaches immediately.
3. **Director:** Oversees implementation, coordinates with MOD security authorities, and maintains alignment
  with the Cyber Governance Policy.
1. **CISO:** Approves exceptions, risk acceptances, and compensating controls in line with the Risk Management Policy and the
  Incident Response Policy.
1. **Commercial Director:** Ensures contractual clauses incorporate MOD/DCC requirements for subcontractors and evidence retention.

Exception requests must follow the process in the Cyber Governance Policy and be recorded in accordance with the Document Control
Policy.

## Review

This policy will be reviewed at least annually, after significant MOD/DCC guidance changes, or following relevant incident
findings.

## Implementation and Assurance

1. All requests and approvals must be tracked in the ServiceDesk system.
2. Conduct quarterly control self-assessments against DCC Level 2 requirements; report outcomes to the Risk and Compliance Committee
  per the Continuous Improvement Policy.
1. Integrate monitoring events into the central SIEM with 12-month minimum log retention, noting MOD-specific alerting rules.
2. Exceptions require written approval from the Director and must include MOD/DCC-endorsed compensating controls.

## Revision History

| Version | Date | Description | Author |
| ------- | ---------- | ----------- | ------ |
| 3.0-DCC | 2025-11-24 | Introduced MOD protective markings, DCC handling controls, and evidence retention updates. | Policy Team |
