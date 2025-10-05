# Incident Response Plan

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** Wayne Evans (Director)

This plan outlines the process for detecting, responding to, and recovering from cybersecurity incidents in alignment with CE/CE+ and ISO/IEC 27035 incident management requirements. A consistent response framework ensures that security events are handled efficiently, evidence is preserved, and stakeholder communication is timely and accurate.

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

The purpose of the Incident Response Plan (IRP) is to provide a structured approach to minimize the impact of security incidents, protect organizational assets, and meet legal, regulatory, and contractual obligations. The plan establishes clear procedures for coordinating response activities, preserving evidence, and implementing lessons learned.

## Scope

This plan applies to all information assets, personnel, facilities, and third parties interacting with company systems. It covers incidents ranging from malware infections and data breaches to physical security breaches and insider threats. All employees and contractors must understand their role in the incident response process.

## Definitions

1. **Incident:** An event that compromises the confidentiality, integrity, or availability of information assets.
2. **Event:** A deviation from normal operations that may or may not be an incident.
3. **Security Operations Center (SOC):** The team responsible for monitoring and analyzing activity to detect threats.
4. **Forensic Preservation:** The process of collecting and maintaining evidence in a manner suitable for legal proceedings.

## Response Phases

1. **Preparation**
   1. Maintain incident response policies, playbooks, tools, and secure communication channels.
   2. Conduct regular training and exercises for the incident response team and supporting personnel.
   3. Ensure contact lists for internal teams, external partners, and regulators are current and accessible.

2. **Identification**
   1. Monitor systems, applications, and networks for indicators of compromise using automated tools and manual processes.
   2. Employees must report suspected incidents to the SOC or service desk immediately.
   3. The SOC validates alerts, classifies the incident, and assigns a severity level.

3. **Containment**
   1. Implement short-term measures such as isolating affected systems, disabling compromised accounts, or blocking malicious IP addresses to prevent further damage.
   2. Develop long-term containment strategies that may include patching systems, applying firewall rules, or migrating services to alternate environments.

4. **Eradication**
   1. Remove malicious code, unauthorized changes, or artifacts from affected systems.
   2. Identify the root cause and address underlying vulnerabilities or process gaps.
   3. Coordinate with vendors or forensic specialists if specialized expertise is required.

5. **Recovery**
   1. Restore systems from clean backups, reintroduce services in a controlled manner, and validate integrity through testing.
   2. Monitor restored systems for signs of recurring issues before declaring the incident closed.

6. **Lessons Learned**
   1. Within 30 days of incident closure, conduct a post-incident review involving all relevant stakeholders.
   2. Document findings, update risk assessments, and implement improvements to policies, procedures, and controls.

## Roles and Responsibilities

1. **Incident Response Coordinator (IRC):** Leads response activities, ensures adherence to the IRP, and serves as primary communication point.
2. **Security Operations Center:** Detects and triages events, gathers evidence, and supports containment and eradication activities.
3. **IT and Infrastructure Teams:** Execute technical containment, eradication, and recovery tasks.
4. **Management and Executive Team:** Approves external communications, allocates resources, and provides strategic direction.
5. **Legal and Compliance:** Advises on regulatory obligations, coordinates with law enforcement, and manages eDiscovery requirements.
6. **Communications/Public Relations:** Handles public statements and media inquiries in coordination with management.
7. **All Employees:** Report suspected incidents promptly and cooperate with investigators.

## Accountable Roles and Decision Authority

1. **Director:** Owns and maintains this policy, coordinates updates, and ensures alignment with the Cyber Governance Policy and Document Control Policy.
2. **Director (Risk Owner):** Reviews and approves exceptions, risk acceptances, and material control changes, documenting rationale in line with the Risk Management Policy.
3. **Director (Service Owner):** Oversees day-to-day execution of this policy, vendor engagement, and customer communications when actions affect external parties.


## Communication and Reporting

1. Incidents must be reported via the service desk or designated hotline within one hour of discovery.
2. High-severity incidents are escalated immediately to executive management, legal, and the Director.
3. External communications to customers, partners, or regulators require prior approval from management and legal.
4. Evidence must be collected and preserved according to forensic best practices; chain-of-custody documentation is mandatory for all collected evidence.

## Incident Severity Levels

