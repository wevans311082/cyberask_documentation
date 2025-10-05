# PCI DSS Policy

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

This policy establishes requirements for pci dss to protect organizational assets and ensure compliance with applicable laws and regulations.

## Scope

This policy applies to all employees, contractors, and third parties who access or manage company resources related to pci dss.

## Policy

Cyber Ask Ltd adopts the Payment Card Industry Data Security Standard (PCI DSS) as the baseline framework for protecting cardholder data. The following subsections detail the 12 PCI DSS requirements and the controls implemented to satisfy them.

### Requirement 1 – Install and Maintain Network Security Controls
1. Maintain documented firewall and router standards, including justification for all open ports and services.
2. Enforce network segmentation that isolates the Cardholder Data Environment (CDE) from corporate and development networks, with quarterly verification of segmentation effectiveness.
3. Restrict inbound and outbound traffic to only what is necessary for payment processing partners and service providers.

### Requirement 2 – Apply Secure Configurations to All System Components
1. Change vendor-supplied defaults (passwords, SNMP strings, certificates) before systems are deployed in the CDE.
2. Maintain configuration hardening baselines aligned to CIS Benchmarks for servers, workstations, and network devices supporting payment services.
3. Document and approve configuration deviations through the Change Management Policy with compensating controls.

### Requirement 3 – Protect Stored Account Data
1. Prohibit storage of sensitive authentication data post-authorization unless explicitly justified and approved.
2. Encrypt primary account numbers (PAN) using industry-standard algorithms and manage keys in secure, access-controlled repositories.
3. Render PAN unreadable wherever stored through truncation, tokenisation, or hashing mechanisms.

### Requirement 4 – Protect Cardholder Data with Strong Cryptography During Transmission
1. Use TLS 1.2 or higher for all transmissions of cardholder data across open, public networks.
2. Maintain up-to-date certificates and disable insecure protocols and ciphers.
3. Monitor network connections for unauthorised services attempting to transmit cardholder data.

### Requirement 5 – Protect Systems and Networks from Malicious Software
1. Deploy anti-malware solutions with automatic signature updates across all endpoints within the CDE and supporting systems.
2. Restrict administrative privileges to reduce the likelihood of malware execution.
3. Review malware alerts daily and document response actions within the incident management system.

### Requirement 6 – Develop and Maintain Secure Systems and Software
1. Track vendor security advisories and apply critical patches within 30 days for systems in scope for PCI DSS.
2. Follow secure coding practices, including static and dynamic testing, for any bespoke payment integrations.
3. Document change approvals and rollback procedures for software impacting the CDE.

### Requirement 7 – Restrict Access to System Components and Cardholder Data
1. Grant access based on least privilege and role-based access controls reviewed at least quarterly.
2. Enforce unique IDs for each user and document access approval workflows.
3. Remove or disable access promptly when personnel change roles or leave the organisation.

### Requirement 8 – Identify Users and Authenticate Access to System Components
1. Require multi-factor authentication for all remote access to the CDE and administrative functions.
2. Enforce password complexity, lockout thresholds, and session timeouts per PCI DSS minimums.
3. Log authentication events and correlate them with privileged activity monitoring.

### Requirement 9 – Restrict Physical Access to Cardholder Data
1. Store physical media containing cardholder data in locked cabinets with access logs and CCTV coverage where applicable.
2. Escort visitors within facilities housing CDE systems and record their entry/exit times.
3. Destroy media securely using shredding or degaussing before disposal or reuse.

### Requirement 10 – Log and Monitor All Access to System Components and Cardholder Data
1. Centralise log collection for all CDE systems and security devices with retention meeting PCI DSS requirements.
2. Review daily security event logs, file integrity monitoring alerts, and access anomalies.
3. Synchronise system clocks using authenticated NTP sources to support forensic investigations.

### Requirement 11 – Test Security of Systems and Networks Regularly
1. Conduct quarterly external vulnerability scans by an Approved Scanning Vendor (ASV) and remediate non-compliant findings within 30 days.
2. Perform internal vulnerability scans at least quarterly and after significant changes, documenting remediation actions.
3. Execute annual penetration tests that include segmentation testing and validation of scoping assumptions.

### Requirement 12 – Support Information Security with Organisational Policies and Programmes
1. Maintain and annually review PCI DSS policies, incident response procedures, and third-party agreements.
2. Deliver PCI DSS awareness training to all personnel with access to the CDE before access is granted and annually thereafter.
3. Maintain a risk assessment covering the CDE, including vendor reliance, emerging threats, and business changes.

### Merchant-Specific Exemptions
1. Cyber Ask Ltd primarily operates as a consultancy without direct storage, processing, or transmission of cardholder data, relying on third-party payment service providers. As such, the company qualifies for the SAQ A or SAQ A-EP (where web redirection is used) and leverages service provider attestations to reduce control scope.
2. Where engagements require handling of client-provided card data for analysis, a documented risk assessment and temporary scope expansion must be approved by the Director, including compensating controls and data minimisation steps.
3. Any reliance on service provider PCI DSS compliance is documented with current Attestations of Compliance (AOCs) and service descriptions clarifying shared responsibilities.

## Technical Controls

1. Configure and maintain systems to enforce the requirements of the PCI DSS Policy, using appropriate tools and automation.
2. Enable logging, monitoring, and alerting to detect and respond to deviations from the PCI DSS Policy.
3. Apply encryption, access controls, and regular audits to ensure compliance with this policy.

## Roles and Responsibilities

1. **Employees and Contractors:** Follow pci dss procedures and report issues or non-compliance.
2. **Management:** Provide resources and enforce this policy within their areas of responsibility.
3. **Security and Compliance Teams:** Monitor pci dss controls, provide guidance, and coordinate improvements.

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
