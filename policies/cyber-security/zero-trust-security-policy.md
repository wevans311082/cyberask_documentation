# Zero Trust Security Policy

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

This policy establishes requirements for zero trust security to protect organizational assets and ensure compliance with applicable laws and regulations.

## Scope

This policy applies to all employees, contractors, and third parties who access or manage company resources related to zero trust security.

## Policy
1. The organization shall define and document procedures for zero trust security.
2. Controls for zero trust security must align with industry best practices and regulatory obligations.
3. Activities related to zero trust security shall be reviewed and updated regularly to address emerging risks.
4. Records demonstrating compliance with this policy shall be maintained.

1. All aspects of Zero Trust Security Policy must align with ISO/IEC 27001:2022 controls and the NCSC Cyber Assessment Framework.
2. Procedures shall be documented, communicated, and reviewed at least annually by the Director.
3. Staff and contractors must receive training on Zero Trust Security Policy before being granted related responsibilities.
4. Access and activities associated with Zero Trust Security Policy shall be logged and monitored to detect and respond to unauthorised actions.
5. Deviations from this policy must be reported within 24 hours and remedied within 30 days.
6. Technology configurations supporting Zero Trust Security Policy must follow relevant CIS Benchmarks and vendor hardening guides.
7. Third parties engaged in Zero Trust Security Policy processes shall have contractual obligations to meet equivalent security standards.
8. Records demonstrating compliance with this policy shall be retained for audit for a minimum of six years.
9. The Director must approve exceptions in writing, including scope, duration, and compensating controls.
10. Failure to comply with this policy may result in disciplinary action, removal of access, or termination of contract.

1. Systems processing Zero Trust Security Policy shall enforce least privilege and role-based access controls.
2. Changes affecting Zero Trust Security Policy configurations must follow the Change Management Policy and receive formal approval.
3. Monitoring tools shall generate alerts for Zero Trust Security Policy violations and designated staff must review these alerts daily.
4. Internal audits shall verify adherence to Zero Trust Security Policy at least annually and report findings to senior management.
5. Data associated with Zero Trust Security Policy must be protected in accordance with GDPR and UK statutory requirements.
6. Users shall acknowledge and accept this policy annually to retain relevant access rights.

## Technical Controls

1. Configure and maintain systems to enforce the requirements of the Zero Trust Security Policy, using appropriate tools and automation.
2. Enable logging, monitoring, and alerting to detect and respond to deviations from the Zero Trust Security Policy.
3. Apply encryption, access controls, and regular audits to ensure compliance with this policy.

## Roles and Responsibilities

1. **Employees and Contractors:** Follow zero trust security procedures and report issues or non-compliance.
2. **Management:** Provide resources and enforce this policy within their areas of responsibility.
3. **Security and Compliance Teams:** Monitor zero trust security controls, provide guidance, and coordinate improvements.

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

## Zero Trust Pillars in Practice

The Cyber Ask zero-trust programme is structured around three core pillars: Verify Explicitly, Enforce Least Privilege, and Assume Breach. Each pillar is supported by technology controls, operational procedures, and continuous improvement cycles.

### Verify Explicitly

- **Identity Assurance:** Every access request must be authenticated using phishing-resistant methods (FIDO2 hardware keys, certificate-based auth) coupled with conditional access policies. Device posture, geolocation, time-of-day, and behavioural risk scores inform allow/deny decisions.
- **Continuous Validation:** Session re-evaluation occurs whenever context changes—new device, unusual network, privilege escalation, or anomalous behaviour. Microsoft Entra ID Conditional Access and BeyondCorp-inspired proxies enforce re-authentication and step-up checks.
- **Telemetry Integration:** Authentication, network, endpoint, and SaaS logs feed into the central SIEM (e.g., Splunk, Microsoft Sentinel). Automated correlations flag access anomalies such as impossible travel, excessive privilege activation, and abnormal API usage.

### Enforce Least Privilege

