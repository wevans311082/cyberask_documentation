# Information Security Policy (DCC Level 2 Alignment)

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** WEvans Director  
**Current Version:** 3.0

## Purpose

Establish and maintain an Information Security Management System (ISMS) that meets ISO/IEC 27001:2022 requirements, supports Defence Cyber Compliance (DCC) Level 2 obligations, and demonstrably aligns with applicable NIST frameworks (SP 800-53 Rev. 5, SP 800-171 Rev. 3, and the NIST Cybersecurity Framework 2.0) as well as DEF STAN 05-138.

## Scope

This policy applies to all personnel, business units, information assets, processes, and technology supporting Ministry of Defence (MOD) contracts or processing MOD Controlled or Classified information. Third parties, suppliers, and cloud providers supporting these services must adhere to equivalent controls and provide evidence of compliance with ISO/IEC 27001, NIST, DEF STAN 05-138, and DCC Level 2 control expectations.

## Policy

- Maintain an ISO/IEC 27001:2022 certified ISMS and ensure Statement of Applicability coverage for DCC Level 2, DEF STAN 05-138, and mapped NIST controls.
- Implement controls across NIST SP 800-53 and SP 800-171 families, including Access Control (AC), Audit and Accountability (AU), Configuration Management (CM), Contingency Planning (CP), Incident Response (IR), Personnel Security (PS), Physical and Environmental Protection (PE), Risk Assessment (RA), System and Communications Protection (SC), and System and Information Integrity (SI). Control owners must reference the relevant supporting policies (e.g., Access Control Policy, Incident Response Plan) and maintain auditable evidence for each family.
- Align ISMS governance and risk treatment practices to the NIST CSF functions (Identify, Protect, Detect, Respond, Recover) through linked policies and plans (e.g., Risk Management Policy, Business Continuity Management Policy, Security Operations Policy).
- Enforce Defence Cyber Protection Partnership (DCPP) and DEF STAN 05-138 control requirements, including supplier assurance, secure configuration, vulnerability management, and security incident reporting within mandated timeframes.
- Ensure monitoring, attestation, and evidence collection are documented in the ISMS evidence register, retained for a minimum of six years, and available to MOD assurance teams.
- Conduct annual integrated control testing that covers ISO/IEC 27001 Annex A, NIST SP 800-53/800-171 control families, DEF STAN 05-138 schedules, and DCC Level 2 objectives. Gaps are tracked in the Corrective and Preventive Action (CAPA) register.
- Require third parties supporting MOD contracts to submit DCPP supplier assurance statements, ISO/IEC 27001 or SOC 2 reports, and attestations of NIST control alignment at least annually.
- Report and remediate control deficiencies in accordance with the Cyber Governance Policy, Continuous Improvement Policy, and CAPA Policy.
- Maintain secure system configurations aligned with CIS Benchmarks or MOD platform hardening guides, with change approvals recorded per the Change Management Policy.
- Ensure data protection obligations under GDPR, the Official Secrets Act, and MOD contract clauses are met, including incident notification requirements.

## Governance

- The Executive Leadership Team approves this policy, confirms ISO/IEC 27001 certification scope, and receives quarterly assurance updates covering ISO, NIST, DEF STAN 05-138, and DCC Level 2 compliance status.
- The Information Security Manager (ISM) maintains the crosswalk matrix, coordinates MOD assurance engagements, and ensures integration of NIST control assessments into the ISMS risk treatment plan.
- The Risk and Compliance Committee reviews integrated control testing outcomes, risk registers, and attestation evidence. Findings impacting NIST control families or DCC Level 2 compliance are escalated to the CISO.
- Control owners must maintain lineage from policy statements to ISO Annex A controls, NIST families, DEF STAN 05-138 controls, and DCC Level 2 objectives, updating artefact registers quarterly.

## Risk Management

