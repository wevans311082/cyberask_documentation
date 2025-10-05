# Cyber Ask Ltd Enterprise Cyber Security Risk Assessment 2025

## 1. Context

| Item | Details |
| --- | --- |
| Assessment Name | Cyber Ask Ltd Annual Cyber Security Risk Assessment |
| Business Function / Process | End-to-end operations covering consulting delivery, Microsoft 365 collaboration, Windows Server domain services, AI-assisted analysis workflows, and customer data handling |
| Assessment Trigger (project, change, review) | Annual enterprise review in accordance with the Risk Management Policy and ISO/IEC 27001 alignment objectives |
| Prepared By | Director (Risk Owner) |
| Date Initiated | 2025-02-14 |
| Review Cycle | Annual, or upon material change to infrastructure, services, threat landscape, or regulatory obligations |

## 2. Scope and Assumptions

- **In-Scope Assets / Services:**
  - Microsoft 365 tenant providing email, collaboration, and identity synchronisation with Microsoft Entra ID.
  - Windows Server domain controller virtual machine hosting Active Directory services.
  - BitLocker-encrypted laptops, removable storage, and collaboration tooling supporting customer deliverables.
  - AI/LLM-enabled analysis pipelines that incorporate third-party and open-source models.
  - Vulnerability scanning, secure coding scripts, and automation used to support client engagements.
  - Contracts and data processed for client engagements retained for a minimum of six years.
- **Excluded Items:**
  - Client-managed environments where Cyber Ask Ltd provides advisory services only.
  - Third-party SaaS platforms used ad-hoc for client collaboration subject to their own risk assessments.
- **Assumptions / Dependencies:**
  - Single-employee operating model centralises risk ownership and requires strict change management discipline.
  - Microsoft 365 standard licence limits availability of advanced Microsoft Defender and Purview tooling; compensating controls are required.
  - Weekly vulnerability assessments and rapid patching continue as documented in existing security policies.
  - Threat intelligence from trusted sources (NCSC, CISA, MITRE, ENISA, commercial reports) is reviewed monthly to identify emerging risks.

## 3. Risk Matrix (define scoring reference)

| Likelihood Score | Description |
| --- | --- |
| 1 | Rare – Exceptional circumstances only |
| 2 | Unlikely – Could occur at some time |
| 3 | Possible – Might occur at least annually |
| 4 | Likely – Expected to occur multiple times per year |
| 5 | Almost Certain – Expected to occur frequently |

| Impact Score | Description |
| --- | --- |
| 1 | Negligible – Minimal impact, easily contained |
| 2 | Minor – Limited operational disruption |
| 3 | Moderate – Noticeable service impact or regulatory concern |
| 4 | Major – Significant disruption, reportable breach likely |
| 5 | Severe – Critical failure, substantial legal/financial penalties |

## 4. Top 10 Risk Register (2025 Focus)

