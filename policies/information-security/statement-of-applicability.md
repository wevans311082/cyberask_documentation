# Statement of Applicability

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** Wayne Evans (Director)

The Statement of Applicability (SoA) lists ISO/IEC 27001:2022 Annex A controls, their applicability within the organisation, justification for inclusion or exclusion, implementation status, and supporting evidence references.

## Cyber Ask Operating Context

1. Cyber Ask Ltd operates with a single employee who also serves as the sole director responsible for governance, risk, and compliance decisions.
2. Cyber Ask Ltd maintains professional liability insurance covering its consulting and advisory services.
3. A dedicated virtual machine functions as the single Windows Server domain controller and is synchronised with Microsoft Entra ID for identity management.
4. The organisation holds a standard Microsoft 365 licence; Microsoft Purview and Microsoft Defender add-ons are not deployed, and Windows Defender provides endpoint protection.
5. Customer data is stored on BitLocker-encrypted drives to protect information at rest.
6. Cyber Ask Ltd assets are vulnerability-assessed weekly and patched promptly according to remediation guidance.
7. Cyber Ask Ltd has not yet achieved Cyber Essentials, Cyber Essentials Plus, or ISO 27001 certification but aligns its controls with those standards where practicable.
8. The Director personally fulfils HR, IT administration, and compliance duties, engaging specialist suppliers when additional expertise is required.

## Structure

1. **Control Reference and Title:** Identifier and name from Annex A.
2. **Applicability:** Indicates whether the control is in scope for the organisation.
3. **Justification:** Reason for inclusion or exclusion, tied to risk treatment decisions.
4. **Implementation Status:** Implemented, In Progress, Planned, or Not Applicable.
5. **Evidence:** Key artefacts maintained in the ISMS repository.

## Control Summary

