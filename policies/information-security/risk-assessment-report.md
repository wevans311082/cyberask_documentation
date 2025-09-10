# Risk Assessment Report

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** WEvans Director

This report summarizes the results of the latest information security risk assessment in accordance with ISO 27001.

## Overview

- **Assessment Date:** <DATE>
- **Assessed By:** Information Security Officer and designated risk owners.

## Key Findings

- Document high and medium risks with descriptions of assets, threats, and vulnerabilities.
- Provide likelihood and impact ratings and reference supporting evidence.

## Recommendations

- Outline proposed treatments for each significant risk.
- Identify risks accepted by management and justification.

## Approval

Management reviews and approves this report and associated treatment decisions.

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
