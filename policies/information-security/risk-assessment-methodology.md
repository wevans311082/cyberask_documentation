# Risk Assessment Methodology

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** Wayne Evans (Director)

This document describes the systematic approach for identifying, analyzing, and evaluating information security risks in compliance with ISO 27001.

## Cyber Ask Operating Context

1. Cyber Ask Ltd operates with a single employee who also serves as the sole director responsible for governance, risk, and compliance decisions.
2. Cyber Ask Ltd maintains professional liability insurance covering its consulting and advisory services.
3. A dedicated virtual machine functions as the single Windows Server domain controller and is synchronized with Microsoft Entra ID for identity management.
4. The organisation holds a standard Microsoft 365 licence; Microsoft Purview and Microsoft Defender add-ons are not deployed, and Windows Defender provides endpoint protection.
5. Customer data is stored on BitLocker-encrypted drives to protect information at rest.
6. Cyber Ask Ltd assets are vulnerability-assessed weekly and patched promptly according to remediation guidance.
7. Cyber Ask Ltd has not yet achieved Cyber Essentials, Cyber Essentials Plus, or ISO 27001 certification but aligns its controls with those standards where practicable.
8. The Director personally fulfils HR, IT administration, and compliance duties, engaging specialist suppliers when additional expertise is required.



## Method

The methodology follows an Identify → Analyse → Evaluate → Treat (IAET) cycle supported by the enterprise risk register.

1. **Identify**  
   a. Catalogue business processes, information assets, supporting technology, and data flows using the asset inventory.  
   b. Assign asset owners and capture confidentiality, integrity, and availability (CIA) requirements.  
   c. Link assets to legal, regulatory, and contractual obligations (e.g., UK GDPR, client SLAs).
2. **Analyse**  
   a. Identify threats, vulnerabilities, and existing controls using sources such as threat intelligence feeds, vulnerability scans, and audit findings.  
   b. Estimate inherent likelihood and impact using the 5x5 scoring matrix defined in the Risk Management Policy.  
   c. Where data is available, perform quantitative analysis (e.g., estimating annualised loss expectancy) and record assumptions in the risk register.
3. **Evaluate**  
   a. Compare inherent risk scores against tolerance thresholds (Low/Moderate/High/Critical).  
   b. Determine residual risk after considering existing controls, evidencing effectiveness through control testing results.  
   c. Decide whether to accept, mitigate, transfer, or avoid the risk; document rationale and required approvals in the register workflow.
4. **Treat**  
   a. Define treatment actions, owners, costs, and due dates.  
   b. Update the risk treatment plan and integrate actions with the CAPA register and project backlog.  
   c. Monitor treatment progress monthly and reassess residual risk upon completion or significant change.

### Quantitative Example – Monte Carlo Simulation

For high-impact risks (residual score ≥16) the Director performs or commissions a Monte Carlo simulation to stress-test financial exposure:

1. Identify probability distributions for key variables (e.g., frequency of credential compromise per year, average incident response cost).  
2. Use a minimum of 10,000 iterations to simulate annual loss expectancy.  
3. Record mean, median, 95th percentile, and worst-case outcomes in the risk register, attaching calculation worksheets.  
4. Compare simulated outcomes against cyber insurance limits and business continuity impact tolerances to inform acceptance or further treatment decisions.  
5. Update the Statement of Applicability and control assurance plan where additional controls are required to reduce tail risk.

### Integration with the Enterprise Risk Register

1. All risk records are created and maintained in the enterprise risk register (current platform: Microsoft Lists with Power BI dashboard).  
2. Each risk entry must include asset linkage, regulatory obligations, scoring rationale, treatment status, and evidence references.  
3. Automated workflows notify risk owners of overdue actions and escalate critical risks to the Director for decision within five working days.  
4. Risk metrics feed into management review meetings, the Statement of Applicability, and customer assurance reports.

## Frequency

1. Conduct a comprehensive assessment annually and after significant changes to systems or processes.

## Recording Results

1. Document findings in the Risk Assessment Report, including risk owners and treatment decisions.

## Approval

The Director approves the methodology and reviews it annually.

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
