# GDPR and UK Data Protection Act Policy

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
This policy establishes requirements for complying with the UK General Data Protection Regulation (UK GDPR), the EU GDPR where applicable, and the UK Data Protection Act 2018 (DPA 2018). It ensures personal data is processed lawfully, fairly, and transparently while protecting the rights of data subjects and supporting contractual and regulatory obligations.

## Scope
This policy applies to all employees, contractors, suppliers, and third parties who create, collect, store, access, transmit, or otherwise process personal data on behalf of Cyber Ask Ltd. It covers all processing performed within the UK and processing of EU personal data when Cyber Ask Ltd is subject to EU GDPR extraterritorial provisions.

## Definitions
- **Personal Data:** Any information relating to an identified or identifiable natural person.
- **Special Category Data:** Personal data revealing racial or ethnic origin, political opinions, religious beliefs, trade union membership, genetic or biometric data, health data, or data concerning a person’s sex life or sexual orientation.
- **Controller:** The natural or legal person that determines the purposes and means of processing personal data.
- **Processor:** A natural or legal person that processes personal data on behalf of the controller.
- **Data Subject:** An individual whose personal data is processed by Cyber Ask Ltd.

## Policy

### Lawfulness, Fairness, and Transparency
1. Processing must be based on a documented lawful basis (consent, contract, legal obligation, vital interests, public task, or legitimate interests) recorded in the [Records of Processing Policy](records-of-processing-policy.md) and related registers.
2. Privacy notices shall be maintained and made available prior to data collection, clearly describing purposes, retention, rights, and contact points for the Data Protection Officer (DPO).
3. For processing based on consent, Cyber Ask Ltd must obtain explicit, informed, and freely given consent that can be withdrawn at any time.

### Purpose Limitation and Data Minimisation
1. Personal data must be collected for specified, explicit, and legitimate purposes and not further processed in a manner incompatible with those purposes unless permitted by law.
2. Personnel must only collect the minimum data necessary to achieve documented processing purposes and must avoid storing redundant or excessive personal data.
3. Special category data requires documented necessity, additional safeguards, and reliance on DPA 2018 Schedule 1 conditions.

### Accuracy and Storage Limitation
1. Personal data must be accurate and kept up to date; inaccurate data shall be rectified or erased without undue delay when notified.
2. Retention periods are defined in the [Records Management and Archiving Policy](records-management-and-archiving-policy.md) and the Records of Processing Activities (RoPA). Data exceeding the defined retention period must be securely deleted or anonymised.

### Integrity and Confidentiality
1. Technical and organisational controls including encryption, access controls, secure configuration, and monitoring must be implemented per the [Data Protection and Privacy Policy](../cyber-security/data-protection-and-privacy-policy.md) and supporting security standards.
2. Personal data transfers must utilise secure channels such as TLS 1.2+ or approved file transfer solutions, and data at rest must be protected using BitLocker or equivalent encryption.
3. Third parties handling personal data on behalf of Cyber Ask Ltd must sign data processing agreements (DPAs) defining responsibilities, security measures, and audit rights.

### Accountability and Governance
1. The DPO maintains the RoPA, DPIA register, and evidence of lawful bases, ensuring records are accurate and available for inspection by the Information Commissioner’s Office (ICO).
2. Data Protection Impact Assessments (DPIAs) must be completed for processing that is likely to result in a high risk to the rights and freedoms of individuals using the [DPIA Template](../../templates/dpia-template.md).
3. Annual privacy compliance reviews evaluate adherence to this policy, legal developments, and effectiveness of implemented controls. Findings and remediation actions are captured within the compliance management system.

### Data Subject Rights Management
1. Procedures must exist to authenticate and respond to data subject requests (DSRs) for access, rectification, erasure, restriction, portability, and objection within one month, extendable by two months for complex requests.
2. The DPO maintains a request log capturing receipt, verification, fulfilment actions, and justification for any refusal. Decisions are documented and retained for a minimum of six years.
3. Where processing is automated, individuals must be informed of meaningful logic involved, significance, and consequences, and provided mechanisms for human review upon request.

### International Transfers
1. Personal data may only be transferred outside the UK or EU when adequate safeguards exist, such as UK adequacy regulations, EU adequacy decisions, International Data Transfer Agreements (IDTAs), or Standard Contractual Clauses (SCCs) with Transfer Risk Assessments.
2. The DPO maintains an inventory of cross-border transfers, safeguards applied, and review dates. Transfers lacking sufficient safeguards require Director approval and documented compensating controls.

### Incident Response and Breach Notification
1. Suspected personal data breaches must be reported immediately to the DPO and handled in accordance with the [Incident Response Plan](../cyber-security/incident-response-plan.md).
2. The DPO assesses breach severity and determines whether notification to the ICO is required within 72 hours and whether affected individuals must be informed without undue delay.
3. Breach records including cause, scope, remediation, and notification decisions must be retained for six years.

### Training and Awareness
1. All personnel must complete privacy and data protection training upon onboarding and annually thereafter, covering GDPR principles, handling procedures, and breach reporting.
2. Targeted training is required for roles handling special category data, conducting DPIAs, or managing DSRs.

## Technical Controls
1. Access to personal data repositories must be governed by least privilege, multi-factor authentication, and regular access reviews.
2. Encryption keys and secrets supporting personal data protection must be managed per the [Cryptography and Key Management Policy](../cyber-security/cryptography-and-key-management-policy.md).
3. Automated data loss prevention (DLP) and audit logging capabilities are configured within Microsoft 365 and endpoint tooling where available; gaps are documented with compensating controls.

## Roles and Responsibilities
1. **Director / Data Protection Officer:** Owns this policy, maintains compliance evidence, responds to ICO communications, and ensures timely completion of DPIAs and DSRs.
2. **Employees and Contractors:** Follow privacy procedures, complete required training, and promptly escalate suspected breaches or DSRs.
3. **Suppliers and Processors:** Implement contractual safeguards, restrict processing to documented instructions, and support audits or assurance requests.

## Accountable Roles and Decision Authority
1. **Director:** Approves new processing activities, international transfers, and processor engagements after reviewing DPIAs and contractual safeguards.
2. **Director (Risk Owner):** Evaluates residual privacy risks, approves risk acceptances, and coordinates remediation tracking.
3. **Director (Service Owner):** Ensures operational procedures for data protection remain effective, including training updates and technical control maintenance.

## Compliance
Failure to comply with this policy may result in disciplinary action, contractual penalties, or enforcement action by the ICO or other supervisory authorities.

## Review
This policy will be reviewed at least annually and upon significant changes to applicable data protection legislation, regulatory guidance, or business operations.

## Revision History
| Version | Date       | Description | Author |
| ------- | ---------- | ----------- | ------ |
| 1.0     | 2025-10-06 | Initial policy release covering GDPR and UK DPA compliance requirements. | Wayne Evans (Director) |
