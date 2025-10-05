# Data Loss Prevention (DLP) Policy

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

This policy establishes requirements for data loss prevention (dlp) to protect organizational assets and ensure compliance with applicable laws and regulations.

## Scope

This policy applies to all employees, contractors, and third parties who access or manage company resources related to data loss prevention (dlp).

## Policy
1. The organisation shall define and document procedures for data loss prevention (DLP), including tooling configuration, event handling, and exception management.
2. DLP controls must align with industry best practices, contractual commitments, and regulatory obligations (e.g., UK GDPR Articles 32–34, client security schedules).
3. Activities related to DLP shall be reviewed quarterly to address emerging risks, data handling changes, or lessons learned from incidents.
4. Records demonstrating compliance with this policy—including policy configuration exports, incident tickets, and review minutes—shall be maintained for at least six years.
5. DLP metrics (blocked events, overrides, false positives) must be reported to the Director monthly and fed into management review meetings.

## Procedures and Tooling

### Microsoft Purview Configuration

1. Classify data using sensitivity labels mapped to the Data Classification and Handling Policy.  
2. Implement Exchange Online, SharePoint, OneDrive, and Teams DLP policies with rules for Restricted and Confidential data.  
3. Enable endpoint DLP for managed Windows devices to monitor USB, printing, and clipboard actions.  
4. Configure policy tips to educate users before enforcing blocking actions.  
5. Review and test DLP policies in audit mode before moving to enforcement.

### False Positive Reduction

1. Apply document fingerprinting for approved templates to improve detection accuracy.  
2. Exclude trusted domains and service accounts documented in supplier agreements.  
3. Utilise adaptive scopes (e.g., high-risk departments) to focus blocking controls where they deliver greatest value.  
4. Conduct monthly tuning sessions analysing incident logs to adjust thresholds and rule conditions.  
5. Provide feedback loops with users via the DLP override justification form to refine business rules.

### Incident Response Integration

1. DLP alerts feed into the incident management workflow; high severity alerts trigger the incident response plan.  
2. All overrides require justification and manager approval within two working days.  
3. Repeat offenders are referred for additional training or disciplinary action in line with the Disciplinary Policy.

## GDPR Alignment

1. Document lawful processing purposes for monitored data and communicate monitoring practices in privacy notices.  
2. Ensure DLP logging complies with data minimisation principles; limit retention to 12 months unless legal proceedings require longer.  
3. Support data subject rights by enabling extraction of monitoring data relevant to subject access requests.  
4. Notify the Director within one hour of any DLP event indicating potential personal data breach to ensure 72-hour supervisory authority reporting can be met.  
5. Record DPIA outcomes for DLP deployments and review annually.

1. All aspects of Data Loss Prevention Dlp Policy must align with ISO/IEC 27001:2022 controls and the NCSC Cyber Assessment Framework.
2. Procedures shall be documented, communicated, and reviewed at least annually by the Director.
3. Staff and contractors must receive training on Data Loss Prevention Dlp Policy before being granted related responsibilities.
4. Access and activities associated with Data Loss Prevention Dlp Policy shall be logged and monitored to detect and respond to unauthorised actions.
5. Deviations from this policy must be reported within 24 hours and remedied within 30 days.
6. Technology configurations supporting Data Loss Prevention Dlp Policy must follow relevant CIS Benchmarks and vendor hardening guides.
7. Third parties engaged in Data Loss Prevention Dlp Policy processes shall have contractual obligations to meet equivalent security standards.
8. Records demonstrating compliance with this policy shall be retained for audit for a minimum of six years.
9. The Director must approve exceptions in writing, including scope, duration, and compensating controls.
10. Failure to comply with this policy may result in disciplinary action, removal of access, or termination of contract.

1. Systems processing Data Loss Prevention Dlp Policy shall enforce least privilege and role-based access controls.
2. Changes affecting Data Loss Prevention Dlp Policy configurations must follow the Change Management Policy and receive formal approval.
3. Monitoring tools shall generate alerts for Data Loss Prevention Dlp Policy violations and designated staff must review these alerts daily.
4. Internal audits shall verify adherence to Data Loss Prevention Dlp Policy at least annually and report findings to senior management.
5. Data associated with Data Loss Prevention Dlp Policy must be protected in accordance with GDPR and UK statutory requirements.
6. Users shall acknowledge and accept this policy annually to retain relevant access rights.

## Technical Controls

1. Configure and maintain systems to enforce the requirements of the Data Loss Prevention (DLP) Policy, using appropriate tools and automation.
2. Enable logging, monitoring, and alerting to detect and respond to deviations from the Data Loss Prevention (DLP) Policy.
3. Apply encryption, access controls, and regular audits to ensure compliance with this policy.

## Roles and Responsibilities

1. **Employees and Contractors:** Follow data loss prevention (dlp) procedures and report issues or non-compliance.
2. **Management:** Provide resources and enforce this policy within their areas of responsibility.
3. **Security and Compliance Teams:** Monitor data loss prevention (dlp) controls, provide guidance, and coordinate improvements.

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
