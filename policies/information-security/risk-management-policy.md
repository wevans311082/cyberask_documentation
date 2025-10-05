# Risk Management Policy

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** WEvans Director

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

This policy establishes requirements for risk management to protect organizational assets and ensure compliance with applicable laws and regulations.

## Scope

This policy applies to all employees, contractors, and third parties who access or manage company resources related to risk management.

## Policy
1. The organization shall define and document procedures for risk management.
2. Controls for risk management must align with industry best practices and regulatory obligations.
3. Activities related to risk management shall be reviewed and updated regularly to address emerging risks.
4. Records demonstrating compliance with this policy shall be maintained.
5. A master risk register, risk treatment plan, and supporting risk assessments shall be maintained in the "Risk Assessments" repository folder with version control and access limited to authorised personnel.
6. Risk treatment progress shall be monitored monthly and reported through the security metrics pack alongside evidence of control effectiveness.

1. All aspects of Risk Management Policy must align with ISO/IEC 27001:2022 controls and the NCSC Cyber Assessment Framework.
2. Procedures shall be documented, communicated, and reviewed at least annually by the Director.
3. Staff and contractors must receive training on Risk Management Policy before being granted related responsibilities.
4. Access and activities associated with Risk Management Policy shall be logged and monitored to detect and respond to unauthorised actions.
5. Deviations from this policy must be reported within 24 hours and remedied within 30 days.
6. Technology configurations supporting Risk Management Policy must follow relevant CIS Benchmarks and vendor hardening guides.
7. Third parties engaged in Risk Management Policy processes shall have contractual obligations to meet equivalent security standards.
8. Records demonstrating compliance with this policy shall be retained for audit for a minimum of six years.
9. The Director must approve exceptions in writing, including scope, duration, and compensating controls.
10. Failure to comply with this policy may result in disciplinary action, removal of access, or termination of contract.

1. Systems processing Risk Management Policy shall enforce least privilege and role-based access controls.
2. Changes affecting Risk Management Policy configurations must follow the Change Management Policy and receive formal approval.
3. Monitoring tools shall generate alerts for Risk Management Policy violations and designated staff must review these alerts daily.
4. Internal audits shall verify adherence to Risk Management Policy at least annually and report findings to senior management.
5. Data associated with Risk Management Policy must be protected in accordance with GDPR and UK statutory requirements.
6. Users shall acknowledge and accept this policy annually to retain relevant access rights.
7. Risk decisions, approvals, and evidentiary artefacts shall be retained for a minimum of six years within the secure document repository referenced by the master risk register.

## Technical Controls

1. Configure and maintain systems to enforce the requirements of the Risk Management Policy, using appropriate tools and automation.
2. Enable logging, monitoring, and alerting to detect and respond to deviations from the Risk Management Policy.
3. Apply encryption, access controls, and regular audits to ensure compliance with this policy.

## Roles and Responsibilities

1. **Employees and Contractors:** Follow risk management procedures and report issues or non-compliance.
2. **Management:** Provide resources and enforce this policy within their areas of responsibility.
3. **Security and Compliance Teams:** Monitor risk management controls, provide guidance, and coordinate improvements.

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
6. The Director maintains the Risk Assessments folder structure (current risk assessments, master risk register, technical control roadmap, and risk treatment plan) and logs updates via the ticketing workflow defined in the Risk Treatment Plan.
7. Monthly risk review meetings confirm progress against treatment actions, update residual risk scores, and ensure alignment with ISO/IEC 27001:2022 and NCSC CAF objectives.


## Revision History

| Version | Date | Description | Author |
| ------- | ---------- | ----------------------- | ------ |
| 2.1     | 2025-02-14 | Added Risk Assessments repository requirements and monthly monitoring expectations | Director |
| 2.0     | 2025-09-10 | Implementation guidelines added | Policy Team |
