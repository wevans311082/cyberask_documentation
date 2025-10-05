# Supplier Security Policy (DCC Version)

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** WEvans Director  
**Classification:** OFFICIAL-SENSITIVE when completed

## Purpose

This Defence Cyber Compliance (DCC) aligned policy defines supplier security expectations for Ministry of Defence (MOD) delivery and support contracts. It establishes assurance tiers, onboarding and vetting controls, contractual flow-down clauses, and continuous monitoring obligations required to protect MOD information and services throughout the supply chain.

## Scope

This policy applies to:
- All Cyber Ask Ltd staff managing MOD contracts and supplier relationships.
- Direct suppliers, subcontractors, and service partners engaged on MOD-funded or MOD-owned deliverables.
- Any external party that stores, processes, transmits, transports, or disposes of MOD protectively marked assets on behalf of Cyber Ask Ltd.

## Policy Requirements

### Supplier Assurance Tiers and DCC Profiles

Suppliers shall be risk assessed using the MOD Defence Cyber Compliance profiles and assigned an assurance tier that drives onboarding, contractual, and monitoring requirements.

| DCC Profile | Typical Contract Drivers | Supplier Assurance Tier | Minimum Assurance Requirements |
|-------------|-------------------------|-------------------------|--------------------------------|
| Profile 1 – Baseline | Non-complex services handling OFFICIAL data only | Tier 1 | Signed security charter, Cyber Essentials (or equivalent) certification, completion of MOD baseline questionnaire, adherence to Cyber Ask secure onboarding pack. |
| Profile 2 – Enhanced | Managed services or systems with limited personal/sensitive MOD data | Tier 2 | Evidence of Cyber Essentials Plus, documented secure development practices, annual self-assessment against DEF STAN 05-138 controls, onboarding interview covering secure logistics handling, 12-month corrective action plan tracking. |
| Profile 3 – Substantial | Systems integration, classified design information, remote administrative access | Tier 3 | External audit against DEF STAN 05-138 Annex A, Security-As-Delivered plan, protective marking handling procedures, annual site visit by Cyber Ask security, continuous vulnerability scanning with results shared quarterly. |
| Profile 4 – Critical | Mission or safety critical systems, SECRET or higher | Tier 4 | Joint MOD/Cyber Ask accreditation, Security Assurance Case approved by Accreditor, NIST SP 800-171 implementation evidence (or SP 800-172 for enhanced controls), dedicated security officer, near-real-time monitoring feeds to Cyber Ask SOC, participation in MOD Cyber Protection Partnership reviews. |

Assurance tiers shall be reviewed when scope changes, new data classifications are introduced, or on an annual cadence, whichever occurs first.

### Onboarding, Personnel Vetting, and Access Provisioning

1. Suppliers must not be activated in procurement systems until onboarding tasks defined for their assurance tier are completed and approved by the Information Security Manager.
2. Personnel vetting shall be commensurate with the highest protective marking of information to be accessed:
   - Tier 1: Baseline Personnel Security Standard (BPSS) verification with confirmation retained by the Contract Manager.
   - Tier 2: BPSS plus Security Check (SC) where MOD data includes personal or sensitive operational details; onboarding must validate SC currency via UKSV.
   - Tier 3: SC minimum; Developed Vetting (DV) for roles with routine SECRET or compartmented data access.
   - Tier 4: DV or higher-level national caveat clearances as mandated by MOD Accreditor.
3. Suppliers shall provide named security points of contact and maintain joiner/mover/leaver logs. Access revocations must occur within four hours of notification for Tier 3 and Tier 4 suppliers.
4. All supplier staff shall complete MOD-mandated security awareness (e.g., DSPCR regulation brief, JSP 440 modules) prior to system access.

### Continuous Monitoring and Assurance

1. Contract Managers shall maintain a Supplier Assurance Plan (SAP) aligned with DEF STAN 05-138 Annex B, documenting planned audits, evidence submissions, and remediation tracking.
2. Tier 1 suppliers must submit annual self-assessment returns. Tier 2 suppliers provide semi-annual assurance statements and quarterly vulnerability status.
3. Tier 3 and Tier 4 suppliers shall provide continuous monitoring data feeds, including:
   - Monthly security KPI dashboards (patch status, incident metrics, privileged access reviews).
   - Quarterly penetration test or red team summaries for in-scope services.
   - Notification of configuration drift or control exceptions within five business days.
4. Cyber Ask SOC shall integrate supplier-provided telemetry into joint threat detection where technically feasible.

### Contractual Flow-Down Requirements

