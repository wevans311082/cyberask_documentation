# Cyber Ask Ltd Enterprise Cyber Security Risk Assessment 2025

## 1. Context

| Item | Details |
| --- | --- |
| Assessment Name | Cyber Ask Ltd Annual Cyber Security Risk Assessment |
| Business Function / Process | End-to-end operations covering consulting delivery, Microsoft 365 collaboration, Windows Server domain services, and customer data handling |
| Assessment Trigger (project, change, review) | Annual enterprise review in accordance with the Risk Management Policy and ISO/IEC 27001 alignment objectives |
| Prepared By | Director (Risk Owner) |
| Date Initiated | 2025-02-14 |
| Review Cycle | Annual, or upon material change to infrastructure, services, or regulatory obligations |

## 2. Scope and Assumptions

- **In-Scope Assets / Services:**
  - Microsoft 365 tenant providing email, collaboration, and identity synchronisation with Microsoft Entra ID.
  - Windows Server domain controller virtual machine hosting Active Directory services.
  - BitLocker-encrypted laptops and removable storage handling customer deliverables.
  - Vulnerability scanning tooling and patch management processes.
  - Contracts and data processed for client engagements retained for a minimum of six years.
- **Excluded Items:**
  - Client-managed environments where Cyber Ask Ltd provides advisory services only.
  - Third-party SaaS platforms used ad-hoc for client collaboration subject to their own risk assessments.
- **Assumptions / Dependencies:**
  - Single-employee operating model centralises risk ownership and requires strict change management discipline.
  - Microsoft 365 standard licence limits availability of advanced Microsoft Defender and Purview tooling; compensating controls are required.
  - Weekly vulnerability assessments and rapid patching continue as documented in existing security policies.

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

## 4. Risk Register

| Risk ID | Threat / Vulnerability Description | Impacted Assets / Processes | Existing Controls | Likelihood | Impact | Inherent Risk (L x I) | Additional Controls / Actions | Control Owner | Target Date | Residual Risk |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| R1 | Compromise of Microsoft 365 or Entra ID credentials through phishing or password spraying due to limited advanced detection licences | Microsoft 365 tenant, identity services, client data stored in SharePoint/OneDrive | MFA enforced for all accounts, conditional access baseline, security awareness training, Windows Defender anti-phishing | 3 | 4 | 12 | Deploy conditional access policies for geolocation and device compliance, enable number matching for MFA, acquire Defender for Office P1 or configure third-party phishing detection with daily review, run simulated phishing quarterly | Director | 2025-06-30 | 6 |
| R2 | Ransomware infection on Windows Server domain controller disrupting identity services and client deliverables | Windows Server VM, BitLocker laptops, customer deliverables | Weekly vulnerability scans, Windows Defender real-time protection, BitLocker encryption, offline backup rotation | 3 | 5 | 15 | Implement immutable cloud backups, configure ASR rules, document and test ransomware response playbook, enable application whitelisting via Windows Defender Application Control | Director | 2025-05-31 | 9 |
| R3 | Data loss or unavailability due to failed backup or retention processes for project files and emails | Customer data repositories, contractual records | Manual weekly backups, retention schedule aligning to six-year requirement, change management approvals for backup jobs | 2 | 4 | 8 | Automate backup verification reports, integrate backup job alerts into monitoring dashboard, maintain quarterly restore tests with evidence, document retention exceptions | Director | 2025-04-30 | 4 |
| R4 | Supplier or specialist subcontractor breach leading to exposure of shared client information | Supplier collaboration workflows, NDA processes | NDA and contractual clauses, third-party access control policy, manual due diligence checks | 2 | 4 | 8 | Formalise supplier security questionnaire, require documented security attestations annually, maintain register of third-party access reviews, enforce secure file transfer tooling | Director | 2025-07-31 | 6 |
| R5 | Single-person dependency causing delays or errors in change management and incident response | Change management process, service delivery | Change Management Policy, documented SOPs, calendar reminders for reviews | 3 | 3 | 9 | Implement peer review via trusted partner for high-risk changes, adopt ticketing system for change tracking, schedule quarterly external audit of critical procedures | Director | 2025-08-31 | 6 |
| R6 | Misconfiguration of cloud services due to lack of centralised configuration baselines | Microsoft 365 security settings, Azure AD configuration | CIS benchmark references, manual monthly reviews, baseline hardening guides | 3 | 4 | 12 | Deploy configuration-as-code baseline documentation, use Microsoft Secure Score with monthly evidence capture, adopt automated configuration drift reporting via baseline scripts, align to NCSC CAF objectives | Director | 2025-06-30 | 6 |

## 5. Risk Acceptance and Treatment Decisions

| Risk ID | Decision (Accept / Mitigate / Transfer / Avoid) | Decision Rationale | Approver | Approval Date |
| --- | --- | --- | --- | --- |
| R1 | Mitigate | Enhanced conditional access and phishing detection are feasible within budget and reduce likelihood materially | Director | 2025-02-14 |
| R2 | Mitigate | Cost of immutable backup subscription and ASR configuration acceptable versus operational impact of ransomware | Director | 2025-02-14 |
| R3 | Mitigate | Automation and testing reduce dependency on manual checks while meeting legal retention requirements | Director | 2025-02-14 |
| R4 | Mitigate | Formal supplier assurance protects shared data and supports contractual obligations | Director | 2025-02-14 |
| R5 | Mitigate | External oversight and tooling strengthen governance without adding staff | Director | 2025-02-14 |
| R6 | Mitigate | Automated baselines and Secure Score monitoring align with policy requirements and standards | Director | 2025-02-14 |

## 6. Review and Closure

- **Follow-up Actions Tracked In:** Master Risk Register and ticketing system (to be implemented) with linkage to Corrective and Preventive Action log.
- **Next Scheduled Review:** 2026-02-14 or sooner following significant technology or regulatory changes.
- **Additional Notes:** Risk treatment progress will be reviewed monthly in conjunction with vulnerability management and policy compliance checks to evidence alignment with ISO/IEC 27001 and NCSC CAF requirements.
