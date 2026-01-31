# Risk Assessment Report

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** Wayne Evans (Director)

This report summarizes the results of the latest information security risk assessment in accordance with ISO 27001.

## Cyber Ask Operating Context

1. Cyber Ask Ltd operates with a single employee who also serves as the sole director responsible for governance, risk, and compliance decisions.
2. Cyber Ask Ltd maintains professional liability insurance covering its consulting and advisory services.
3. A dedicated virtual machine functions as the single Windows Server domain controller and is synchronized with Microsoft Entra ID for identity management.
4. The organisation holds a standard Microsoft 365 licence; Microsoft Purview and Microsoft Defender add-ons are not deployed, and Windows Defender provides endpoint protection.
5. Customer data is stored on BitLocker-encrypted drives to protect information at rest.
6. Cyber Ask Ltd assets are vulnerability-assessed weekly and patched promptly according to remediation guidance.
7. Cyber Ask Ltd has not yet achieved Cyber Essentials, Cyber Essentials Plus, or ISO 27001 certification but aligns its controls with those standards where practicable.
8. The Director personally fulfils HR, IT administration, and compliance duties, engaging specialist suppliers when additional expertise is required.



## Overview

1. **Assessment Date:** 2025-03-12
2. **Assessed By:** Wayne Evans (Director) with supplier input for Microsoft 365 and managed service providers.
3. **Assessment Scope:** Corporate information assets, Microsoft 365 tenant, Windows Server domain controller, consulting deliverables, and supplier-managed SaaS services.

## Key Findings

The following risks align to the master risk register and ISO/IEC 27001:2022 Statement of Applicability control decisions.

| Risk ID | Assets at Risk | Threat | Vulnerability | Likelihood | Impact | Owner | SoA Control Linkages |
| --- | --- | --- | --- | --- | --- | --- | --- |
| R1 | Client deliverables, advisory reports, AI tooling | Malicious AI model update poisoning outputs | Limited third-party assurance of model update pipelines | 3 | 5 | Director | A.5.19, A.5.21, A.8.25 |
| R2 | Microsoft 365 backups, SharePoint sites | Double-extortion ransomware | Limited immutable backup configuration options in standard M365 licence | 3 | 5 | Director | A.5.24, A.8.13, A.8.16 |
| R3 | Microsoft Entra ID tenant, user sessions | Adversary-in-the-middle phishing stealing OAuth tokens | Conditional access gaps and limited phishing-resistant MFA | 3 | 4 | Director | A.5.17, A.8.5, A.8.16 |
| R4 | Confidential assessment data, client workpapers | Prompt injection into generative AI tooling | Inconsistent prompt hygiene and client data segregation | 4 | 4 | Director | A.5.10, A.5.12, A.8.11 |
| R5 | Microsoft 365 tenant configuration, storage | Cloud configuration drift exposing data | Limited automated configuration monitoring | 3 | 4 | Director | A.8.9, A.8.16, A.8.20 |
| R6 | Microsoft Teams add-ins, endpoint devices | Zero-day exploitation of add-ins | Dependence on vendor patch cycle | 2 | 4 | Director | A.8.8, A.8.19, A.8.20 |
| R7 | Finance workflows, client invoices | Deepfake-enabled business email compromise | Single approver workflows and limited out-of-band verification | 3 | 3 | Director | A.5.2, A.5.15, A.8.2 |
| R8 | Microsoft 365 tenant, supplier integrations | Managed service provider compromise | Shared admin access and limited supplier assurance reviews | 2 | 5 | Director | A.5.19, A.5.22, A.8.21 |
| R9 | Vulnerability scanning scripts, automation | Supply-chain tampering introducing backdoors | Limited code signing and integrity checks | 2 | 4 | Director | A.8.28, A.8.31, A.8.32 |
| R10 | Archived client data | Quantum-capable decryption | Long-term retention of encrypted archives | 2 | 5 | Director | A.8.24, A.8.13, A.8.27 |
| R11 | Incident response, change approvals | Single-person dependency | Lack of documented deputies | 3 | 3 | Director | A.5.2, A.5.24, A.6.3 |
| R12 | Compliance evidence repository | Reporting failure | Manual evidence tracking and fragmented storage | 2 | 3 | Director | A.5.33, A.5.37, A.8.15 |
| R14 | Home office connectivity, service delivery | Power/fibre outage | Single internet provider and limited redundancy | 3 | 3 | Director | A.5.29, A.5.30, A.8.14 |

## Recommendations

1. Prioritise treatment actions for R1, R2, R4, and R5 due to their high inherent impact and exposure across client deliverables.
2. Implement supplier assurance cadence (A.5.21, A.5.22) and update contractual clauses for AI and managed service providers to reduce R1 and R8.
3. Strengthen identity protections with phishing-resistant MFA and session controls to reduce R3.
4. Formalise prompt hygiene controls and data segregation for AI tooling to reduce R4.
5. Introduce configuration monitoring baselines and alerting for cloud configuration drift to reduce R5.
6. Develop documented deputy coverage and cross-training to address R11.
7. Accept residual risk for R10 once PQC transition roadmap is approved and aligned with client contracts.

## Approval

Management reviews and approves this report and associated treatment decisions.

**Approval Date:** 2025-03-15  
**Approved By:** Wayne Evans (Director)

## Accountable Roles and Decision Authority

1. **Director:** Owns and maintains this policy, coordinates updates, and ensures alignment with the Cyber Governance Policy and Document Control Policy.
2. **Director (Risk Owner):** Reviews and approves exceptions, risk acceptances, and material control changes, documenting rationale in line with the Risk Management Policy.
3. **Director (Service Owner):** Oversees day-to-day execution of this policy, vendor engagement, and customer communications when actions affect external parties.


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
| 2.2     | 2025-03-15 | Populated assessment with assets, threats, ratings, and ownership | Wayne Evans (Director) |
