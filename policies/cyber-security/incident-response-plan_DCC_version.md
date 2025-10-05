# Incident Response Plan (DCC Version)

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** Wayne Evans (Director)
**Applicable Frameworks:** DEF STAN 05-138 Issue 4, DCPP Level 2 (Balanced Profile), ISO/IEC 27035, NCSC Cyber Assessment Framework

This Defence Cyber Contractor (DCC) incident response plan extends the corporate Incident Response Plan to satisfy Ministry of Defence (MOD) contractual obligations, Defence Cyber Protection Partnership (DCPP) supplier requirements, and the notification and liaison duties contained in DEF STAN 05-138 and the DCC Level 2 guide.

## Cyber Ask Operating Context

1. Cyber Ask Ltd operates with a single employee who also serves as the sole director responsible for governance, risk, and compliance decisions.
2. Cyber Ask Ltd maintains professional liability insurance covering its consulting and advisory services.
3. A dedicated virtual machine functions as the single Windows Server domain controller and is synchronized with Microsoft Entra ID for identity management.
4. The organisation holds a standard Microsoft 365 licence; Microsoft Purview and Microsoft Defender add-ons are not deployed, and Windows Defender provides endpoint protection.
5. Customer data is stored on BitLocker-encrypted drives to protect information at rest.
6. Cyber Ask Ltd assets are vulnerability-assessed weekly and patched promptly according to remediation guidance.
7. Cyber Ask Ltd has not yet achieved Cyber Essentials, Cyber Essentials Plus, or ISO 27001 certification but aligns its controls with those standards where practicable.
8. The Director personally fulfils HR, IT administration, and compliance duties, engaging specialist suppliers when additional expertise is required.



## Purpose and Scope

This plan governs how Cyber Ask Ltd detects, triages, reports, and recovers from cybersecurity incidents impacting MOD contracts, MOD information, or DCPP-mandated controls. It applies to all staff, third parties, and subcontractors handling MOD data classified as OFFICIAL, OFFICIAL-SENSITIVE, SECRET, or mission-essential services delivered under DCC Level 2 contracts.

## MOD and DCPP Notification Triggers and Timelines

DCPP requires rapid notification through official MOD channels when an incident meets the thresholds defined in DEF STAN 05-138 Annex D and the DCC Level 2 (Balanced) guide. Cyber Ask Ltd will apply the following triggers and timelines:

| Trigger | Examples | Reporting timeline | Primary contact channel | Accountable owner |
| --- | --- | --- | --- | --- |
| Confirmed or suspected compromise, loss, or unauthorized disclosure of MOD OFFICIAL-SENSITIVE or higher data | Exfiltration of design artefacts, accidental disclosure, confirmed ransomware, loss of encrypted media with MOD data | Notify within 24 hours of detection. Provide initial notification immediately after classification, even if facts are incomplete. | Submit the MOD Cyber Incident Notification Form via the Defence Supplier Portal or email the DCPP Incident Management mailbox listed in DEF STAN 05-138 Annex D (currently **dcpp-ir@mod.gov.uk**) and call the 24/7 Defence Cyber Incident Hotline (**+44 (0)30 6770 7025**). | Incident Response Coordinator (IRC) with Legal & Compliance support |
| Significant loss of confidentiality, integrity, or availability of systems delivering contracted outputs | Service outage affecting MOD deliverables, compromise of build pipeline, unauthorized changes to deployed capability | Notify within 24 hours. Provide follow-up situational reports every 24 hours until service is restored or risk mitigated. | Email the contracting authority Commercial/Project Officer using secure MODNET or encrypted email, copying the DCPP Incident mailbox. | IRC and Contract Manager |
| Incidents involving Critical or High impact per MOD impact categories (see “Incident Severity Classification”) | Any event classified Category 1 or Category 2 | Immediate escalation (within 1 hour internally) and external notification within 24 hours. | Call the MOD Cyber Security Operations Centre (CSOC) watchkeeper using the number published in current contract security instructions (recorded in the secure contact directory) and confirm in writing via the official mailbox. | Director or delegate |
| Notifiable personal data breaches involving MOD personnel | Loss of MOD personnel records, compromise of HR systems supporting MOD contract | Notify MOD authority and DCPP within 24 hours; notify the ICO within 72 hours when required. | DCPP Incident mailbox plus MOD Commercial Officer and MOD Data Protection Officer (per contract). | Data Protection Officer |
| Incidents requiring law-enforcement liaison (e.g., fraud, insider threat) | Evidence of criminal activity involving MOD assets | Notify MOD Police or Defence Serious Crime Unit via contacts provided in DEF STAN 05-138 Annex F immediately after containment actions approved by Legal. | Telephone the Defence Serious Crime Unit control room (per secure directory) and record in incident log. | Legal Counsel |