1. **Low:** Minimal impact with limited scope; handled by operational staff.
2. **Medium:** Noticeable impact requiring coordination across teams; may involve external notifications.
3. **High:** Significant impact on critical systems or data; requires executive management involvement and potential regulatory reporting.
4. **Critical:** Severe impact threatening organizational viability or public safety; immediate escalation to crisis management team.

## Coordination with Law Enforcement and Regulators

1. The Legal and Compliance team determines when engagement with law enforcement or regulatory bodies is required.
2. All communications with external authorities must be coordinated through the IRC and Legal to maintain consistency and protect privileged information.

## Tools and Resources

1. Maintain an incident response toolkit containing forensic utilities, communication templates, and hardware for evidence acquisition.
2. Ensure secure storage for collected evidence and incident documentation.

## Training and Exercises

1. Conduct incident response tabletop exercises twice per year and full-scale simulations annually.
2. Provide specialized training for incident handlers on malware analysis, forensic techniques, and legal considerations.

## Metrics and Reporting

1. Track metrics such as mean time to detect (MTTD), mean time to respond (MTTR), and number of incidents by category.
2. Report quarterly to executive management on incident trends and improvement initiatives.

## Post-Incident Reporting

1. A formal incident report summarizing timeline, impact, root cause, and remediation actions must be issued within two weeks of incident closure.
2. Reports shall be retained for at least five years and made available to auditors and regulators upon request.

## Plan Maintenance and Review

1. The IRP is reviewed annually or after significant incidents to ensure effectiveness.
2. Updates must be communicated to all stakeholders, and training adjusted to reflect procedural changes.

## Exceptions

1. Any deviations from this plan must be documented and approved by the Director, including compensating controls and expiration dates.

## Revision History

| Version | Date       | Description                        | Author  |
| ------- | ---------- | ---------------------------------- | ------- |
| 1.0     | 2023-01-01 | Initial plan release               | IR Team |
| 2.0     | 2025-09-10 | Comprehensive expansion and update | IR Team |
| 3.0     | 2025-09-10 | Implementation guidelines added | Policy Team |
| 3.1     | 2025-10-05 | Author attribution updated | Wayne Evans (Director) |

## Implementation Guidelines
1. The Director records policy-related approvals and evidence in the central document repository and retains them for audit purposes.
2. BitLocker-encrypted storage protects customer data on company systems, and Windows Defender telemetry is reviewed weekly.
3. Weekly vulnerability scans and monthly patch reviews are led by the Director, with remediation actions tracked to completion.
4. Microsoft 365 security settings rely on features provided within the standard licence; compensating controls are documented when advanced tooling is unavailable.
5. Exceptions require written approval from the Director, including compensating controls and a defined review date.


## Contact Directory

The following contacts must be reachable 24/7 during incident response. Contact information is reviewed quarterly and whenever staffing changes occur.

| Role | Primary Contact | Contact Details | Availability | Backup Contact |
| --- | --- | --- | --- | --- |
| Incident Response Coordinator | Wayne Evans | +44 20 0000 0000 / incident@cyberask.co.uk | 24/7 on-call | Managed Service SOC lead |
| Security Operations (Managed SOC) | SecureOps Partner | soc@secureops.example / +44 800 555 0101 | 24/7 monitoring | Director |
| Legal Counsel | External Counsel (TechLaw LLP) | legal@techlawllp.example / +44 20 5555 2222 | Business hours with emergency hotline | Director |
| Cloud Provider Support | Microsoft Premier Support | portal.microsoft.com | 24/7 with severity-based SLA | Director |
| Cyber Insurance Carrier | InsureCyber Claims Desk | claims@insurecyber.example / +44 800 777 3333 | 24/7 | Legal Counsel |
| Law Enforcement Liaison | National Cyber Security Centre (NCSC) | ncscincidents@ncsc.gov.uk | 24/7 | Director |

## Escalation Matrix

Incident escalations follow the matrix below to ensure timely leadership engagement and resource mobilization.

| Severity | Impact Description | RTO Target | RPO Target | Notification Requirements | Escalation Path |
| --- | --- | --- | --- | --- | --- |
| Low | Minor service degradation, no data exposure. | 24 hours | 1 business day | Internal ticket updates. | IRC → Managed SOC |
| Medium | Limited data exposure or customer impact. | 12 hours | 4 hours | Director, affected clients within 48 hours. | IRC → Director → Legal |
| High | Significant data breach or service outage. | 4 hours | 1 hour | Director, clients within 24 hours, regulators within 72 hours. | IRC → Director → Executive Briefing → Legal & Communications |
| Critical | Catastrophic impact or existential threat. | 2 hours | Near-zero tolerance | Immediate regulator and law enforcement engagement. | IRC → Director → Crisis Management Team → Board |