1. Contracts with suppliers must include applicable MOD contractual clauses, including but not limited to DEFCON 658 (Cyber), DEFCON 659A (Security Requirements for Information Technology), DEFCON 565 (MOD-Owned Equipment), DEFCON 660 (Security Measures), and DEFCON 76 (Contractors on Deployed Operations).
2. Where the Defence and Security Public Contracts Regulations (DSPCR) 2011 apply, suppliers shall accept flow-down of MOD security obligations, export controls, protective marking handling, and incident reporting requirements.
3. Subcontracts shall include equivalent clauses ensuring lower-tier suppliers meet the same standards; Contract Managers must evidence flow-down in contract files.

### Incident Reporting and Escalation

1. Suppliers shall report suspected or confirmed security incidents affecting MOD data, services, or systems to Cyber Ask within one hour of discovery and to the MOD Defence Cyber Protection Partnership (DCPP) portal within 12 hours, unless otherwise directed by contract.
2. Incident reports must include protective marking, impact assessment, initial containment actions, and preliminary timeline.
3. High-severity incidents (impacting SECRET or operational availability) require immediate telephone escalation to the MOD Authority and Cyber Ask CISO.
4. Suppliers shall cooperate with joint investigations, provide forensic images when requested, and maintain evidence in accordance with JSP 440 and JSP 604 guidelines.

### Assurance Evidence (DEF STAN 05-138 Alignment)

Suppliers shall maintain evidence artefacts consistent with DEF STAN 05-138, including:
- Completed Supplier Assurance Questionnaire and Cyber Implementation Plan with agreed risk profile.
- Statement of Compliance matrix mapping controls to supplier policies and procedures.
- Records of risk treatment plans, security testing reports, and remediation closure evidence.
- Audit reports, certifications (Cyber Essentials Plus, ISO/IEC 27001, NIST SP 800-171 System Security Plans), and supplier assurance dashboards.
- Logistics traceability logs covering chain-of-custody for protectively marked assets and hardware.

### Secure Logistics and Protective Marking Handling

1. Suppliers transporting MOD assets shall use MOD-approved carriers, tamper-evident packaging, and maintain chain-of-custody records for the life of the shipment.
2. Protective markings (OFFICIAL-SENSITIVE, SECRET, NATO RESTRICTED, etc.) must be applied, stored, transmitted, and destroyed per JSP 440 and MOD contract instructions.
3. Tier 3 and Tier 4 suppliers shall implement dual-control for movement of SECRET or higher material and validate that storage facilities meet MOD Physical Security Standards (e.g., SAPC, Class 2 containers).
4. Disposal of MOD media shall follow CESG (NCSC) approved destruction methods with certificates of destruction provided to Cyber Ask within five business days.

### Standards and External Compliance Expectations

1. All suppliers must comply with applicable UK law, MOD policy (JSP 440, JSP 604, JSP 745), and this policy.
2. Suppliers handling US Department of Defense Controlled Unclassified Information (CUI) under MOD-DoD collaborative programmes shall implement and maintain controls equivalent to NIST SP 800-171, with NIST SP 800-172 enhanced controls required where specified by contract or data owner.
3. Suppliers shall inform Cyber Ask of any control gaps against NIST SP 800-171/172 within 30 days of identification and provide a Plan of Actions and Milestones (POA&M) for remediation.
4. International suppliers must demonstrate compliance with relevant export control regimes and cross-border data handling agreements before accessing MOD data.

## Roles and Responsibilities

- **Information Security Manager:** Owns supplier assurance framework, approves onboarding, and ensures DEF STAN 05-138 alignment.
- **Contract Manager:** Maintains Supplier Assurance Plans, confirms contractual flow-down clauses, and monitors compliance evidence.
- **Security Operations Centre (SOC):** Integrates supplier telemetry, monitors incidents, and coordinates response activities.
- **Supplier Security Point of Contact:** Ensures supplier personnel vetting, manages joiner/mover/leaver processes, and reports incidents.
- **Executive Leadership Team:** Provides oversight, resources, and governance for MOD supply chain security obligations.

## Compliance and Exceptions

Failure to comply with this policy may result in suspension of supplier access, contract termination, and notification to the MOD Authority. Exceptions require written approval from the CISO, endorsement by the MOD Accreditor where mandated, and documented compensating controls.

## Review

This policy shall be reviewed at least annually or upon significant change to MOD or DEF STAN 05-138 requirements, ensuring continuous alignment with DCC guidance and contractual obligations.

## Revision History

| Version | Date | Description | Author |
| ------- | ---------- | ------------ | ------ |
| 1.0 | 2024-07-01 | Initial DCC-aligned supplier security policy issued. | Policy Team |
| 1.1 | 2025-09-10 | Updated assurance tiers, MOD onboarding, DEFCON flow-down, incident reporting, NIST SP 800-171/172 alignment, and secure logistics guidance. | Policy Team |
