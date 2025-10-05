# Password and Authentication Policy

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

This policy establishes requirements for password and authentication to protect organizational assets and ensure compliance with applicable laws and regulations.

## Scope

This policy applies to all employees, contractors, and third parties who access or manage company resources related to password and authentication.

## Policy
1. The organization shall define and document procedures for password and authentication.
2. Controls for password and authentication must align with industry best practices and regulatory obligations.
3. Activities related to password and authentication shall be reviewed and updated regularly to address emerging risks.
4. Records demonstrating compliance with this policy shall be maintained.

1. All aspects of Password And Authentication Policy must align with ISO/IEC 27001:2022 controls and the NCSC Cyber Assessment Framework.
2. Procedures shall be documented, communicated, and reviewed at least annually by the Director.
3. Staff and contractors must receive training on Password And Authentication Policy before being granted related responsibilities.
4. Access and activities associated with Password And Authentication Policy shall be logged and monitored to detect and respond to unauthorised actions.
5. Deviations from this policy must be reported within 24 hours and remedied within 30 days.
6. Technology configurations supporting Password And Authentication Policy must follow relevant CIS Benchmarks and vendor hardening guides.
7. Third parties engaged in Password And Authentication Policy processes shall have contractual obligations to meet equivalent security standards.
8. Records demonstrating compliance with this policy shall be retained for audit for a minimum of six years.
9. The Director must approve exceptions in writing, including scope, duration, and compensating controls.
10. Failure to comply with this policy may result in disciplinary action, removal of access, or termination of contract.

1. Systems processing Password And Authentication Policy shall enforce least privilege and role-based access controls.
2. Changes affecting Password And Authentication Policy configurations must follow the Change Management Policy and receive formal approval.
3. Monitoring tools shall generate alerts for Password And Authentication Policy violations and designated staff must review these alerts daily.
4. Internal audits shall verify adherence to Password And Authentication Policy at least annually and report findings to senior management.
5. Data associated with Password And Authentication Policy must be protected in accordance with GDPR and UK statutory requirements.
6. Users shall acknowledge and accept this policy annually to retain relevant access rights.

## Technical Controls

1. Configure and maintain systems to enforce the requirements of the Password and Authentication Policy, using appropriate tools and automation.
2. Enable logging, monitoring, and alerting to detect and respond to deviations from the Password and Authentication Policy.
3. Apply encryption, access controls, and regular audits to ensure compliance with this policy.

## Roles and Responsibilities

1. **Employees and Contractors:** Follow password and authentication procedures and report issues or non-compliance.
2. **Management:** Provide resources and enforce this policy within their areas of responsibility.
3. **Security and Compliance Teams:** Monitor password and authentication controls, provide guidance, and coordinate improvements.

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

## Strategic Direction: Phasing Out Passwords

Cyber Ask Ltd is transitioning to passwordless authentication as the default method for all corporate services by the end of 2025. Passwords remain as a temporary fallback for legacy systems only when compensating controls are in place. The following mandates apply across the estate:

- Passwords must never be shared or stored in unsecured locations; credential managers approved by the Director are mandatory for any residual password use.
- Weak or deprecated authentication factors, including SMS one-time passwords (OTP), voice calls, and email-based codes, are prohibited due to susceptibility to SIM swap and phishing attacks.
- Hardware-backed phishing-resistant methods (FIDO2 security keys, Windows Hello for Business, certificate-based smart cards) are required for privileged accounts effective immediately.
- Any new system procurement must evidence support for passwordless protocols (FIDO2/WebAuthn, certificate auth) before approval.

## Interim Password Requirements

Where passwords cannot yet be eliminated, the following controls ensure resilience during the transition:

1. **Complexity and Length:** Minimum length of 14 characters with passphrase guidance, though complexity requirements are relaxed to support usability.
2. **Credential Rotation:** Password changes are event-driven (suspected compromise or policy exception). Routine forced rotations are discouraged to maintain usability and align with NIST SP 800-63B.
3. **Breach Monitoring:** Passwords are screened against known compromised credential databases using automated tooling. Detections trigger immediate resets and security investigations.
4. **System Isolation:** Legacy password-dependent services must reside behind secure gateways enforcing conditional access and continuous monitoring.

## Enforcement and Assurance

- Quarterly authentication audits verify that no accounts rely on SMS OTP or basic push approvals. Findings are documented in the compliance tracker and remediated within 15 days.
- The Director reviews authentication logs monthly to ensure MFA fatigue attacks are mitigated by number matching and device-binding policies.
- Annual penetration tests include social engineering scenarios to validate resistance to credential phishing.

## Training and Awareness

Cyber Ask University provides micro-learning modules on phishing-resistant authentication, secure use of hardware tokens, and incident reporting. Completion is mandatory prior to issuance of security keys and refreshed annually. Supplementary job aids demonstrate how to register FIDO2 devices and recover accounts through secure administrator-assisted processes.

## Dependencies and Related Policies

This policy operates alongside the [Multi-Factor Authentication (MFA) Policy](./multi-factor-authentication-mfa-policy.md) and the [Passwordless Authentication Policy](./passwordless-authentication-policy.md). All three documents form the cohesive authentication control framework guiding the passwordless transition.