## AI-Enhanced Detection and Analysis

As of 2025, the Managed SOC deploys AI-driven detection pipelines that fuse endpoint telemetry, Microsoft 365 audit logs, and cloud workload metrics. Machine learning models surface anomalous behaviours such as lateral movement, data exfiltration patterns, and suspicious OAuth consent grants. Analysts validate AI-generated alerts within 15 minutes, and feedback is fed into model tuning cycles. Integration with the SOAR platform enables automated enrichment, including threat intelligence lookups, geolocation tagging, and historical event correlation.

## Response Playbooks

Playbooks provide step-by-step guidance tailored to incident type. Each playbook references the core response phases defined in the [Incident Response Policy](./incident-response-policy.md).

### Ransomware Playbook

1. **Detection and Validation**
   - Confirm the ransomware strain using hash analysis and reverse engineering resources provided by NoMoreRansom.
   - Initiate forensic imaging of affected systems before powering down or reimaging devices.

2. **Containment**
   - Isolate infected endpoints by disabling network interfaces and removing from domain trust relationships.
   - Revoke compromised credentials and enforce password resets or key rotation for service accounts.
   - Block command-and-control indicators at firewall and proxy layers.

3. **Eradication**
   - Deploy EDR cleansing scripts or trusted rebuild images to affected systems.
   - Patch exploited vulnerabilities and review access control changes introduced by attackers.
   - Remove persistence mechanisms (scheduled tasks, registry keys, startup items).

4. **Recovery**
   - Restore systems from immutable, offline backups verified to be ransomware-free. Validate integrity via checksums and application testing.
   - Reintroduce services gradually, prioritizing critical workloads to meet the four-hour RTO.
   - Monitor network traffic and SIEM alerts for evidence of reinfection.

5. **Negotiation and Communication**
   - Engage legal counsel and cyber insurance prior to any communication with threat actors. Payment decisions require Director approval and insurer concurrence.
   - Prepare client and regulator notifications outlining impact, remediation, and next steps.

6. **Lessons Learned**
   - Document attack vectors, security control gaps, and response timelines. Update the ransomware tabletop exercise scenario to incorporate observed tactics.

### Business Email Compromise (BEC) Playbook

1. Validate suspicious email forwarding rules, OAuth grants, and unusual login locations using SIEM dashboards.
2. Revoke tokens, reset passwords, and enable conditional access requiring phishing-resistant MFA.
3. Coordinate with finance to halt fraudulent payments and initiate recall procedures.
4. Notify affected clients and update DMARC/DKIM policies to strengthen email authentication.

### Cloud Configuration Breach Playbook

1. Use cloud security posture management (CSPM) alerts to identify misconfigured resources.
2. Apply remediation templates (infrastructure as code) to enforce baseline security settings.
3. Run compliance scans post-remediation to verify alignment with CIS benchmarks.

## Communication Templates

Incident handlers must use approved communication templates stored in the secure document library. Templates cover executive briefings, customer notifications, regulatory disclosures, and internal status updates. Each template includes sections for incident summary, impact, containment status, next steps, and key contacts.

## Evidence Handling Procedures

- Capture system images, log exports, and memory dumps using write-protected media.
- Maintain chain-of-custody documentation, logging each transfer of evidence with timestamps and signatures.
- Store evidence in encrypted repositories with access restricted to the Director, IRC, and legal counsel.

## Post-Incident Review Workflow

1. Schedule debrief within ten business days of incident closure.
2. Review timeline, tooling performance, communications, and decision points.
3. Identify corrective actions, assign owners, and track remediation progress via the risk register.
4. Update metrics dashboards with actual MTTD/MTTR values and RTO/RPO performance.

## Plan Testing and Continuous Improvement

- Conduct quarterly tabletop exercises focused on ransomware, BEC, and insider threat scenarios, incorporating AI-generated anomalies to test detection accuracy.
- Perform at least one live failover test annually to verify backup restoration capabilities meet RPO expectations.
- Coordinate with third-party providers to validate incident communication pathways and joint responsibilities.