| Control | Applicability | Justification | Implementation Status | Evidence |
| --- | --- | --- | --- | --- |
| A.5.1 Policies for information security | Yes | Foundational governance for ISMS | Implemented | Approved policies, management review minutes |
| A.5.2 Information security roles and responsibilities | Yes | Clarifies accountability for controls | Implemented | Organisation chart, role descriptions |
| A.5.3 Segregation of duties | Yes | Prevents conflict of interest even in small team via dual-control suppliers | In Progress | Segregation matrix, supplier contracts |
| A.5.4 Management responsibilities | Yes | Ensures leadership oversight of security | Implemented | Management review records |
| A.5.5 Contact with authorities | Yes | Required for incident escalation and regulatory liaison | Implemented | Contact list, notification playbooks |
| A.5.6 Contact with special interest groups | Yes | Access to industry threat information | Planned | Membership applications |
| A.5.7 Threat intelligence | Yes | Supports risk assessments | In Progress | Threat bulletin repository |
| A.5.8 Information security in project management | Yes | Consulting projects require embedded security | Implemented | Project checklists, change logs |
| A.5.9 Inventory of information and other associated assets | Yes | Asset management baseline | Implemented | Asset register extracts |
| A.5.10 Acceptable use of information and other associated assets | Yes | Controls data usage by staff and contractors | Implemented | Acceptable use policy acknowledgements |
| A.5.11 Return of assets | Yes | Ensures asset recovery at offboarding | Implemented | Offboarding checklist |
| A.5.12 Classification of information | Yes | Supports handling requirements | Implemented | Data classification policy |
| A.5.13 Labelling of information | Yes | Enables consistent handling | In Progress | Labelling procedures |
| A.5.14 Information transfer | Yes | Controls secure data sharing | Implemented | Secure transfer guidelines |
| A.5.15 Access control | Yes | High-level access policy | Implemented | Access control policy |
| A.5.16 Identity management | Yes | Centralised accounts in Entra ID | Implemented | Identity lifecycle records |
| A.5.17 Authentication information | Yes | Protects credentials | Implemented | Password/MFA standards |
| A.5.18 Access rights | Yes | Regular entitlement reviews | Implemented | Quarterly access review logs |
| A.5.19 Information security in supplier relationships | Yes | Suppliers support operations | Implemented | Supplier security policy |
| A.5.20 Addressing information security within supplier agreements | Yes | Contract clauses enforce controls | Implemented | Signed contracts |
| A.5.21 Managing information security in the ICT supply chain | Yes | Reliance on SaaS providers | In Progress | Supply chain risk register |
| A.5.22 Monitoring, review and change management of supplier services | Yes | Ensures ongoing assurance | In Progress | Supplier review meeting notes |
| A.5.23 Information security for use of cloud services | Yes | Microsoft 365 hosts client data | Implemented | Cloud configuration baselines |
| A.5.24 Information security incident management planning and preparation | Yes | Incident readiness | Implemented | Incident response plan |
| A.5.25 Assessment and decision on information security events | Yes | Prioritises events | Implemented | Event triage workflow |
| A.5.26 Response to information security incidents | Yes | Mandatory for legal compliance | Implemented | Incident tickets |
| A.5.27 Learning from information security incidents | Yes | Supports continual improvement | Implemented | Post-incident review reports |
| A.5.28 Collection of evidence | Yes | Supports forensics and legal needs | Planned | Evidence handling procedure draft |
| A.5.29 Information security during disruption | Yes | Aligns with BCM | Implemented | BCM playbooks |
| A.5.30 ICT readiness for business continuity | Yes | Ensures technology resilience | In Progress | Disaster recovery test schedule |
| A.5.31 Legal, statutory, regulatory and contractual requirements | Yes | Compliance obligation | Implemented | Compliance register |
| A.5.32 Intellectual property rights | Yes | Protects IP of clients and company | Implemented | IP register, NDAs |
| A.5.33 Protection of records | Yes | Ensures record integrity | Implemented | Records management policy |
| A.5.34 Privacy and protection of PII | Yes | GDPR compliance | Implemented | Privacy framework, RoPA |
| A.5.35 Independent review of information security | Yes | Objective assessment of ISMS | Planned | Internal audit schedule |
| A.5.36 Compliance with policies and standards for information security | Yes | Monitoring adherence | Implemented | Compliance monitoring reports |
| A.5.37 Documented operating procedures | Yes | Ensures repeatable processes | Implemented | Procedural runbooks |
| A.6.1 Screening | Yes | Supplier vetting and personal screening | Implemented | Baseline screening records |
| A.6.2 Terms and conditions of employment | Yes | Contracts embed security obligations | Implemented | Employment contracts |
| A.6.3 Information security awareness, education and training | Yes | Essential for competence | In Progress | Training metrics |
| A.6.4 Disciplinary process | Yes | Enforces policy compliance | Implemented | Employee handbook |
| A.6.5 Responsibilities after termination or change of employment | Yes | Ensures obligations continue | Implemented | Offboarding acknowledgements |
| A.6.6 Confidentiality or non-disclosure agreements | Yes | Protects client data | Implemented | Executed NDAs |
| A.6.7 Remote working | Yes | Default operating model | Implemented | Remote working standard |
| A.6.8 Information security event reporting | Yes | All personnel must report issues | Implemented | Incident reporting procedure |
| A.7.1 Physical security perimeters | No | No dedicated corporate premises; home office assessed separately | Not Applicable | Home working risk assessment |
| A.7.2 Physical entry controls | No | No corporate offices managed by organisation | Not Applicable | Supplier facility attestations |
| A.7.3 Securing offices, rooms and facilities | No | Reliance on third-party managed office spaces | Not Applicable | Co-working agreements |
| A.7.4 Physical security monitoring | No | Physical monitoring handled by hosting suppliers | Not Applicable | Supplier SOC 2 reports |
| A.7.5 Protection against physical and environmental threats | No | No owned facilities; covered by cloud/data centre suppliers | Not Applicable | Supplier assurance pack |
| A.7.6 Security of assets off-premises | Yes | Laptops used remotely require controls | Implemented | Device management logs |
| A.7.7 Secure disposal or re-use of equipment | Yes | Laptops and storage devices need sanitisation | Implemented | Secure disposal certificates |
| A.7.8 Unattended user equipment | Yes | Home office operations | Implemented | Endpoint lock policy |
| A.7.9 Clear desk and clear screen | Yes | Prevents disclosure in shared workspaces | Implemented | User awareness materials |
| A.7.10 Working in secure areas | No | No secure areas under direct control | Not Applicable | Remote work procedures |
| A.7.11 Delivery and loading areas | No | No deliveries handled at corporate premises | Not Applicable | Supplier logistics clauses |
| A.7.12 Equipment siting and protection | Yes | Home office equipment placement | Implemented | Workspace assessments |
| A.7.13 Supporting utilities | No | No dedicated facilities; utilities managed by hosting providers | Not Applicable | Supplier DR evidence |
| A.7.14 Cabling security | No | No on-premise cabling infrastructure | Not Applicable | Cloud provider diagrams |
| A.8.1 User endpoint devices | Yes | Controls for laptops and mobile devices | Implemented | Endpoint management policy |
| A.8.2 Privileged access rights | Yes | Privileged roles restricted and monitored | Implemented | PAM reviews |
| A.8.3 Information access restriction | Yes | Enforces least privilege | Implemented | Access control configurations |
| A.8.4 Access to source code | Yes | Protects client and internal code assets | Planned | Repository access logs |
| A.8.5 Secure authentication | Yes | MFA and conditional access | Implemented | Authentication standards |
| A.8.6 Capacity management | Yes | Ensures SaaS services scale | Implemented | Service monitoring dashboards |
| A.8.7 Protection against malware | Yes | Windows Defender and policies | Implemented | Endpoint telemetry |
| A.8.8 Management of technical vulnerabilities | Yes | Weekly scans and patching | Implemented | Vulnerability reports |
| A.8.9 Configuration management | Yes | Baselines for servers and SaaS | In Progress | Configuration baselines |
| A.8.10 Information deletion | Yes | Secure erasure of data | In Progress | Deletion SOPs |
| A.8.11 Data masking | Yes | Protects sensitive data in lower environments | Planned | Masking design document |
| A.8.12 Data leakage prevention | Yes | Required for Restricted data | Planned | DLP roadmap |
| A.8.13 Information backup | Yes | Backups for critical data | Implemented | Backup logs |
| A.8.14 Redundancy of information processing facilities | Yes | Cloud resilience | Implemented | Microsoft 365 availability SLA |
| A.8.15 Logging | Yes | Capture security-relevant logs | Implemented | Log retention configuration |
| A.8.16 Monitoring activities | Yes | Continuous monitoring of alerts | Implemented | Security monitoring workbooks |
| A.8.17 Clock synchronization | Yes | Accurate time for forensics | Implemented | NTP configuration records |
| A.8.18 Use of privileged utility programs | Yes | Restricts admin tools | Implemented | Admin toolkit register |
| A.8.19 Installation of software on operational systems | Yes | Controls software changes | Implemented | Change management tickets |
| A.8.20 Network security | Yes | Protects network boundaries | Implemented | Firewall/M365 security settings |
| A.8.21 Security of network services | Yes | Ensures supplier-provided services secure | Implemented | Network service agreements |
| A.8.22 Segregation of networks | Yes | Separate production and admin networks | In Progress | Network segmentation plan |
| A.8.23 Web filtering | Yes | Prevents access to malicious sites | Implemented | Web filtering policy |
| A.8.24 Use of cryptography | Yes | Encryption for data at rest/in transit | Implemented | Encryption key inventory |
| A.8.25 Secure development life cycle | Yes | Project-based development requires SDLC | Planned | Secure SDLC framework |
| A.8.26 Application security requirements | Yes | Consulting deliverables may include tooling | Planned | Requirements catalogue |
| A.8.27 Secure system architecture and engineering principles | Yes | Guides solution design | In Progress | Architecture standards |
| A.8.28 Secure coding | Yes | Ensures developed scripts are secure | Planned | Coding standards draft |
| A.8.29 Security testing in development and acceptance | Yes | Validates deliverables | Planned | Test reports |
| A.8.30 Outsourced development | Yes | Third parties may develop assets | Planned | Supplier contracts |
| A.8.31 Separation of development, test and production environments | Yes | Avoids cross-environment risk | In Progress | Environment segregation plan |
| A.8.32 Change management | Yes | Controls changes to systems | Implemented | Change records |
| A.8.33 Test information | Yes | Protects test data | Implemented | Test data handling procedure |
| A.8.34 Protection of information systems during audit activities | Yes | Ensures audits do not impact operations | Implemented | Audit engagement guidelines |