| Risk ID | Threat Scenario | Threat Intelligence Sources | Impacted Assets / Processes | Existing Controls | Likelihood | Impact | Inherent Risk (L x I) | Additional Controls / Actions | Control Owner | Target Date | Residual Risk |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| R1 | Malicious or poisoned AI model updates compromise analysis outputs supplied to clients | MITRE ATLAS 2025 updates; ENISA AI Threat Landscape 2024 | AI-assisted analysis workflows; client deliverable repositories | Manual code review of models; supplier due diligence; controlled distribution channels | 3 | 5 | 15 | Require supplier attestations, hash validation, and sandbox evaluation prior to deployment (Action R1-A1, R1-A2) | Director | 2025-07-31 | 8 |
| R2 | Ransomware with data theft targets Microsoft 365 and Azure backups, threatening double extortion | CrowdStrike Global Threat Report 2025; Microsoft Digital Defense Report 2024 | Microsoft 365 tenant; backup storage; client data | MFA enforced; BitLocker; weekly vulnerability scans; offline copy of key data | 3 | 5 | 15 | Deploy immutable backups, ASR policies, and rehearsed ransomware response playbook (Actions R2-A1, R2-A2) | Director | 2025-05-31 | 9 |
| R3 | Adversary-in-the-middle phishing steals OAuth tokens and session cookies to bypass MFA | CISA AA24-241A; Mandiant M-Trends 2024 | Microsoft Entra ID; Microsoft 365 services; client collaboration spaces | MFA with number matching; baseline conditional access; awareness training | 3 | 4 | 12 | Expand conditional access with device compliance, phishing-resistant MFA, and real-time token revocation (Actions R3-A1, R3-A2) | Director | 2025-06-30 | 6 |
| R4 | Prompt injection and data exfiltration through generative AI assistants and plugins | OWASP Top 10 for LLM Applications 2023; NCSC Secure AI System Development Guidance 2024 | AI assistant integrations; client data sets; knowledge bases | Prompt libraries; limited dataset exposure; manual review of AI outputs | 4 | 4 | 16 | Implement content filters, request isolation, and red-teaming for AI workflows (Actions R4-A1, R4-A2) | Director | 2025-09-30 | 8 |
| R5 | Cloud misconfiguration or drift exposes SharePoint/OneDrive sites or Azure storage publicly | IBM X-Force Threat Intelligence Index 2024; Wiz State of Cloud 2024 | Microsoft 365 collaboration data; Azure storage | Baseline configuration guides; monthly manual review; Secure Score tracking | 3 | 4 | 12 | Automate baseline scanning, integrate IaC validation, and document remediation SLAs (Actions R5-A1, R5-A2) | Director | 2025-06-30 | 6 |
| R6 | Zero-day vulnerability in Microsoft Teams or productivity add-ins exploited before patch release | CISA KEV Catalog 2024; Google TAG Quarterly 2024 | Microsoft Teams; integrated third-party apps; user endpoints | Rapid patching; Defender AV; application allow-listing pilots | 2 | 4 | 8 | Subscribe to rapid threat intelligence feeds, enable attack surface reduction rules, and rehearse virtual patching (Actions R6-A1, R6-A2) | Director | 2025-08-31 | 4 |
| R7 | Deepfake-enabled social engineering leading to business email compromise and fraudulent payments | FBI IC3 2024; Europol 2024 Internet Organised Crime Assessment | Finance workflows; accounts payable processes; executive communications | Out-of-band payment verification; awareness training; monitoring of finance mailbox rules | 3 | 3 | 9 | Deploy voice verification callbacks, DMARC enforcement, and finance-specific simulation exercises (Actions R7-A1, R7-A2) | Director | 2025-07-31 | 5 |
| R8 | Managed service provider or SaaS partner compromise enables lateral movement into Cyber Ask tenant | NCSC/CISA Advisory AA24-046A; BlackBerry Global Threat Intelligence Report 2024 | Third-party integrations; delegated admin portals; secure file transfer services | Contractual security clauses; manual access reviews; privileged identity management | 2 | 5 | 10 | Formalise third-party assurance programme and enforce just-in-time access (Actions R8-A1, R8-A2) | Director | 2025-10-31 | 6 |
| R9 | Post-quantum capable adversaries harvest encrypted archives for future decryption | NIST PQC Readiness Update 2024; NSA CNSA 2.0 guidance 2024 | Archived client data; long-term contracts; secure communications | TLS 1.2+; BitLocker full disk encryption; key rotation every 12 months | 2 | 5 | 10 | Develop crypto-agility roadmap, inventory algorithms, and pilot PQC solutions (Actions R9-A1, R9-A2) | Director | 2026-03-31 | 6 |
| R10 | Regional cloud outage or major SaaS disruption halts access to collaboration platforms | Azure Service Reliability Reports 2024; Gartner 2025 Cloud Risk Trends | Microsoft 365; ticketing and metrics tooling; client reporting dashboards | Documented manual fallback; alternate communication channels; local cache of key data | 3 | 3 | 9 | Expand continuity playbooks, test failover communications, and stage offline work kits (Actions R10-A1, R10-A2) | Director | 2025-05-31 | 5 |

## 5. Risk Acceptance and Treatment Decisions

| Risk ID | Decision (Accept / Mitigate / Transfer / Avoid) | Decision Rationale | Approver | Approval Date |
| --- | --- | --- | --- | --- |
| R1 | Mitigate | Supplier attestation, sandbox validation, and monitoring materially reduce the likelihood of AI model compromise. | Director | 2025-02-14 |
| R2 | Mitigate | Immutable backups and ASR controls offer cost-effective protection compared with ransomware impact. | Director | 2025-02-14 |
| R3 | Mitigate | Enhanced conditional access and phishing-resistant authentication are feasible and align with policy requirements. | Director | 2025-02-14 |
| R4 | Mitigate | Investment in AI security controls is necessary to maintain client trust and comply with data protection duties. | Director | 2025-02-14 |
| R5 | Mitigate | Automation of baseline checks reduces manual effort and addresses recurring misconfiguration findings. | Director | 2025-02-14 |
| R6 | Mitigate | Rapid threat intelligence integration and ASR coverage balance cost with heightened threat activity. | Director | 2025-02-14 |
| R7 | Mitigate | Additional verification and monitoring controls prevent financial loss from deepfake-enabled fraud. | Director | 2025-02-14 |
| R8 | Mitigate | Strengthened third-party assurance and access restrictions reduce exposure from MSP compromises. | Director | 2025-02-14 |
| R9 | Mitigate | Early quantum readiness actions support regulatory guidance and long-term confidentiality obligations. | Director | 2025-02-14 |
| R10 | Mitigate | Continuity enhancements are proportionate to service reliance on hyperscale SaaS providers. | Director | 2025-02-14 |

## 6. Review and Closure

- **Follow-up Actions Tracked In:** Master Risk Register and risk treatment plan with linkage to Corrective and Preventive Action log.
- **Next Scheduled Review:** 2026-02-14 or sooner following significant technology, supplier, or regulatory changes.
- **Additional Notes:** Risk treatment progress will be reviewed monthly in conjunction with vulnerability management, AI governance, and policy compliance checks to evidence alignment with ISO/IEC 27001, NCSC CAF, and evolving AI assurance expectations.
