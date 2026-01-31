# Asset Register (Controlled Record)

**Record Owner:** Director (Risk Owner)  
**Applies To:** Cyber Ask Ltd information assets, infrastructure, software, and SaaS services  
**Last Review Date:** 2025-03-15  
**Next Review Date:** 2025-06-15  
**Related Policies & Registers:**
- [Data Classification Policy](../policies/information-security/data-classification-policy.md)
- [Master Risk Register](../Risk%20Assessments/master-risk-register.md)

## Asset Register

| Asset ID | Asset Name / Description | Asset Type (Hardware / Software / Data / Service) | Owner (Role / Department) | Custodian / Support Team | Information Classification | Lifecycle Status | Location / Hosting | Business Criticality | Dependencies | Backup / Recovery Details | Linked Risk Register Entries |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| HW-001 | Director primary laptop (BitLocker-encrypted endpoint) | Hardware | Director (IT/Admin) | Director | Internal | Active | Home office | High | Windows Defender, Microsoft 365 | OneDrive sync; weekly encrypted local backup | [R13](../Risk%20Assessments/master-risk-register.md#risk-register) – hardware supply delays; [R11](../Risk%20Assessments/master-risk-register.md#risk-register) – single-person dependency |
| HW-002 | Home office router/firewall and ISP modem | Hardware | Director (Operations) | ISP support + Director | Internal | Active | Home office | Medium | ISP link; power protection | ISP-managed recovery; config backup quarterly | [R14](../Risk%20Assessments/master-risk-register.md#risk-register) – power/fibre outage |
| SW-001 | Windows Server VM (domain controller synced to Entra ID) | Software | Director (IT) | Director | Confidential | Active | Local VM + Entra ID | High | Entra ID, endpoint protections | Weekly VM snapshot; recovery runbook | [R3](../Risk%20Assessments/master-risk-register.md#risk-register) – OAuth token theft; [R5](../Risk%20Assessments/master-risk-register.md#risk-register) – configuration drift |
| SaaS-001 | Microsoft 365 (Exchange, SharePoint, OneDrive) | Service (SaaS) | Director (Service Owner) | Microsoft support + Director | Confidential / Restricted | Active | Microsoft 365 cloud | High | Entra ID, MFA | Microsoft retention + OneDrive sync | [R2](../Risk%20Assessments/master-risk-register.md#risk-register) – ransomware; [R3](../Risk%20Assessments/master-risk-register.md#risk-register) – token theft |
| Data-001 | Client assessment deliverables repository (reports, evidence packs) | Data | Director (Data Owner) | Director | Restricted | Active | SharePoint + encrypted local storage | High | Microsoft 365; BitLocker | Encrypted backup set; retention schedule | [R4](../Risk%20Assessments/master-risk-register.md#risk-register) – prompt injection; [R19](../Risk%20Assessments/master-risk-register.md#risk-register) – retention lapses |
| SaaS-002 | Risk register workspace (Microsoft Lists + Power BI dashboard) | Service (SaaS) | Director (Risk Owner) | Director | Confidential | Active | Microsoft 365 cloud | Medium | Microsoft 365 | Daily Microsoft 365 retention | [R12](../Risk%20Assessments/master-risk-register.md#risk-register) – reporting failure; [R20](../Risk%20Assessments/master-risk-register.md#risk-register) – governance drift |

## Asset Lifecycle Notes

| Asset ID | Event (Acquisition / Update / Decommission) | Description | Date | Authorised By |
| --- | --- | --- | --- | --- |
| HW-001 | Update | Endpoint replaced with new laptop; legacy device securely wiped | 2025-02-01 | Director |
| SW-001 | Update | Entra ID sync hardening and baseline review | 2025-02-15 | Director |
| SaaS-001 | Update | MFA baseline and conditional access policy review | 2025-03-01 | Director |
| Data-001 | Update | Review of classification labels per policy | 2025-03-10 | Director |

## Linkage Notes

- Asset classifications above follow the [Data Classification Policy](../policies/information-security/data-classification-policy.md) and are reviewed at least annually or when data sensitivity changes.
- Risk references link to the [Master Risk Register](../Risk%20Assessments/master-risk-register.md) entries that require tracking when asset criticality or control maturity changes.
