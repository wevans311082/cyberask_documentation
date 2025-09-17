# Risk Assessment Methodology

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** WEvans Director

This document describes the systematic approach for identifying, analyzing, and evaluating information security risks in compliance with ISO 27001.

## Method

1. **Asset Identification:** Compile an inventory of information assets, owners, and locations.
2. **Threat and Vulnerability Identification:** Determine potential threats and vulnerabilities for each asset.
3. **Risk Analysis:** Evaluate likelihood and impact using a qualitative scale of Low, Medium, High.
4. **Risk Evaluation:** Compare risks against predefined acceptance criteria to prioritize treatment.

## Frequency

- Conduct a comprehensive assessment annually and after significant changes to systems or processes.

## Recording Results

- Document findings in the Risk Assessment Report, including risk owners and treatment decisions.

## Approval

The Information Security Officer approves the methodology and reviews it annually.

## Accountable Roles and Decision Authority

- **Policy Owner (Information Security Manager):** Maintains this policy, coordinates updates, and ensures alignment with the Cyber Governance Policy and Document Control Policy.
- **Chief Information Security Officer (CISO):** Approves exceptions, risk acceptances, and material control changes in line with the Information Security Policy and Risk Management Policy.
- **Risk and Compliance Committee:** Reviews escalated risks, endorses significant remediation decisions, and provides oversight consistent with the Risk Management Policy.
- **Executive Leadership Team:** Ratifies budgetary or strategic decisions related to this policy as defined in the Cyber Governance Policy.

Exception requests must follow the exception management process described in the Cyber Governance Policy and all approvals must be recorded in accordance with the Document Control Policy.


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
