# Employee Onboarding and Offboarding Policy

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
Establish controlled procedures to ensure new starters are integrated securely and leavers are removed from systems promptly, protecting company assets and meeting legal obligations.

## Scope
Applies to all employees, contractors and third parties who join or leave Cyber Ask Ltd.

## Policy
### 1. Onboarding
1.1 HR shall issue employment contracts and collect right to work documentation before start dates.
1.2 Line managers must submit access requests at least five working days before the start date specifying required systems and physical access.
1.3 HR shall initiate background screening within two working days of offer acceptance, in line with the Background Check Procedure and Legal and Regulatory Compliance Policy, ensuring checks comply with the Data Protection Act 2018 and Rehabilitation of Offenders Act 1974.
1.4 IT shall provision accounts with least privilege and record them in the access register no later than two working days before the start date.
1.5 New starters must complete induction training, Code of Conduct acknowledgment and security awareness training before being granted production system access.
1.6 Equipment must be asset-tagged, imaged according to the Secure Configuration Policy and issued against a signed receipt on day one.
1.7 Probation objectives shall be documented and reviewed at monthly intervals during the probation period.
1.8 HR shall maintain an onboarding checklist for each new hire and file it in the personnel record upon completion.

### 2. Offboarding
2.1 Line managers must notify HR of departures immediately upon resignation or termination and provide the last working day.
2.2 HR shall initiate the offboarding checklist and inform IT and Facilities within one working day.
2.3 IT shall disable system accounts, revoke credentials and remove access tokens no later than the employee’s final working day, with privileged access revoked within four hours of notification and all other access revoked within 24 hours post-termination.
2.4 Physical access cards, keys, ID badges and equipment must be returned before final payroll is released.
2.5 HR shall notify any managed service providers of the departure within one working day to trigger third-party access removal.
2.6 Exit interviews shall be conducted by HR to recover knowledge, confirm return of assets and remind leavers of ongoing confidentiality obligations under the Non-Disclosure Agreement and Data Protection Act.
2.7 Forwarding of emails and redirection of phone numbers shall be configured by IT for a maximum of 30 days unless otherwise approved.
2.8 Final pay, accrued holiday settlement and benefits termination shall be processed in accordance with the Employment Rights Act 1996.

### 3. Background Check Procedure Integration
1. Pre-employment screening levels shall be determined by role sensitivity and documented within the Background Check Procedure.
2. Checks may include identity verification, employment history, criminal record (where legally permissible) and professional qualifications.
3. Candidates must provide informed consent for all checks; results shall be stored securely and retained in line with the Records Retention Policy.
4. Any adverse findings will be assessed by HR and the Director, referencing the Legal and Regulatory Compliance Policy to ensure decisions are proportionate and legally defensible.

### 4. Onboarding and Offboarding Checklists

**Onboarding Checklist**

| Task | Owner | Target Timeline |
| ---- | ----- | --------------- |
| Issue contract and obtain signed acceptance | HR | Within 2 working days of verbal offer |
| Initiate background checks and right to work verification | HR | Within 2 working days of offer acceptance |
| Submit and approve access requests | Line Manager / Director | ≥5 working days pre-start |
| Build and configure equipment | IT | ≥3 working days pre-start |
| Conduct induction and mandatory training | HR / Director | Day 1 |
| Confirm probation objectives and mentor assignment | Line Manager | Week 1 |
| File completed onboarding pack in personnel record | HR | Within 5 working days of start |

**Offboarding Checklist**

| Task | Owner | Target Timeline |
| ---- | ----- | --------------- |
| Receive formal notification and confirm final working day | HR | Immediately on notification |
| Trigger access revocation request and disable privileged accounts | IT | Within 4 hours of notification |
| Collect company assets and revoke physical access | Facilities / HR | By final working day |
| Conduct exit interview and remind of confidentiality obligations | HR | Final working day |
| Remove remaining system access and update asset register | IT | Within 24 hours post-termination |
| Finalise payroll, benefits and documentation | HR / Finance | Within 5 working days post-termination |
| Archive completed offboarding checklist and evidence | HR | Within 10 working days post-termination |

### 5. Record Keeping and Auditing
5.1 Access provisioning and deprovisioning actions shall be logged and reviewed quarterly by the Director.
5.2 Onboarding and offboarding checklists must be retained for at least six years for audit purposes.
5.3 Any exceptions to the above procedures require written approval from the Director and HR.

## Roles and Responsibilities
1. **Human Resources:** Coordinate onboarding and offboarding, maintain records and ensure legal compliance.
2. **Line Managers:** Request and validate access requirements, ensure return of assets and complete checklists.
3. **IT Department:** Provision and revoke technical access, maintain asset inventory and log changes.
4. **Facilities:** Manage physical access cards and office equipment.

## Accountable Roles and Decision Authority

1. **Director:** Owns and maintains this policy, coordinates updates, and ensures alignment with the Cyber Governance Policy and Document Control Policy.
2. **Director (Risk Owner):** Reviews and approves exceptions, risk acceptances, and material control changes, documenting rationale in line with the Risk Management Policy.
3. **Director (Service Owner):** Oversees day-to-day execution of this policy, vendor engagement, and customer communications when actions affect external parties.


## Compliance
Failure to follow this policy may lead to disciplinary action and increased security risk. Regular audits shall verify adherence to ISO/IEC 27001 control A.7.1 and NCSC CAF principles.

## Review
This policy will be reviewed annually and after any significant organisational change.

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