- **Dynamic RBAC and ABAC:** Access entitlements are calculated based on role, attributes (department, project, device compliance), and sensitivity of requested resources. Privileges are granted just-in-time, expire automatically, and require renewal with documented justification.
- **Micro-Segmentation:** Network segmentation is enforced using VMware NSX or Illumio to create granular policy zones. For example, consulting project environments are isolated from corporate services, and east-west traffic is restricted to approved application flows.
- **Data-Centric Controls:** Data loss prevention (DLP) and information protection labels define who can access, modify, or share sensitive documents. Encryption keys are scoped to business units, preventing lateral access even within the same domain.

### Assume Breach

- **Threat Hunting:** Analysts proactively search for indicators of compromise across identity, endpoint, and cloud telemetry. Hunt queries run weekly and include behavioural analytics to detect stealthy adversaries.
- **Resilience Engineering:** Incident response playbooks emphasise rapid containment, forensic readiness, and service restoration. Backup systems are segmented and protected by immutable storage to mitigate ransomware threats.
- **Red Team Exercises:** Annual red/purple team engagements test zero-trust controls, focusing on bypass attempts and privilege escalation. Findings drive improvements in detection rules and automation scripts.

## Micro-Segmentation Blueprint

Micro-segmentation divides the network into isolated trust zones to limit lateral movement. Cyber Ask deploys the following approach:

1. **Zone Classification:** Assets are categorised into zones: Identity Services, Core Productivity, Client Deliverables, Development/Test, and Management Plane. Each zone has defined ingress/egress policies.
2. **Policy Definition:** Using NSX distributed firewalls, policies are written in plain language (e.g., "Allow HTTPS from Compliance Workstations to Case Management App"). Illumio labels support workload-based enforcement for hybrid environments.
3. **Enforcement Mechanics:** Traffic flows are monitored in discovery mode before enforcement to understand dependencies. Once baselines are established, default-deny rules block unapproved flows.
4. **Change Management:** Policy changes require risk assessments, peer review, and testing in a staging environment. Automated compliance checks validate that segmentation rules align with CIS benchmarks and regulatory obligations.
5. **Visibility:** NSX Intelligence dashboards and Illumio Explorer provide heatmaps of traffic patterns. Anomalies, such as unexpected RDP traffic between zones, trigger alerts and incident response procedures.

## Behavioural Analytics and SIEM Integration

Behavioural analytics provide continuous verification of user and entity behaviour. The SIEM aggregates telemetry from identity providers, endpoints, network sensors, and SaaS APIs.

- **Data Sources:** Microsoft 365 audit logs, Okta/BeyondCorp access data, EDR telemetry, DNS logs, firewall events, and CASB alerts feed into Splunk or Sentinel.
- **Machine Learning Models:** UEBA (User and Entity Behaviour Analytics) models establish baselines for login frequency, file access volumes, and data transfer rates. Deviations generate risk scores and automated containment actions (e.g., temporary session suspension).
- **Sample Splunk Queries:**
  - Detect suspicious OAuth consent grants:
    ```spl
    index=o365 sourcetype="o365:management" Workload="AzureActiveDirectory" Operation="Consent to application"
    | stats count by UserId, AppId
    | where count > 2
    ```
  - Flag anomalous data exfiltration:
    ```spl
    index=proxy_logs action=allowed
    | stats sum(bytes_out) as total_out by user, dest_domain
    | where total_out > 5*avg(total_out) by user
    ```
- **Automated Response:** SOAR workflows isolate devices, revoke tokens, or prompt MFA challenges when high-risk scores are detected. Alerts integrate with the incident response process for triage and remediation.

## Zero Trust Architecture Diagram

