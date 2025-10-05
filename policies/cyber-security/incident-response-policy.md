# Incident Response Policy

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** Wayne Evans (Director)

## Cyber Ask Operating Context

1. Cyber Ask Ltd operates with a single employee who also serves as the sole director responsible for governance, risk, and compliance decisions.
2. Cyber Ask Ltd maintains professional liability insurance covering its consulting and advisory services.
3. A dedicated virtual machine functions as the single Windows Server domain controller and is synchronized with Microsoft Entra ID for identity management.
4. The organisation holds a standard Microsoft 365 licence; Microsoft Purview and Microsoft Defender add-ons are not deployed, and Windows Defender provides endpoint protection.
5. Customer data is stored on BitLocker-encrypted drives to protect information at rest.
6. Cyber Ask Ltd assets are vulnerability-assessed weekly and patched promptly according to remediation guidance.
7. Cyber Ask Ltd has not yet achieved Cyber Essentials, Cyber Essentials Plus, or ISO 27001 certification but aligns its controls with those standards where practicable.
8. The Director personally fulfils HR, IT administration, and compliance duties, engaging specialist suppliers when additional expertise is required.



## Purpose

This policy establishes requirements for incident response to protect organizational assets and ensure compliance with applicable laws and regulations.

## Scope

This policy applies to all employees, contractors, and third parties who access or manage company resources related to incident response.

## Policy
1. The organization shall define and document procedures for incident response.
2. Controls for incident response must align with industry best practices and regulatory obligations.
3. Activities related to incident response shall be reviewed and updated regularly to address emerging risks.
4. Records demonstrating compliance with this policy shall be maintained.

1. All aspects of Incident Response Policy must align with ISO/IEC 27001:2022 controls and the NCSC Cyber Assessment Framework.
2. Procedures shall be documented, communicated, and reviewed at least annually by the Director.
3. Staff and contractors must receive training on Incident Response Policy before being granted related responsibilities.
4. Access and activities associated with Incident Response Policy shall be logged and monitored to detect and respond to unauthorised actions.
5. Deviations from this policy must be reported within 24 hours and remedied within 30 days.
6. Technology configurations supporting Incident Response Policy must follow relevant CIS Benchmarks and vendor hardening guides.
7. Third parties engaged in Incident Response Policy processes shall have contractual obligations to meet equivalent security standards.
8. Records demonstrating compliance with this policy shall be retained for audit for a minimum of six years.
9. The Director must approve exceptions in writing, including scope, duration, and compensating controls.
10. Failure to comply with this policy may result in disciplinary action, removal of access, or termination of contract.

1. Systems processing Incident Response Policy shall enforce least privilege and role-based access controls.
2. Changes affecting Incident Response Policy configurations must follow the Change Management Policy and receive formal approval.
3. Monitoring tools shall generate alerts for Incident Response Policy violations and designated staff must review these alerts daily.
4. Internal audits shall verify adherence to Incident Response Policy at least annually and report findings to senior management.
5. Data associated with Incident Response Policy must be protected in accordance with GDPR and UK statutory requirements.
6. Users shall acknowledge and accept this policy annually to retain relevant access rights.

## Technical Controls

1. Configure and maintain systems to enforce the requirements of the Incident Response Policy, using appropriate tools and automation.
2. Enable logging, monitoring, and alerting to detect and respond to deviations from the Incident Response Policy.
3. Apply encryption, access controls, and regular audits to ensure compliance with this policy.

## Roles and Responsibilities

1. **Employees and Contractors:** Follow incident response procedures and report issues or non-compliance.
2. **Management:** Provide resources and enforce this policy within their areas of responsibility.
3. **Security and Compliance Teams:** Monitor incident response controls, provide guidance, and coordinate improvements.

## Accountable Roles and Decision Authority

1. **Director:** Owns and maintains this policy, coordinates updates, and ensures alignment with the Cyber Governance Policy and Document Control Policy.
2. **Director (Risk Owner):** Reviews and approves exceptions, risk acceptances, and material control changes, documenting rationale in line with the Risk Management Policy.
3. **Director (Service Owner):** Oversees day-to-day execution of this policy, vendor engagement, and customer communications when actions affect external parties.


## Compliance

Failure to adhere to this policy may result in disciplinary action, up to and including termination, and may expose the organization to legal or regulatory penalties.

