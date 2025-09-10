# Data Classification Policy

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** WEvans Director

This policy establishes a framework for classifying and handling information based on sensitivity, aligning with CE/CE+ and ISO 27001 requirements.

## Classification Levels

1. **Public:** Information approved for external release.
2. **Internal:** Information intended for employees and authorized partners.
3. **Confidential:** Sensitive business data requiring restricted access.
4. **Restricted:** Highly sensitive data such as personal or financial information; access is strictly controlled.

## Handling Requirements

- Label documents and systems with appropriate classification.
- Encrypt confidential and restricted data at rest and in transit.
- Share restricted data only with authorized individuals under NDA.
- Dispose of physical and electronic media according to classification level.

## Roles and Responsibilities

- **Data Owners:** Determine classification and handling requirements.
- **Users:** Follow handling requirements and report misclassification.
- **IT:** Provide technical controls to enforce classifications.

## Review

Classifications are reviewed annually or when significant changes in data usage occur.

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
