# Acceptable Use Policy

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** WEvans Director

This policy defines acceptable and unacceptable uses of company information assets and technology resources in support of CE/CE+ and ISO 27001.

## Purpose

Protect company assets from misuse and maintain a secure working environment.

## Scope

Applies to all employees, contractors, and third parties using company equipment or accessing company data.

## Policy

### General Use
- Company information systems must be used only for legitimate business purposes. Limited personal use is permitted but must not interfere with duties, consume excessive resources or breach any law or company policy.
- Users shall comply with UK legislation, including the Computer Misuse Act 1990 and the Data Protection Act 2018.
- Users must lock or log off devices when unattended and keep equipment secure to prevent unauthorised access.
- Credentials must be kept secret. Passwords and multi-factor tokens must not be shared or reused across services.

### Access Control and Authentication
- Users shall only access data and systems for which they have explicit authorisation and a business need.
- Privileged accounts must not be used for day-to-day activities and shall employ multi-factor authentication.
- Remote access to company systems must occur via the approved VPN from devices that meet corporate security standards.

### Software and Device Management
- Only software approved and provisioned by the IT department may be installed. Executable code from unknown or untrusted sources must not be executed.
- Security controls such as anti-malware, endpoint detection, firewalls and automatic updates shall not be disabled or bypassed.
- Requests for new or updated software or hardware must follow the Change Management process and receive prior approval.
- Removable media must be company issued, encrypted and scanned for malware before use. Personal USB devices or unencrypted media must not be connected to company systems.

### Network and Communications
- Devices shall connect only to trusted networks. When using public networks, the company VPN must be enabled.
- Creation of ad-hoc networks, wireless hotspots or connection-sharing is prohibited without written authorisation.
- Peer-to-peer, file sharing or anonymity services must not be used unless explicitly approved for business purposes.

### Data Handling and Privacy
- Information must be classified and handled in accordance with the Data Classification Policy.
- Company data shall not be stored on or transmitted through personal email accounts, cloud storage or messaging platforms.
- Sensitive data must be encrypted in transit and at rest using approved mechanisms.

### Behaviour and Reporting
- Users must not attempt to circumvent security controls, gain unauthorised access or perform actions that could harm the organisation’s reputation or systems.
- Sending offensive material, engaging in illegal activities or introducing malicious software through company resources is strictly prohibited.
- Suspected or actual security incidents or policy breaches must be reported to the Information Security team immediately and no later than one hour after detection.

### Monitoring and Compliance
- Use of company systems may be monitored and logged for operational, compliance and security purposes. Users have no expectation of privacy when utilising company resources.
- Failure to comply with this policy may result in disciplinary action up to and including dismissal, and could lead to civil or criminal penalties.

## Monitoring

Company systems may be monitored to ensure compliance and security.

## Enforcement

Alleged breaches must be reported immediately and will be logged jointly by Information Security and HR. An investigation will
commence within one working day following the steps defined in the [Disciplinary Policy for Security Breaches](../hr/disciplinary-policy-for-security-breaches.md),
including evidence preservation, witness interviews and documented findings. Outcomes and sanctions will align with that policy
and may include corrective training, written warnings or dismissal.

Individuals have the right to appeal any disciplinary decision through the formal route set out in the
[Grievance Policy](../hr/grievance-policy.md). Appeals must be submitted in writing within the timeframe stated in the
grievance procedure and will be heard by a manager not previously involved in the case.

## Review

This policy is reviewed annually and communicated to all users upon revision.

## Implementation Guidelines
- All requests and approvals must be tracked in the ServiceDesk system.
- Data at rest must use AES-256 encryption; data in transit must use TLS 1.2+ with perfect forward secrecy.
- Security events shall log to the central SIEM and be retained for 12 months.
- Control owners perform quarterly self-assessments; Information Security conducts annual audits.
- Exceptions require written CISO approval and must include compensating controls.

## Revision History

| Version | Date | Description | Author |
| ------- | ---------- | ----------------------- | ------ |
| 2.0     | 2025-09-10 | Implementation guidelines added | Policy Team |