```mermaid
graph LR
    subgraph Users
        A[Employees]
        B[Contractors]
        C[Clients]
    end
    subgraph Devices
        D[Managed Laptops]
        E[Mobile Devices]
        F[Virtual Desktops]
    end
    subgraph Access
        G[Identity Provider
(Microsoft Entra ID)]
        H[Okta/BeyondCorp Proxy]
        I[Conditional Access Policies]
    end
    subgraph Security Services
        J[SIEM/UEBA]
        K[SOAR Automation]
        L[EDR/Defender]
        M[DLP/Information Protection]
    end
    subgraph Resources
        N[Client Data Zone]
        O[Productivity Apps]
        P[Management Plane]
        Q[Development Zone]
    end

    A --> D
    B --> E
    C --> F
    D --> G
    E --> G
    F --> G
    G --> H
    H --> I
    I --> N
    I --> O
    I --> P
    I --> Q
    J --> K
    L --> J
    M --> J
    H --> J
    K --> H
    K --> L
    K --> M
```

## Implementation Roadmap and Risk Heatmap

Zero-trust adoption progresses through phased implementation. Each phase evaluates residual risk levels and control maturity.

| Phase | Description | Key Activities | Risk Level (Pre-Control) | Residual Risk (Post-Control) |
| --- | --- | --- | --- | --- |
| Phase 1: Foundation | Establish identity-centric controls. | Enforce phishing-resistant MFA, inventory assets, deploy conditional access. | High | Medium |
| Phase 2: Visibility | Gain holistic telemetry and classify assets. | Integrate SIEM, deploy NSX/Illumio sensors, map data flows. | High | Medium |
| Phase 3: Enforcement | Apply micro-segmentation and least privilege. | Implement zone policies, PIM, DLP, and just-in-time access. | Medium | Low |
| Phase 4: Automation | Automate response and continuous validation. | Deploy SOAR runbooks, UEBA-driven containment, automated compliance checks. | Medium | Low |
| Phase 5: Optimisation | Continuous improvement and resilience. | Conduct red-team exercises, refine analytics models, update playbooks. | Medium | Very Low |

Residual risk values are reviewed quarterly and after major changes to validate that controls remain effective and aligned with business priorities.

## Governance and Accountability

- The Director serves as Zero Trust Programme Owner, chairing monthly steering meetings to review metrics, risk register entries, and project milestones.
- A cross-functional working group (security, IT, legal, client services) assesses new technology requests for zero-trust alignment before procurement.
- Exceptions to zero-trust mandates require a documented business justification, compensating controls, and an expiration date not exceeding 90 days.
- Third-party vendors must demonstrate equivalent zero-trust controls through due diligence questionnaires and contractual clauses.

## Metrics and Continuous Improvement

Key performance indicators demonstrate programme effectiveness:

- Percentage of applications protected by conditional access and micro-segmentation.
- Time to revoke compromised credentials detected via UEBA alerts.
- Number of lateral movement attempts blocked by NSX/Illumio policies.
- Coverage of automated response playbooks (measured by incidents resolved without manual intervention).
- Training completion rates for zero-trust awareness modules.

Findings inform quarterly improvement plans and budget allocations. Lessons learned from incidents or exercises drive updates to control objectives and technology investments.

## Training and Culture

Zero trust success depends on user behaviour. The organisation delivers multi-layered education:

- **Foundational Modules:** Introduce zero-trust concepts, emphasising the move away from perimeter-based thinking.
- **Role-Based Labs:** Administrators practice configuring conditional access, micro-segmentation policies, and Splunk queries in sandbox environments.
- **Executive Briefings:** Highlight business benefits, compliance outcomes, and investment requirements.
- **Tabletop Exercises:** Simulate breach scenarios to reinforce assume-breach mindset and validate cross-team coordination.

Training attendance is tracked via the learning management system, and completion is required for system access privileges.

## Integration with Broader Security Frameworks

Zero-trust controls complement other enterprise policies:

- **Access Control Policy:** Provides RBAC foundations and provisioning workflows consumed by zero-trust enforcement mechanisms.
- **Incident Response Policy and Plan:** Define escalation paths when zero-trust analytics detect anomalies.
- **Passwordless and MFA Policies:** Supply the identity assurance capabilities necessary for verify-explicitly controls.
- **Cloud and API Security Policies:** Extend zero-trust principles to infrastructure-as-a-service, platform-as-a-service, and API ecosystems.

Cross-references ensure consistent control implementation and facilitate audits.

