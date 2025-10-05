# Passwordless Authentication Policy

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

This policy establishes requirements for passwordless authentication to protect organizational assets and ensure compliance with applicable laws and regulations.

## Scope

This policy applies to all employees, contractors, and third parties who access or manage company resources related to passwordless authentication.

## Policy
1. The organization shall define and document procedures for passwordless authentication.
2. Controls for passwordless authentication must align with industry best practices and regulatory obligations.
3. Activities related to passwordless authentication shall be reviewed and updated regularly to address emerging risks.
4. Records demonstrating compliance with this policy shall be maintained.

1. All aspects of Passwordless Authentication Policy must align with ISO/IEC 27001:2022 controls and the NCSC Cyber Assessment Framework.
2. Procedures shall be documented, communicated, and reviewed at least annually by the Director.
3. Staff and contractors must receive training on Passwordless Authentication Policy before being granted related responsibilities.
4. Access and activities associated with Passwordless Authentication Policy shall be logged and monitored to detect and respond to unauthorised actions.
5. Deviations from this policy must be reported within 24 hours and remedied within 30 days.
6. Technology configurations supporting Passwordless Authentication Policy must follow relevant CIS Benchmarks and vendor hardening guides.
7. Third parties engaged in Passwordless Authentication Policy processes shall have contractual obligations to meet equivalent security standards.
8. Records demonstrating compliance with this policy shall be retained for audit for a minimum of six years.
9. The Director must approve exceptions in writing, including scope, duration, and compensating controls.
10. Failure to comply with this policy may result in disciplinary action, removal of access, or termination of contract.

1. Systems processing Passwordless Authentication Policy shall enforce least privilege and role-based access controls.
2. Changes affecting Passwordless Authentication Policy configurations must follow the Change Management Policy and receive formal approval.
3. Monitoring tools shall generate alerts for Passwordless Authentication Policy violations and designated staff must review these alerts daily.
4. Internal audits shall verify adherence to Passwordless Authentication Policy at least annually and report findings to senior management.
5. Data associated with Passwordless Authentication Policy must be protected in accordance with GDPR and UK statutory requirements.
6. Users shall acknowledge and accept this policy annually to retain relevant access rights.

## Technical Controls

1. Configure and maintain systems to enforce the requirements of the Passwordless Authentication Policy, using appropriate tools and automation.
2. Enable logging, monitoring, and alerting to detect and respond to deviations from the Passwordless Authentication Policy.
3. Apply encryption, access controls, and regular audits to ensure compliance with this policy.

## Roles and Responsibilities

1. **Employees and Contractors:** Follow passwordless authentication procedures and report issues or non-compliance.
2. **Management:** Provide resources and enforce this policy within their areas of responsibility.
3. **Security and Compliance Teams:** Monitor passwordless authentication controls, provide guidance, and coordinate improvements.

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

## Passwordless Principles

The organisation adopts passwordless authentication as the strategic default for all systems. Core principles include:

- Phishing-resistant authenticators (FIDO2 security keys, Windows Hello for Business, certificate-based smart cards) must be used whenever technically feasible.
- SMS OTP, email links, knowledge-based verification, and push notifications without number matching are prohibited.
- Device biometrics must be backed by hardware security modules (e.g., TPM) and configured to require secure PIN fallback for accessibility.
- Service onboarding checklists require confirmation of WebAuthn or certificate-based authentication support prior to procurement.

## FIDO2 Implementation Approach

1. **Architecture:** FIDO2 authenticators bind users to specific devices using public-key cryptography. Microsoft Entra ID provides the relying party service and integrates with Azure AD Conditional Access. Hardware keys are centrally procured, asset-tagged, and distributed with tamper-evident packaging.
2. **Registration:** Users enrol at least two authenticators (primary hardware key and backup platform authenticator) through a supervised onboarding session. Registration requires in-person identity verification or approved remote proofing.
3. **Lifecycle Management:** Lost or stolen authenticators are reported within one hour. Helpdesk staff verify identity using secure video calls and revoke keys via the identity platform. Replacement devices are issued within one business day.
4. **Integration:** Legacy applications that cannot support WebAuthn are fronted by identity-aware proxies enforcing token-based access. Exceptions must include a compensating control plan and defined retirement date.

## Benefits and Considerations

| Aspect | Benefits | Considerations |
| --- | --- | --- |
| Security | Resistant to phishing, credential stuffing, and replay attacks. | Requires physical key distribution and inventory management. |
| User Experience | Fast, seamless sign-ins with minimal friction. | Users must have access to compatible hardware and may need accessibility accommodations. |
| Compliance | Aligns with NIST SP 800-63B AAL3 and UK NCSC guidance on phishing-resistant MFA. | Auditors require evidence of key lifecycle management and tamper-proof storage. |
| Operations | Reduces password reset volume and helpdesk workload. | Contingency procedures needed for travel scenarios or shared workstations. |

## Enforcement and Auditing

- Quarterly audits confirm that 100% of active users possess at least two registered FIDO2 authenticators. Audit evidence is archived for seven years.
- Conditional Access policies enforce passwordless sign-in for all cloud services, blocking fallbacks to passwords unless a Director-approved break-glass account is used.
- Break-glass accounts are reviewed monthly and tested quarterly to ensure availability while preventing misuse.

## Training and Change Management

A structured change programme educates users on passwordless benefits, secure key handling, and incident reporting. Training assets include:

- Instructor-led onboarding sessions with live demonstrations and troubleshooting.
- E-learning modules covering secure storage, travel considerations, and reporting lost keys.
- Quick reference guides explaining how to authenticate on Windows, macOS, and mobile devices using FIDO2.

Completion of training is required before activation of passwordless profiles. Refresher sessions occur annually and after any material platform updates.

## Alignment with Related Policies

This policy is enforced alongside the [Password and Authentication Policy](./password-and-authentication-policy.md) and [Multi-Factor Authentication (MFA) Policy](./multi-factor-authentication-mfa-policy.md), ensuring a coordinated move toward passwordless operations within the broader zero-trust programme.

