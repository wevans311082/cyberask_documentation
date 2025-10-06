# GDPR and UK Data Protection Act Policy (DCC Version)

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** Defence Cyber Compliance Lead

## Cyber Ask Operating Context (DCC)

1. Cyber Ask Ltd supports Ministry of Defence (MOD) contracts under Defence Cyber Protection Partnership (DCPP) frameworks requiring Defence Cyber Compliance (DCC) Level 2 assurance.
2. MOD-controlled data is processed within segregated Microsoft 365 tenants and Azure subscriptions dedicated to MOD engagements, with UK data residency enforced and Conditional Access policies mandating multi-factor authentication.
3. A secure enclave hosted on BitLocker-encrypted infrastructure with hardware-backed Trusted Platform Modules stores MOD personal data, supported by Microsoft Purview Information Protection for labelling OFFICIAL-SENSITIVE content.
4. The Director acts as Senior Information Risk Owner (SIRO) and Data Protection Officer, supported by cleared subcontractors who undergo Baseline Personnel Security Standard (BPSS) checks prior to accessing MOD data.
5. Contracts mandate adherence to DEF STAN 05-138 Issue 4, JSP 440, and relevant Joint Service Publications covering protective security, incident management, and records handling.
6. Cyber Ask Ltd maintains a Corrective and Preventive Action (CAPA) register aligned to DCC Level 2 findings, reviewed quarterly with MOD commercial representatives.
7. Security operations leverage endpoint detection and response (EDR), security information and event management (SIEM), and vulnerability management tooling scoped to MOD workloads, with weekly reporting to the DCC governance forum.

## Purpose
This DCC-aligned policy augments the corporate GDPR and UK Data Protection Act Policy to satisfy MOD contractual obligations, DCC Level 2 control expectations, and DEF STAN 05-138 privacy requirements when processing MOD personal data or data subject to security classifications up to OFFICIAL-SENSITIVE.

## Scope
This policy applies to all Cyber Ask Ltd personnel, subcontractors, and suppliers processing MOD personal data or providing services within DCC Level 2 engagements. It covers collection, storage, sharing, and disposal of MOD personal data processed within the UK, EU, or internationally when transfer derogations are approved by the MOD.

## Definitions (DCC Specific)
- **MOD Personal Data:** Any personal data provided by or generated for the MOD under contract, including OFFICIAL and OFFICIAL-SENSITIVE information.
- **Security Assurance Coordinator (SAC):** Individual designated by MOD to oversee DCPP compliance and assurance activities.
- **Protective Marking:** MOD classification applied to information (e.g., OFFICIAL, OFFICIAL-SENSITIVE) dictating handling controls.
- **MOD Delegated Authority:** Written authorisation from the MOD commercial or security authority approving specific processing, transfers, or retention beyond baseline requirements.

## Policy

### Integrated Lawful Basis and Contractual Controls
1. MOD contracts, Statements of Work, and Security Aspects Letters define lawful bases under Article 6(1)(b) (contract) and Article 6(1)(c) (legal obligation). Article 9(2)(g) and DPA 2018 Schedule 1 Part 2 Paragraph 6 (statutory and governmental purposes) govern special category data processing.
2. The DPO maintains a MOD-specific Records of Processing Activities annex mapping contractual obligations, lawful bases, protective markings, and DEF STAN 05-138 clause references.
3. Data processing agreements with cleared subcontractors must incorporate MOD-mandated flow-down clauses, audit rights, and restrictions on subcontracting without MOD approval.

### Protective Security and Technical Safeguards
1. MOD personal data must be processed only within MOD-accredited environments that meet DEF STAN 05-138 Annex F controls, including segregation from commercial workloads and enforced device hardening (CIS Level 1 benchmark minimum).
2. Multi-factor authentication, Conditional Access, and Privileged Access Workstations (PAWs) are required for administrative access. Session recording is enabled for privileged actions within the MOD enclave.
3. All data at rest must utilise AES-256 encryption with centrally managed keys stored in Hardware Security Modules (HSMs) or Azure Key Vault with UK data residency. Transfers employ MOD-approved secure gateways or encrypted Virtual Private Networks (VPNs).
4. Microsoft Purview Sensitivity Labels automate classification and encryption of OFFICIAL-SENSITIVE documents. Tamper-evident audit logs must be retained for a minimum of seven years or contractually specified period.

### Data Subject Rights in MOD Context
1. The DPO coordinates with the MOD Data Protection Officer and SAC to verify authority before responding to DSRs; where MOD retains controller status, Cyber Ask Ltd acts strictly on documented instructions.
2. DSRs impacting national security considerations require escalation to the SIRO and MOD authority. Response timelines may be extended per DPA 2018 Section 26 when exemptions apply; rationale is recorded in the DSR log.
3. For joint controller arrangements, Cyber Ask Ltd maintains memoranda of understanding (MOUs) detailing shared responsibilities, communication pathways, and dispute resolution.