## Review

This policy will be reviewed at least annually and updated as necessary to remain effective and compliant with relevant requirements.

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

## Incident Response Objectives and Targets

Cyber Ask Ltd commits to containing security incidents swiftly, safeguarding evidence, and restoring services within defined business recovery thresholds. The Director establishes the following objectives:

- **Recovery Time Objective (RTO):** High-severity incidents must restore critical client-facing services within four hours; medium severity incidents within 12 hours; low severity incidents within 24 hours.
- **Recovery Point Objective (RPO):** Data loss must not exceed one hour for high severity, four hours for medium, and one business day for low severity incidents.
- **Notification Commitment:** Regulatory and contractual notifications shall be issued within statutory timelines and no later than 72 hours from breach confirmation.

These targets underpin resource allocation, tabletop exercises, and investment in automation capabilities.

## Phased Response Framework

The policy adopts a six-phase lifecycle aligned with ISO/IEC 27035 and NIST SP 800-61. Each phase includes mandatory actions, decision authorities, and success criteria. Detailed procedures reside in the [Incident Response Plan](./incident-response-plan.md).

### 1. Preparation
- Maintain updated playbooks, AI-enhanced detection tooling, secure communications, and incident documentation templates.
- Conduct semi-annual resilience assessments covering backup integrity, privileged access controls, and third-party readiness.
- Ensure all responders complete annual legal, evidentiary, and technical training.

### 2. Identification
- Monitor environments with layered telemetry including SIEM, endpoint detection and response (EDR), and AI-driven anomaly detection. Integration with Microsoft Sentinel or Splunk automates correlation of behavioral indicators.
- Classify incidents using the severity matrix, referencing RTO/RPO thresholds.
- Record initial findings in the incident management platform within 30 minutes of detection.

### 3. Containment
- Apply short-term containment within 60 minutes of high-severity confirmation, such as isolating systems or enforcing firewall blocks.
- Implement long-term containment controls (patches, segmentation, credential resets) with change management oversight.
- Ensure that containment actions preserve forensic evidence and comply with chain-of-custody requirements.

### 4. Eradication
- Remove malicious artifacts, unauthorized changes, and compromised credentials.
- Validate remediation steps via vulnerability scans and integrity checks before progressing to recovery.
- Document root cause analysis, leveraging threat intelligence feeds to understand attacker tradecraft.

### 5. Recovery
- Restore services from verified clean backups, prioritizing systems based on business impact.
- Monitor for recurrence, ensuring that systems meet hardened baseline configurations prior to returning to production.
- Coordinate communications with customers and partners to confirm service restoration.

### 6. Lessons Learned
- Convene a post-incident review within ten business days of closure.
- Update policies, playbooks, and training materials based on findings.
- Track corrective actions and control improvements through the risk register until completion.

## Governance and Metrics

Incident response governance integrates with the enterprise risk management programme. The Director reviews performance metrics quarterly, including:

- Mean time to detect (MTTD) and mean time to respond (MTTR) across severity levels.
- Adherence to RTO/RPO thresholds and percentage of incidents meeting target windows.
- Number of incidents detected through AI/ML correlation as part of the 2025 detection enhancement initiative.
- Completion rate of lessons learned action items within 60 days.

Findings are reported to executive leadership alongside recommendations for tooling, staffing, or process improvements.

## Technology Enablement and 2025 Enhancements

The 2025 roadmap integrates AI-driven threat detection and automated response coordination:

- **AI-Assisted Detection:** Deploy behaviour analytics in the SIEM to highlight anomalies in user access, network flows, and cloud API usage. Models are tuned monthly using red-team simulation data.
- **Automated Playbook Orchestration:** Security orchestration, automation, and response (SOAR) workflows execute repeatable tasks such as quarantine, credential resets, and notification templating, reducing manual toil.
- **Collaborative Incident Workspace:** Cloud-based case management consolidates evidence, approvals, and communication threads, ensuring traceability for audits.

These enhancements are tested during quarterly exercises to validate interoperability with manual processes.

## Policy Linkage and Awareness

All personnel must acknowledge receipt of this policy and review the operational [Incident Response Plan](./incident-response-plan.md) before receiving access to privileged monitoring tools. The Director ensures that contractors and third-party providers are contractually obligated to follow both documents. Deviations are subject to disciplinary measures and may result in contract termination.