**Note:** Contact details are controlled information. The Security Administrator maintains the validated numbers and mailboxes from the current contract pack; quarterly checks verify that the annex listings match the DCPP supplier portal. Alternate channels (secure MODNET Teams bridge) may be used only when pre-approved in writing by the MOD Cyber representative.

## Notification Procedures for Contracting Authorities and DCPP

1. **Initial Assessment** – The SOC raises a suspected incident ticket and applies the MOD impact category. The IRC confirms whether contractual thresholds are met and triggers the DCC notification workflow when criteria above apply.
2. **Internal Authorization** – Within one hour of classification, the IRC briefs the Director, Legal, and Contract Manager. Legal validates that disclosure aligns with export controls and protective marking rules.
3. **Prepare MOD Cyber Incident Notification Form** – Use the current template from the DCPP supplier portal (mirrored internally as `templates/security-incident-report-template.md`). Populate mandatory metadata (contract reference, DUNS number, DCPP profile, protective marking, incident synopsis, containment status, evidence safeguarding measures).
4. **Submission Sequence** –
   1. Submit the completed form via the Defence Supplier Portal (DSP) secure upload.
   2. Email the same form (or DSP receipt) to the DCPP Incident Management mailbox and the MOD contracting authority using secure email (MODNET, encrypted TLS 1.2+, or approved cross-domain gateway).
   3. If portal access is unavailable, call the hotline to provide verbal notification, then follow up with written confirmation within four hours.
5. **Stakeholder Liaison** – Coordinate with the MOD Cyber representative, Commercial Officer, and project stakeholders to agree on public communications, operational workarounds, and any requirement for joint investigations or site access.
6. **Evidence Preservation** – Record all submissions, acknowledgements, and directives in the incident case file. Retain evidence artifacts, chain-of-custody logs, and communication transcripts for a minimum of six years or the duration mandated by contract Schedule H (whichever is longer). Maintain immutable storage copies in accordance with the Forensics and Evidence Handling Policy.
7. **Ongoing Reporting** – Provide situation reports (SITREPs) to DCPP and the contracting authority at intervals agreed during the initial notification (default cadence: every 24 hours for Category 1/2 incidents, every 48 hours for Category 3 until closure). Include progress against action items, residual risk, and planned recovery milestones.
8. **Closure** – Submit a final incident report within 10 working days of containment/eradication confirmation. The final report must include lessons learned, remedial actions, evidential summary, and statement of continued evidence retention.

## Responsibilities

1. **Incident Response Coordinator (IRC):** Owns execution of this DCC notification plan, ensures timely reporting, and maintains liaison logs.
2. **Contract Manager:** Acts as the primary interface with MOD Commercial and contracting authority, ensuring contractual obligations are met.
3. **Legal & Compliance:** Confirms reporting obligations, approves evidence disclosure, and coordinates any law-enforcement engagement.
4. **Security Operations Center (SOC):** Detects events, collates technical evidence, maintains the incident record, and supports forensic collection.
5. **Data Protection Officer (DPO):** Assesses personal data breach implications and coordinates with MOD DPO and ICO as required.
6. **CISO:** Provides executive oversight, authorizes resource allocation, and ensures strategic alignment with MOD expectations.
7. **All Staff and Suppliers:** Report anomalies promptly and support investigations. Suppliers must cascade these obligations to their subcontractors through contract clauses and onboarding briefings.

## Incident Severity Classification (MOD Impact Categories)

Cyber Ask Ltd aligns severity levels with MOD impact categories defined in DEF STAN 05-138:

