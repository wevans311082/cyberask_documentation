# Network Security Policy

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** WEvans Director

This policy defines comprehensive safeguards for protecting company networks from unauthorized access, misuse, and disruption, supporting CE/CE+ and ISO/IEC 27001 control requirements. A secure network infrastructure is essential for protecting information assets and ensuring reliable business operations.

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

Ensure the confidentiality, integrity, and availability of network services by establishing requirements for network architecture, configuration, monitoring, and incident response.

## Scope

This policy applies to all corporate networks, including wired, wireless, virtual private networks (VPNs), cloud-hosted environments, and remote connections. It covers network devices such as routers, switches, firewalls, wireless access points, and any other equipment used to transmit or process company data.

## Definitions

1. **Demilitarized Zone (DMZ):** A network segment that separates external-facing services from the internal network.
2. **Intrusion Detection/Prevention System (IDS/IPS):** Tools that monitor network traffic for malicious activity and take actions to block or alert on threats.
3. **Network Access Control (NAC):** Technology that restricts network access based on device compliance and user authentication.

## Policy Statements

1. **Perimeter Defense**
   1. Firewalls, IDS/IPS, and web application firewalls shall be deployed at network boundaries and monitored continuously.
   2. Firewall rules must follow the principle of least privilege and be reviewed quarterly.

2. **Network Segmentation and Isolation**
   1. Sensitive systems such as payment processing or HR data must reside on dedicated network segments with restricted access.
   2. VLANs and access control lists shall be used to segregate traffic between departments and environments (e.g., development, testing, production).

3. **Secure Configuration and Hardening**
   1. Default passwords on network devices must be changed prior to deployment.
   2. Unnecessary services and ports shall be disabled, and baseline configurations documented and reviewed annually.
   3. Configuration changes require approval and must be tracked through the change management process.

4. **Monitoring and Logging**
   1. Network traffic shall be logged and reviewed for suspicious activity. Logs must be retained for at least one year.
   2. Security information and event management (SIEM) tools will aggregate and analyze logs for anomalies.

5. **Remote Access**
   1. VPN connections must use strong encryption and multi-factor authentication.
   2. Split tunneling is prohibited unless explicitly approved by the Director.
   3. Remote administration of network devices must occur over secure channels (e.g., SSH, HTTPS).

6. **Wireless Networks**
   1. Corporate wireless networks shall use WPA3 or equivalent encryption and require authentication against the enterprise directory.
   2. Guest wireless access must be segmented from internal resources and require acceptance of usage terms.

7. **Network Access Control**
   1. NAC solutions will verify device compliance with security standards before granting access.
   2. Non-compliant devices may be quarantined or denied access until remediation.

8. **Change and Patch Management**
   1. Network devices must receive security patches within 30 days of release or sooner if critical vulnerabilities are identified.
   2. Firmware upgrades shall be tested in a controlled environment before deployment.

9. **Incident Response**
   1. Network anomalies suggesting a security incident must be reported to the SOC immediately.
   2. Containment actions may include blocking traffic, disabling compromised interfaces, or isolating affected segments.

10. **Encryption of Network Traffic**
    1. Sensitive data transmitted over internal or external networks must be encrypted using approved protocols such as TLS 1.2 or higher.
    2. Legacy protocols that transmit data in clear text are prohibited unless an exception is granted with documented compensating controls.

11. **Third-Party and Vendor Connections**
    1. Connections from third-party networks must terminate in a controlled DMZ and be restricted to necessary services.
    2. Third parties must sign security agreements and undergo regular assessments to ensure compliance with company standards.

12. **Network Security Testing**
    1. Periodic vulnerability scans and penetration tests shall be performed to evaluate network defenses.
    2. Findings must be remediated according to the vulnerability management policy.

13. **Documentation and Diagramming**
    1. Up-to-date network diagrams and asset inventories must be maintained to support security analysis and troubleshooting.

## Roles and Responsibilities

1. **Network Administrators:** Configure, maintain, and monitor network security controls, ensure compliance with change management procedures, and document network diagrams.
2. **Security Team:** Reviews logs, performs vulnerability assessments, coordinates incident response, and conducts periodic penetration tests.
3. **IT Operations:** Supports deployment of network infrastructure and ensures backups of device configurations.
4. **Employees and Contractors:** Use corporate networks only for authorized purposes and report suspected security issues.

## Accountable Roles and Decision Authority

1. **Director:** Owns and maintains this policy, coordinates updates, and ensures alignment with the Cyber Governance Policy and Document Control Policy.
2. **Director (Risk Owner):** Reviews and approves exceptions, risk acceptances, and material control changes, documenting rationale in line with the Risk Management Policy.
3. **Director (Service Owner):** Oversees day-to-day execution of this policy, vendor engagement, and customer communications when actions affect external parties.


## Training and Awareness

1. Administrators must receive ongoing training on secure network design and emerging threats.
2. Employees shall complete annual security awareness training that includes safe network usage practices.

## Compliance and Review

Noncompliance may result in access restrictions or disciplinary action. This policy is reviewed annually or after significant network changes to ensure alignment with evolving security requirements and business objectives.

## Revision History

| Version | Date       | Description                        | Author |
| ------- | ---------- | ---------------------------------- | ------ |
| 1.0     | 2023-01-01 | Initial policy release             | NetSec |
| 2.0     | 2025-09-10 | Comprehensive expansion and update | NetSec |
| 3.0     | 2025-09-10 | Implementation guidelines added | Policy Team |

## Implementation Guidelines
1. The Director records policy-related approvals and evidence in the central document repository and retains them for audit purposes.
2. BitLocker-encrypted storage protects customer data on company systems, and Windows Defender telemetry is reviewed weekly.
3. Weekly vulnerability scans and monthly patch reviews are led by the Director, with remediation actions tracked to completion.
4. Microsoft 365 security settings rely on features provided within the standard licence; compensating controls are documented when advanced tooling is unavailable.
5. Exceptions require written approval from the Director, including compensating controls and a defined review date.

