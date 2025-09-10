# Incident Response Plan

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** WEvans Director

This plan outlines the process for detecting, responding to, and recovering from cybersecurity incidents in alignment with CE/CE+ and ISO/IEC 27035 incident management requirements. A consistent response framework ensures that security events are handled efficiently, evidence is preserved, and stakeholder communication is timely and accurate.

## Purpose

The purpose of the Incident Response Plan (IRP) is to provide a structured approach to minimize the impact of security incidents, protect organizational assets, and meet legal, regulatory, and contractual obligations. The plan establishes clear procedures for coordinating response activities, preserving evidence, and implementing lessons learned.

## Scope

This plan applies to all information assets, personnel, facilities, and third parties interacting with company systems. It covers incidents ranging from malware infections and data breaches to physical security breaches and insider threats. All employees and contractors must understand their role in the incident response process.

## Definitions

- **Incident:** An event that compromises the confidentiality, integrity, or availability of information assets.
- **Event:** A deviation from normal operations that may or may not be an incident.
- **Security Operations Center (SOC):** The team responsible for monitoring and analyzing activity to detect threats.
- **Forensic Preservation:** The process of collecting and maintaining evidence in a manner suitable for legal proceedings.

## Response Phases

1. **Preparation**
   - Maintain incident response policies, playbooks, tools, and secure communication channels.
   - Conduct regular training and exercises for the incident response team and supporting personnel.
   - Ensure contact lists for internal teams, external partners, and regulators are current and accessible.

2. **Identification**
   - Monitor systems, applications, and networks for indicators of compromise using automated tools and manual processes.
   - Employees must report suspected incidents to the SOC or service desk immediately.
   - The SOC validates alerts, classifies the incident, and assigns a severity level.

3. **Containment**
   - Implement short-term measures such as isolating affected systems, disabling compromised accounts, or blocking malicious IP addresses to prevent further damage.
   - Develop long-term containment strategies that may include patching systems, applying firewall rules, or migrating services to alternate environments.

4. **Eradication**
   - Remove malicious code, unauthorized changes, or artifacts from affected systems.
   - Identify the root cause and address underlying vulnerabilities or process gaps.
   - Coordinate with vendors or forensic specialists if specialized expertise is required.

5. **Recovery**
   - Restore systems from clean backups, reintroduce services in a controlled manner, and validate integrity through testing.
   - Monitor restored systems for signs of recurring issues before declaring the incident closed.

6. **Lessons Learned**
   - Within 30 days of incident closure, conduct a post-incident review involving all relevant stakeholders.
   - Document findings, update risk assessments, and implement improvements to policies, procedures, and controls.

## Roles and Responsibilities

- **Incident Response Coordinator (IRC):** Leads response activities, ensures adherence to the IRP, and serves as primary communication point.
- **Security Operations Center:** Detects and triages events, gathers evidence, and supports containment and eradication activities.
- **IT and Infrastructure Teams:** Execute technical containment, eradication, and recovery tasks.
- **Management and Executive Team:** Approves external communications, allocates resources, and provides strategic direction.
- **Legal and Compliance:** Advises on regulatory obligations, coordinates with law enforcement, and manages eDiscovery requirements.
- **Communications/Public Relations:** Handles public statements and media inquiries in coordination with management.
- **All Employees:** Report suspected incidents promptly and cooperate with investigators.

## Communication and Reporting

- Incidents must be reported via the service desk or designated hotline within one hour of discovery.
- High-severity incidents are escalated immediately to executive management, legal, and the CISO.
- External communications to customers, partners, or regulators require prior approval from management and legal.
- Evidence must be collected and preserved according to forensic best practices; chain-of-custody documentation is mandatory for all collected evidence.

## Incident Severity Levels

- **Low:** Minimal impact with limited scope; handled by operational staff.
- **Medium:** Noticeable impact requiring coordination across teams; may involve external notifications.
- **High:** Significant impact on critical systems or data; requires executive management involvement and potential regulatory reporting.
- **Critical:** Severe impact threatening organizational viability or public safety; immediate escalation to crisis management team.

## Coordination with Law Enforcement and Regulators

- The Legal and Compliance team determines when engagement with law enforcement or regulatory bodies is required.
- All communications with external authorities must be coordinated through the IRC and Legal to maintain consistency and protect privileged information.

## Tools and Resources

- Maintain an incident response toolkit containing forensic utilities, communication templates, and hardware for evidence acquisition.
- Ensure secure storage for collected evidence and incident documentation.

## Training and Exercises

- Conduct incident response tabletop exercises twice per year and full-scale simulations annually.
- Provide specialized training for incident handlers on malware analysis, forensic techniques, and legal considerations.

## Metrics and Reporting

- Track metrics such as mean time to detect (MTTD), mean time to respond (MTTR), and number of incidents by category.
- Report quarterly to executive management on incident trends and improvement initiatives.

## Post-Incident Reporting

- A formal incident report summarizing timeline, impact, root cause, and remediation actions must be issued within two weeks of incident closure.
- Reports shall be retained for at least five years and made available to auditors and regulators upon request.

## Plan Maintenance and Review

- The IRP is reviewed annually or after significant incidents to ensure effectiveness.
- Updates must be communicated to all stakeholders, and training adjusted to reflect procedural changes.

## Exceptions

- Any deviations from this plan must be documented and approved by the CISO, including compensating controls and expiration dates.

## Revision History

| Version | Date       | Description                        | Author  |
| ------- | ---------- | ---------------------------------- | ------- |
| 1.0     | 2023-01-01 | Initial plan release               | IR Team |
| 2.0     | 2025-09-10 | Comprehensive expansion and update | IR Team |