| Severity label | MOD impact category | Description | Required actions |
| --- | --- | --- | --- |
| **Critical** | Category 1 (Very High) | Catastrophic impact on MOD operations, safety, or mission assurance; compromise of SECRET or higher assets. | Immediate executive and MOD CSOC escalation (within 1 hour), 24-hour reporting to DCPP, hourly internal updates, consider activating Crisis Management Team and MOD Gold/Silver command liaison. |
| **High** | Category 2 (High) | Major degradation of MOD capability, compromise of OFFICIAL-SENSITIVE data at scale, or extended service outage affecting contracted outputs. | Notify MOD/DCPP within 24 hours, initiate joint response bridge with MOD Cyber and prime contractors, deliver 24-hour SITREPs. |
| **Medium** | Category 3 (Moderate) | Limited impact to a subset of MOD services or data, contained malware, or short-term outages with workarounds. | Evaluate notification requirement; if MOD deliverables or data are involved, advise MOD Contract Manager within 48 hours and log decision. Maintain evidence for 6 years. |
| **Low** | Category 4 (Low) | Minimal impact, fully contained, no MOD data exposure. | Manage internally, document in incident log, include in monthly trend report. Upgrade classification if new information emerges. |

Severity re-evaluation occurs whenever new facts emerge. Downgrades require documented approval from the Director and confirmation from the MOD contracting authority.

## Liaison Requirements with MOD Cyber and Stakeholders

1. Establish and maintain a secure communication workspace (MODNET Teams or approved encrypted bridge) for each Category 1–2 incident. Access is granted to MOD Cyber, Commercial Officers, prime contractors, and relevant stakeholders.
2. Assign a dedicated Liaison Officer to attend MOD cyber response coordination calls, provide technical SMEs, and capture action items.
3. Share digital forensics artefacts through the secure file transfer mechanism specified by MOD (e.g., Defence SharePoint, secure FTP) only after MOD approval.
4. Ensure subcontractors cooperate with MOD site visits or inspections within the timeframes stipulated by DEF STAN 05-138.

## Training, Awareness, and Exercises

1. Conduct DCC-focused incident response tabletop exercises at least quarterly, incorporating MOD communication injects and cross-organisation coordination.
2. Execute one joint technical simulation annually with MOD Cyber or prime contractors (e.g., red team scenario or ransomware play) to validate readiness.
3. Provide onboarding briefings for all project staff and suppliers covering MOD impact categories, notification obligations, and use of secure channels.
4. Maintain training records for a minimum of six years and review exercise outcomes within 30 days to capture lessons learned.

## Evidence Management and Retention

1. Follow the Forensics and Evidence Handling Policy for chain-of-custody, storage, and access controls.
2. Retain evidence artefacts, system images, communication logs, and SITREPs for at least six years or longer when contract schedules require (e.g., safety-critical programmes may mandate 10-year retention).
3. Store evidence in the designated secure repository with role-based access, immutable logging, and escrowed encryption keys.
4. Provide evidence availability attestations to MOD auditors upon request and document any release in the evidence disclosure log.

## Metrics and Reporting

1. Track mean time to notify MOD/DCPP (MTTN) with a 24-hour maximum target for Category 1–2 incidents.
2. Report quarterly to the Executive Leadership Team on DCC incidents, training participation, and audit findings.
3. Maintain a compliance dashboard showing notification timeliness, liaison engagement, and remediation progress.

## Plan Maintenance

1. Review this plan semi-annually or upon MOD/DCPP directive changes.
2. Validate contact channels quarterly and after any MOD communications advising updated details.
3. Synchronize updates with the corporate Incident Response Plan and communicate changes to all stakeholders.

## Revision History (DCC Version)

| Version | Date | Description | Author |
| --- | --- | --- | --- |
| 1.0 | 2024-04-15 | Initial DCC-aligned incident response plan issued. | Defence Cyber Compliance Lead |
| 1.1 | 2025-09-15 | Updated MOD/DCPP notification triggers, impact categories, liaison procedures, evidence retention, and training expectations per DEF STAN 05-138 Issue 4 and DCC Level 2 guidance. | Defence Cyber Compliance Lead |
| 1.2     | 2025-10-05 | Author attribution updated | Wayne Evans (Director) |

