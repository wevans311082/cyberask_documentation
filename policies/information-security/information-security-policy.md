# Information Security Policy

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** Wayne Evans (Director)

This policy defines the organization's overall approach to managing information security risks and maintaining compliance with CE/CE+ and ISO 27001.

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

Protect the confidentiality, integrity, and availability of information assets by establishing governance and control objectives.

## Scope

Applies to all employees, contractors, and third parties who access company information.

## Policy
1. The organisation shall maintain an Information Security Management System aligned to ISO/IEC 27001:2022 and the NCSC Cyber Assessment Framework.
2. Information assets must be inventoried and classified, and handling shall follow the Data Classification and Handling Policy.
3. Access to company systems and data shall be authorised, logged and limited to the minimum necessary; privileged access shall be reviewed quarterly.
4. Multi-factor authentication must be used for remote, administrative and cloud services; default passwords and accounts shall be disabled or changed before deployment.
5. Security patches and configuration baselines shall be applied in accordance with the Patch and Vulnerability Management Policy and relevant CIS Benchmarks; unsupported software must not be used.
6. Logging and monitoring controls shall be enabled on all production systems and log data retained for a minimum of 12 months to support audit and incident investigation.
7. Backups of critical information must be taken daily, encrypted, and tested at least quarterly.
8. Users shall only use company-approved devices and services; personal storage solutions or unauthorised software are prohibited.
9. Actual or suspected security incidents, weaknesses or policy breaches must be reported to the Director immediately via the incident reporting procedure.
10. Compliance with this policy is mandatory. Breaches may result in disciplinary action and where appropriate, legal or contractual penalties.

1. All aspects of Information Security Policy must align with ISO/IEC 27001:2022 controls and the NCSC Cyber Assessment Framework.
2. Procedures shall be documented, communicated, and reviewed at least annually by the Director.
3. Staff and contractors must receive training on Information Security Policy before being granted related responsibilities.
4. Access and activities associated with Information Security Policy shall be logged and monitored to detect and respond to unauthorised actions.
5. Deviations from this policy must be reported within 24 hours and remedied within 30 days.
6. Technology configurations supporting Information Security Policy must follow relevant CIS Benchmarks and vendor hardening guides.
7. Third parties engaged in Information Security Policy processes shall have contractual obligations to meet equivalent security standards.
8. Records demonstrating compliance with this policy shall be retained for audit for a minimum of six years.
9. The Director must approve exceptions in writing, including scope, duration, and compensating controls.
10. Failure to comply with this policy may result in disciplinary action, removal of access, or termination of contract.

1. Systems processing Information Security Policy shall enforce least privilege and role-based access controls.
2. Changes affecting Information Security Policy configurations must follow the Change Management Policy and receive formal approval.
3. Monitoring tools shall generate alerts for Information Security Policy violations and designated staff must review these alerts daily.
4. Internal audits shall verify adherence to Information Security Policy at least annually and report findings to senior management.
5. Data associated with Information Security Policy must be protected in accordance with GDPR and UK statutory requirements.
6. Users shall acknowledge and accept this policy annually to retain relevant access rights.

## Governance

1. Senior management endorses the ISMS and allocates resources for implementation.
2. An Director (ISO) oversees policy development, risk management, and compliance.
3. Security objectives are established, measured, and reviewed at least annually.

## Risk Management

1. Conduct formal risk assessments using the approved methodology.
2. Implement controls based on the Statement of Applicability and risk treatment plan.
3. Monitor risks and update assessments after major changes or incidents.

## Accountable Roles and Decision Authority

1. **Director:** Owns and maintains this policy, coordinates updates, and ensures alignment with the Cyber Governance Policy and Document Control Policy.
2. **Director (Risk Owner):** Reviews and approves exceptions, risk acceptances, and material control changes, documenting rationale in line with the Risk Management Policy.
3. **Director (Service Owner):** Oversees day-to-day execution of this policy, vendor engagement, and customer communications when actions affect external parties.


## Compliance

1. All legal, regulatory, and contractual obligations must be identified and met.
2. Noncompliance may result in disciplinary action and contractual penalties.

## Awareness and Training

1. Employees receive security awareness training upon hire and annually thereafter.
2. Specialized training is provided based on role requirements.

## Review

This policy is reviewed annually by management and updated as needed to address emerging threats and business changes.

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