- Conduct risk assessments in line with the Risk Assessment Methodology, ensuring threat scenarios cover MOD supply-chain, classified information handling, and NIST CSF function outcomes.
- Document risk treatments in the Risk Treatment Plan, referencing the applicable ISO, NIST, DEF STAN, and DCC Level 2 controls selected for mitigation. Residual risks require Risk and Compliance Committee approval.

## Accountable Roles and Decision Authority

- **Chief Information Security Officer (CISO):** Approves exceptions, risk acceptances, and material control changes affecting ISO/IEC 27001, NIST, DEF STAN 05-138, or DCC Level 2 obligations.
- **Information Security Manager:** Owns this policy, manages the evidence register, and coordinates audits, attestations, and MOD assurance submissions.
- **Risk and Compliance Committee:** Oversees enterprise risk treatment, validates cross-framework control coverage, and mandates remedial actions.
- **System Owners:** Ensure systems under their control meet the mapped control requirements, maintain configuration baselines, and provide evidence during audits.

Exception requests must follow the Cyber Governance Policy, include compensating controls mapped to the affected frameworks, and be recorded in the Document Control Policy register.

## Compliance

- Compliance is monitored through internal audits, supplier assessments, and external certifications covering ISO/IEC 27001, NIST 800-171 attestation requirements, DEF STAN 05-138 clauses, and DCC Level 2 assurance statements.
- Non-compliance may result in disciplinary action, contract suspension, or MOD notification. Serious breaches must be reported to the MOD Accreditor within the required timeframe and to the ICO where applicable.
- Evidence of compliance, including risk assessments, control testing results, monitoring dashboards, audit reports, and attestation letters, must be retained for six years.

## Awareness and Training

- All staff and contractors must complete annual training covering ISO/IEC 27001 Annex A controls, NIST control families relevant to their roles, DEF STAN 05-138 requirements, and DCC Level 2 obligations.
- Specialist training (e.g., incident responders, system administrators) must include framework-specific procedures and evidence-collection techniques.

## Monitoring and Attestation

- Security monitoring is delivered through SIEM, vulnerability management, and endpoint detection systems aligned with the NIST CSF Detect function and DCC Level 2 monitoring expectations.
- Quarterly control attestations are required from control owners, confirming implementation and effectiveness across ISO/IEC 27001, NIST, DEF STAN 05-138, and DCC Level 2 controls.
- Evidence collection processes must capture screenshots, configuration exports, log samples, test results, and supplier attestations, stored in the ISMS evidence register with retention tags.

## Related Documents

- Statement of Applicability  
- Risk Management Policy  
- Risk Assessment Methodology  
- Business Continuity Management Policy  
- Security Operations Policy  
- Supplier Security Policy  
- Cyber Governance Policy  
- Document Control Policy  
- Corrective and Preventive Action (CAPA) Policy  
- Change Management Policy  
- Incident Response Plan

## Annex A: Framework Control Mapping Matrix

