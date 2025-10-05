# Business Continuity Plan

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** WEvans Director

This plan ensures critical business functions continue during and after a disruption, aligning with CE/CE+ and ISO/IEC 22301 business continuity and ISO/IEC 27001 information security requirements. It establishes a framework to protect life, safeguard assets, and maintain stakeholder confidence through predefined recovery strategies and communication protocols.

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

The purpose of this Business Continuity Plan (BCP) is to provide structured procedures for maintaining or rapidly resuming essential operations following an outage, disaster, or other disruptive event. The plan seeks to minimize downtime, reduce financial loss, and preserve the organization’s reputation by ensuring that critical services remain available within acceptable timeframes.

## Scope

This plan applies to all departments, business units, and supporting services that contribute to customer obligations, regulatory commitments, or essential internal operations. It covers disruptions arising from natural disasters, technological failures, cyber incidents, pandemics, and any other events that could significantly impact the company’s ability to operate. Third-party providers supporting critical processes must maintain compatible continuity plans and provide evidence upon request.

## Definitions

1. **Maximum Tolerable Downtime (MTD):** The longest period that a critical process can be unavailable before unacceptable consequences occur.
2. **Recovery Time Objective (RTO):** The target time set for resumption of a product, service, or process after a disruption.
3. **Recovery Point Objective (RPO):** The maximum tolerable amount of data loss measured in time.
4. **Alternate Work Area:** An offsite facility equipped to support business functions if the primary site is unavailable.

## Plan Elements

1. **Business Impact Analysis (BIA)**
   1. Identify critical processes, resources, and dependencies.
   2. Determine MTD, RTO, and RPO for each process and document in the BIA report.
   3. Assess the financial, regulatory, and reputational impact of potential disruptions.

2. **Risk Assessment**
   1. Evaluate threats such as natural hazards, system failures, supply chain disruptions, and malicious attacks.
   2. Assign likelihood and impact ratings to prioritize mitigation efforts.

3. **Recovery Strategies**
   1. Define alternate processing sites, backup data centers, and cloud failover capabilities.
   2. Establish contracts with alternate suppliers and logistics providers.
   3. Identify manual workarounds for critical processes when automated systems are unavailable.

4. **Plan Activation and Communication**
   1. Establish clear criteria for invoking the BCP, including incident severity levels and decision thresholds.
   2. Provide notification procedures for employees, customers, partners, and regulators using predefined contact lists.
   3. Utilize mass notification systems and redundant communication channels to ensure message delivery.

5. **Emergency Response and Safety**
   1. Prioritize life safety and coordinate with local emergency services when appropriate.
   2. Maintain evacuation plans, shelter-in-place procedures, and first-aid resources at each facility.

6. **Testing and Exercises**
   1. Conduct tabletop exercises, functional tests, and full-scale simulations at least annually.
   2. Document lessons learned and incorporate improvements into the plan within 60 days of each test.

7. **Plan Maintenance**
   1. Review and update the BCP whenever organizational, technological, or regulatory changes occur, or at least annually.
   2. Maintain version control and distribute updated copies to all stakeholders.

## Roles and Responsibilities

1. **Executive Management:** Provide strategic direction, approve the plan, allocate resources, and champion continuity planning across the organization.
2. **Business Continuity Manager:** Coordinates development, testing, maintenance, and activation of the BCP. Serves as the primary point of contact during disruptions.
3. **Department Leads:** Develop and maintain recovery procedures for their functions, ensure staff training, and participate in exercises.
4. **IT Disaster Recovery Team:** Manages restoration of technology services, including systems, networks, and data.
5. **Employees:** Follow instructions during activation, report issues, and maintain awareness of their role in continuity procedures.

## Accountable Roles and Decision Authority

1. **Director:** Owns and maintains this policy, coordinates updates, and ensures alignment with the Cyber Governance Policy and Document Control Policy.
2. **Director (Risk Owner):** Reviews and approves exceptions, risk acceptances, and material control changes, documenting rationale in line with the Risk Management Policy.
3. **Director (Service Owner):** Oversees day-to-day execution of this policy, vendor engagement, and customer communications when actions affect external parties.


## Training and Awareness

1. All employees shall receive BCP awareness training during onboarding and annually thereafter.
2. Key personnel involved in recovery processes must participate in specialized training and exercises relevant to their roles.

## Monitoring and Review

1. After each test or activation, a formal debrief shall be conducted to evaluate performance and identify areas for improvement.
2. Audit and compliance teams may review BCP documentation and test results to verify adherence to standards.

## Supplier and Third-Party Continuity

1. Critical suppliers must provide assurance of their own continuity capabilities and notify the organization of any significant disruptions affecting service delivery.
2. Service level agreements should include provisions for continuity and disaster recovery testing.

## Plan Distribution

1. Controlled copies of this plan shall be stored in both physical and electronic formats with access restricted to authorized personnel.
2. A condensed quick-reference guide will be distributed to key staff for use during emergencies.

## Exceptions

1. Any exceptions to this plan must be documented, risk assessed, and approved by executive management. Compensating controls must be identified to mitigate associated risks.

## Plan Review and Approval

This plan is reviewed after each test or activation and is formally approved by executive management at least annually to ensure continued effectiveness and alignment with business objectives.

## Revision History

| Version | Date       | Description                        | Author |
| ------- | ---------- | ---------------------------------- | ------ |
| 1.0     | 2023-01-01 | Initial plan release               | BCM    |
| 2.0     | 2025-09-10 | Comprehensive expansion and update | BCM    |
| 3.0     | 2025-09-10 | Implementation guidelines added | Policy Team |

## Implementation Guidelines
1. The Director records policy-related approvals and evidence in the central document repository and retains them for audit purposes.
2. BitLocker-encrypted storage protects customer data on company systems, and Windows Defender telemetry is reviewed weekly.
3. Weekly vulnerability scans and monthly patch reviews are led by the Director, with remediation actions tracked to completion.
4. Microsoft 365 security settings rely on features provided within the standard licence; compensating controls are documented when advanced tooling is unavailable.
5. Exceptions require written approval from the Director, including compensating controls and a defined review date.