## Maintenance

1. Update the SoA whenever new controls are implemented, risks change materially, or new services/contracts alter applicability.
2. Review and approve the SoA annually during the ISMS management review.
3. Link SoA updates to the risk register, treatment plan, and internal audit schedule.

## Accountable Roles and Decision Authority

1. **Director:** Owns and maintains this document, ensuring alignment with the Cyber Governance Policy and Document Control Policy.
2. **Director (Risk Owner):** Reviews and approves control applicability decisions, risk acceptances, and compensating controls.
3. **Director (Service Owner):** Coordinates evidence collection with suppliers and customers where controls impact external parties.

## Implementation Guidelines

1. Store evidence referenced in this SoA within the secure document repository with appropriate access controls.
2. Map control status changes to corrective and preventive actions and monitor through the CAPA register.
3. When controls are marked Not Applicable, retain supplier assurances or alternative control evidence supporting the decision.

## Revision History

| Version | Date | Description | Author |
| ------- | ---------- | ----------------------- | ------ |
| 3.0 | 2025-10-05 | Full population of ISO/IEC 27001:2022 control applicability table | Wayne Evans (Director) |
| 2.1 | 2025-10-05 | Author attribution updated | Wayne Evans (Director) |
| 2.0 | 2025-09-10 | Implementation guidelines added | Policy Team |