### Data Protection Impact Assessments and Security Cases
1. DPIAs are mandatory for all new MOD processing activities and must integrate MOD Security Risk Assessments (SRAs) and DCC Control Evidence Matrix references. Output artefacts are provided to the SAC prior to go-live.
2. High-risk findings require documented risk treatment plans signed by the SIRO, MOD authority, and, where necessary, the Senior Responsible Owner (SRO).
3. Change management procedures ensure DPIAs, SRAs, and security cases are reviewed when introducing new systems, locations, or subcontractors.

### International Transfers and Sovereignty
1. MOD personal data must remain within the UK unless explicit MOD delegated authority authorises transfer. If transfers are approved, International Data Transfer Agreements must include MOD-specific clauses and assurance from receiving entities holding equivalent security clearances.
2. Transfer Risk Assessments consider geopolitical risk, host nation surveillance laws, and MOD protective security guidance. Results are reviewed by the SIRO and MOD authority prior to transfer initiation.

### Incident Management and Reporting
1. Personal data breaches involving MOD data trigger the [Incident Response Plan (DCC Version)](../cyber-security/incident-response-plan_DCC_version.md) and must be reported to the MOD within four hours of detection, alongside ICO notification assessments.
2. For incidents meeting DCC Level 2 severity, Cyber Ask Ltd maintains liaison logs, evidence preservation, and forensics artefacts in accordance with DEF STAN 05-138 Annex D.
3. Quarterly MOD-specific incident drills include data breach scenarios, cross-team coordination, and communications exercises.

### Assurance, Auditing, and Continuous Improvement
1. Quarterly assurance attestations map GDPR and DPA 2018 controls to DCC Level 2 requirements, ISO/IEC 27001 Annex A, and MOD JSP guidance. Evidence is stored in the secure SharePoint evidence register.
2. Annual independent audits assess privacy controls within the MOD enclave, covering access governance, DSR management, DPIA quality, and incident readiness. Findings feed into the CAPA register with MOD oversight.
3. Continuous monitoring dashboards provide the SIRO and MOD authority with metrics on DSR volume, DPIA status, control effectiveness, and breach response performance.

### Training and Personnel Security
1. All personnel handling MOD personal data must complete DCPP-approved privacy and security training before access and annually thereafter, covering GDPR principles, DEF STAN 05-138, JSP 440, and MOD-specific breach response.
2. Personnel must hold current BPSS (or higher) clearance. Lapses result in immediate suspension of access pending revalidation.
3. Subcontractor onboarding includes verification of training records, clearance levels, and signed MOD confidentiality undertakings.

## Technical Controls (DCC Augmentation)
1. SIEM correlation rules detect anomalous access, exfiltration attempts, and privilege escalation within MOD workloads. Alerts are triaged within 15 minutes.
2. Data Loss Prevention policies tailored for MOD protective markings prevent unauthorised sharing to unmanaged endpoints, personal email, or unauthorised cloud storage.
3. Secure destruction of MOD media follows NCSC IA Standard No.5 and is documented with certificates of destruction endorsed by the SIRO.

## Roles and Responsibilities
1. **Senior Information Risk Owner (Director):** Owns MOD privacy risk posture, approves DPIAs, and ensures alignment with MOD policies and DCC Level 2 controls.
2. **Defence Cyber Compliance Lead:** Coordinates assurance activities, maintains the control evidence matrix, and liaises with the SAC on privacy matters.
3. **Data Protection Officer:** Interfaces with the ICO and MOD DPO, manages DSRs, maintains records, and ensures lawful basis documentation.
4. **Employees and Subcontractors:** Comply with handling rules, report incidents immediately, and maintain mandatory clearances and training.
5. **Suppliers / Processors:** Provide MOD-compliant security attestations, support audits, and notify Cyber Ask Ltd of incidents within two hours.

## Accountable Roles and Decision Authority
1. **Executive Leadership Team:** Approves this DCC policy, resource allocations, and risk treatment plans affecting MOD engagements.
2. **SIRO (Director):** Authorises residual risk acceptance, international transfers, and subcontractor onboarding for MOD data processing.
3. **MOD Authority / SAC:** Provides final approval for processing changes, transfer requests, and closure of CAPA actions related to privacy controls.

## Compliance
Non-compliance with this policy may result in MOD contractual sanctions, financial penalties, suspension from DCC frameworks, and regulatory action by the ICO. Personnel violations may lead to disciplinary measures or removal from MOD projects.

## Review
This policy is reviewed bi-annually, following significant changes to MOD security directives, DCC Level 2 guidance, or data protection legislation. Interim reviews occur after material incidents or MOD audit findings.

## Revision History (DCC Version)
| Version | Date       | Description | Author |
| ------- | ---------- | ----------- | ------ |
| 1.0-DCC | 2025-10-06 | Initial DCC-aligned GDPR and UK DPA policy issued to cover MOD privacy obligations. | Defence Cyber Compliance Lead |