| ISO/IEC 27001 Annex A Domain | NIST SP 800-53 / 800-171 Control Family | NIST CSF Function | DEF STAN 05-138 Clause / Theme | DCC Level 2 Requirement | Monitoring & Assurance | Attestation & Evidence Collection |
| --- | --- | --- | --- | --- | --- | --- |
| A.5 Information Security Policies | PL (Planning), PM (Program Management) | Identify | Governance & Policy Management | Governance and Risk Management | Annual policy reviews, steering committee minutes | Signed policy approvals, ISO/IEC 27001 certificate, management review records |
| A.6 Organisation of Information Security | PM, CA (Assessment, Authorization), AT (Awareness & Training) | Identify/Protect | Organisation & Responsibilities | Roles and Responsibilities | Quarterly governance meetings, training completion dashboards | Training records, role-based access approvals, organisation charts |
| A.7 Human Resource Security | PS (Personnel Security), AT | Protect | Personnel Security & Vetting | Personnel Security | Pre-employment screening audits, onboarding checklists | Vetting evidence, HR attestations, signed NDAs |
| A.8 Asset Management | CM, MP (Media Protection), PE (Physical Protection) | Identify/Protect | Asset Control & Labelling | Asset Register Controls | CMDB monitoring, asset inventory reconciliation | Asset register extracts, media handling logs, physical access reviews |
| A.9 Access Control | AC (Access Control) | Protect | Access Control | Account Management & Privileged Access | IAM dashboards, privileged session monitoring | Access review sign-offs, MFA logs, PAM reports |
| A.10 Cryptography | SC (System & Communications Protection) | Protect | Cryptographic Controls | Encryption Controls | Key management monitoring, TLS certificate scans | Key escrow records, crypto inventory, compliance attestations |
| A.11 Physical & Environmental Security | PE | Protect | Physical Security & Environmental Controls | Physical Security Controls | CCTV checks, access badge audits | Visitor logs, environmental sensor reports, site inspection evidence |
| A.12 Operations Security | AU (Audit & Accountability), CM, SI (System & Information Integrity) | Detect | Operational Procedures & Security Monitoring | Secure Operations | SIEM alerts, vulnerability scan results | Patch reports, change records, operations runbooks |
| A.13 Communications Security | SC | Protect/Detect | Network Security & Boundary Protection | Boundary and Network Security | Network monitoring, IDS/IPS alerts | Firewall rule reviews, network diagrams, encryption attestations |
| A.14 System Acquisition, Development & Maintenance | SA (System & Services Acquisition), CM | Protect | Secure Development & Change | Secure Development Lifecycle | Secure code reviews, DevSecOps pipeline metrics | SDLC attestations, penetration test reports, change approvals |
| A.15 Supplier Relationships | SR (Supply Chain Risk Management) | Identify/Protect | Supplier Assurance & Contracting | Third Party Management | Supplier risk dashboards, contract compliance monitoring | Supplier assurance statements, security clauses, audit reports |
| A.16 Information Security Incident Management | IR (Incident Response) | Respond | Incident Reporting & Response | Incident Management | Incident response exercises, SOC runbooks | Incident tickets, post-incident reviews, MOD notifications |
| A.17 Information Security Aspects of Business Continuity | CP (Contingency Planning) | Recover | Continuity & Recovery | Business Continuity & Disaster Recovery | DR tests, backup monitoring | BCP/DR test reports, backup logs, recovery attestations |
| A.18 Compliance | RA (Risk Assessment), CA, AU | Identify/Protect/Detect | Compliance & Audit | Compliance Assurance | Internal audit schedule, compliance dashboards | Audit reports, regulatory submissions, compliance statements |

## Annex B: Evidence and Assurance Artefact Register (Excerpt)

| Artefact | Description | Frequency | Owner | Storage Location |
| --- | --- | --- | --- | --- |
| ISMS Evidence Register | Master index of ISO/NIST/DEF STAN/DCC evidence | Quarterly update | Information Security Manager | ISMS SharePoint (restricted) |
| MOD Assurance Pack | Consolidated compliance evidence for MOD audits | Annual / on request | CISO | Secure file transfer portal |
| Supplier Attestation Files | Signed supplier statements for DCPP alignment | Annual | Supplier Security Lead | Third-party risk repository |
| Control Test Reports | Results of integrated control testing | Quarterly | Compliance Analyst | GRC tool document library |
| SIEM Monitoring Dashboards | Logs and alerts evidencing monitoring coverage | Continuous | Security Operations Lead | SOC platform export |

## Review

This policy is reviewed annually or upon significant changes to ISO/IEC 27001, NIST publications, DEF STAN 05-138, or DCC Level 2 requirements.

## Revision History

| Version | Date | Description | Author |
| ------- | ---------- | ----------------------------- | ------ |
| 3.0 | 2025-09-18 | Added NIST alignment, DEF STAN & DCC Level 2 crosswalk annexes, and evidence register references | Policy Team |
| 2.0 | 2025-09-10 | Implementation guidelines added | Policy Team |

## Related Policy References

- Scope of ISMS  
- Statement of Applicability  
- MOD Contract Compliance Guidance  
- Supplier Security Policy  
- Security Operations Policy  
- Business Continuity Management Policy
