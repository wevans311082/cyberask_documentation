# Multi-Factor Authentication (MFA) Policy

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

This policy establishes requirements for multi-factor authentication (mfa) to protect organizational assets and ensure compliance with applicable laws and regulations.

## Scope

This policy applies to all employees, contractors, and third parties who access or manage company resources related to multi-factor authentication (mfa).

## Policy
1. The organization shall define and document procedures for multi-factor authentication (MFA).
2. Microsoft Entra ID (Azure AD) shall be the primary MFA provider for all Microsoft 365 and integrated services, enforcing conditional access policies.
3. Controls for multi-factor authentication (MFA) must align with industry best practices and regulatory obligations.
4. Activities related to multi-factor authentication (MFA) shall be reviewed and updated regularly to address emerging risks.
5. Records demonstrating compliance with this policy shall be maintained.

1. All aspects of Multi Factor Authentication Mfa Policy must align with ISO/IEC 27001:2022 controls and the NCSC Cyber Assessment Framework.
2. Procedures shall be documented, communicated, and reviewed at least annually by the Director.
3. Staff and contractors must receive training on Multi Factor Authentication Mfa Policy before being granted related responsibilities.
4. Access and activities associated with Multi Factor Authentication Mfa Policy shall be logged and monitored to detect and respond to unauthorised actions.
5. Deviations from this policy must be reported within 24 hours and remedied within 30 days.
6. Technology configurations supporting Multi Factor Authentication Mfa Policy must follow relevant CIS Benchmarks and vendor hardening guides.
7. Third parties engaged in Multi Factor Authentication Mfa Policy processes shall have contractual obligations to meet equivalent security standards.
8. Records demonstrating compliance with this policy shall be retained for audit for a minimum of six years.
9. The Director must approve exceptions in writing, including scope, duration, and compensating controls.
10. Failure to comply with this policy may result in disciplinary action, removal of access, or termination of contract.

1. Systems processing Multi Factor Authentication Mfa Policy shall enforce least privilege and role-based access controls.
2. Changes affecting Multi Factor Authentication Mfa Policy configurations must follow the Change Management Policy and receive formal approval.
3. Monitoring tools shall generate alerts for Multi Factor Authentication Mfa Policy violations and designated staff must review these alerts daily.
4. Internal audits shall verify adherence to Multi Factor Authentication Mfa Policy at least annually and report findings to senior management.
5. Data associated with Multi Factor Authentication Mfa Policy must be protected in accordance with GDPR and UK statutory requirements.
6. Users shall acknowledge and accept this policy annually to retain relevant access rights.

## Technical Controls

1. Configure and maintain systems to enforce the requirements of the Multi-Factor Authentication (MFA) Policy, using appropriate tools and automation.
2. Enable logging, monitoring, and alerting to detect and respond to deviations from the Multi-Factor Authentication (MFA) Policy.
3. Apply encryption, access controls, and regular audits to ensure compliance with this policy.
4. Enforce MFA for all users accessing Microsoft 365 using methods such as Microsoft Authenticator, FIDO2 security keys, or certificate-based authentication.
5. Configure Conditional Access in Microsoft Entra ID to require compliant devices and block legacy authentication.
6. Monitor MFA events through Microsoft 365 audit logs and integrate alerts with centralized monitoring tools.

## Roles and Responsibilities

1. **Employees and Contractors:** Follow multi-factor authentication (mfa) procedures and report issues or non-compliance.
2. **Management:** Provide resources and enforce this policy within their areas of responsibility.
3. **Security and Compliance Teams:** Monitor multi-factor authentication (mfa) controls, provide guidance, and coordinate improvements.

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

## Modern Authentication Mandates

To support the enterprise shift away from passwords, MFA is mandatory for every user and service that interacts with company resources. The following practices are enforced:

- SMS OTP, voice calls, email verification codes, and other single-channel factors are prohibited. Phishing-resistant factors such as FIDO2 hardware keys, platform authenticators, or certificate-based smart cards are the only approved methods.
- Push-based authenticators must implement number matching and device binding to defeat MFA fatigue attacks.
- Legacy protocols (IMAP/POP/SMTP basic auth) are blocked at the tenant level unless an exception is approved by the Director with compensating controls and a sunset date.

## Adoption Roadmap

The MFA rollout is tracked via quarterly milestones to ensure enterprise-wide coverage by Q4 2025.

| Quarter | Target Milestone | Coverage Goal | Key Activities |
| --- | --- | --- | --- |
| Q1 2025 | Pilot passwordless-capable MFA for privileged users. | 30% of workforce enrolled in FIDO2 keys. | Distribute hardware keys, update conditional access policies, deliver administrator training. |
| Q2 2025 | Extend phishing-resistant MFA to all core applications. | 65% of workforce using hardware or platform authenticators. | Integrate third-party SaaS via SAML/OIDC, retire legacy OTP methods, monitor adoption metrics. |
| Q3 2025 | Enforce MFA on service accounts and automation workflows. | 85% coverage including non-interactive accounts. | Implement managed identities, rotate secrets, and transition scripts to certificate-based auth. |
| Q4 2025 | Achieve universal phishing-resistant MFA adoption. | 100% workforce coverage with passwordless sign-in for daily workflows. | Decommission password-only login paths, validate recovery procedures, and perform independent assurance review. |

Progress is reported monthly to the Director, with blockers recorded in the risk register and resolved before the next milestone.

## Control Assurance and Auditing

- Continuous monitoring dashboards track MFA success/failure rates, unusual prompt frequency, and impossible travel events. Alerts feed into the SIEM for investigation.
- Semi-annual configuration reviews verify that conditional access policies enforce compliant devices, block legacy authentication, and align with the Zero Trust Security Policy.
- Third-party attestations are obtained from managed service providers to confirm MFA enforcement on shared platforms.

## Training and Support

Training includes live demonstrations on registering FIDO2 devices, recovery using administrative unlock codes, and recognising MFA push bombing. A just-in-time knowledge base article is provided when users enrol new devices. The helpdesk maintains secure break-glass accounts protected by hardware tokens and audited monthly.

## Integration with Complementary Policies

This policy must be applied in tandem with the [Password and Authentication Policy](./password-and-authentication-policy.md) and the [Passwordless Authentication Policy](./passwordless-authentication-policy.md). Together they establish a unified authentication standard that supports zero-trust principles and regulatory expectations.

