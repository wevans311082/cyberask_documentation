# Access Control Policy

**Company:** Cyber Ask Ltd (CYBER ASK LTD), Registered No. 15113248  
**Author:** WEvans Director

This policy establishes comprehensive requirements for granting, reviewing, and revoking access to information systems so that only authorized individuals perform approved activities. It aligns with ISO/IEC 27001 and other regulatory frameworks, providing a control environment that protects confidentiality, integrity, and availability of organizational assets.

## Purpose

The purpose of this policy is to define a consistent and auditable process for managing access to company resources. It ensures that access rights are granted based on legitimate business needs, remain commensurate with job responsibilities, and are removed promptly when no longer required. The policy also seeks to minimize security risks posed by excessive or outdated privileges.

## Scope

This policy applies to all employees, contractors, consultants, partners, and temporary staff who use or manage company information systems. It covers every system, application, database, network device, and cloud service that stores, processes, or transmits organizational information, regardless of location or hosting arrangement. Third-party service providers must adhere to equivalent access controls as a condition of their engagement.

## Definitions

- **Access Rights:** The specific permissions granted to a user to read, modify, execute, or delete information or resources.
- **Least Privilege:** The principle that users should be granted only the minimum access necessary to perform their duties.
- **Multi-factor Authentication (MFA):** A security mechanism requiring two or more verification methods to authenticate a user.
- **Privileged Account:** An account with elevated permissions that can modify system configurations or access restricted data.

## Policy Statements

1. **Account Provisioning**
   - Managers must submit documented access requests through the approved ticketing system.
   - IT will create accounts with unique user IDs and verify managerial approval prior to granting access.
   - Temporary accounts shall include an expiration date not exceeding 30 days unless renewed.

2. **Access Modification**
   - Any change to a user’s role or responsibilities requires a reassessment of existing access rights.
   - Managers and system owners must validate requests for additional permissions and ensure they align with business needs.

3. **Access Reviews**
   - Managers must conduct access reviews at least quarterly to confirm continued necessity of privileges.
   - Results of access reviews shall be documented and retained for a minimum of three years.
   - Internal audit may perform independent spot checks of user access to verify compliance.

4. **Access Revocation**
   - HR will notify IT of employee departures or role changes immediately upon confirmation.
   - IT shall disable associated accounts within one business day of notification.
   - Physical access devices (badges, keys, tokens) must be returned or deactivated on termination.

5. **Privileged Access Management**
   - Administrative accounts must use MFA and are restricted to authorized personnel with demonstrated need.
   - Privileged sessions shall be logged and monitored for anomalous activity.
   - Shared privileged accounts are prohibited unless technically unavoidable, in which case compensating controls such as password vaulting must be implemented.

6. **Password Management**
   - Passwords must meet complexity requirements defined by the company’s password standard and be changed at least every 90 days.
   - Reuse of the previous 12 passwords is prohibited.
   - Default passwords on new systems must be changed before deployment and never used in production environments.

7. **Separation of Duties**
   - No single individual should be able to develop, approve, and deploy changes to production systems without oversight.
   - Access granting functions must be segregated from approval functions to prevent abuse.

8. **Third-Party Access**
   - External vendors or partners requiring system access must sign appropriate agreements and comply with this policy.
   - Accounts for third parties shall be time-bound and reviewed before renewal.

## Roles and Responsibilities

- **IT Department:** Implements technical controls, maintains audit logs, and enforces provisioning and revocation procedures. IT is responsible for monitoring privileged activities and reporting suspected violations.
- **Managers and System Owners:** Initiate access requests, perform periodic access reviews, and ensure that staff receive appropriate security training.
- **Human Resources:** Communicates staffing changes that affect access and coordinates offboarding activities.
- **Internal Audit:** Performs independent assessments of access control effectiveness and reports findings to management.
- **Users:** Maintain the confidentiality of their credentials, follow approved procedures, and report suspected account misuse.

## Monitoring and Enforcement

- All access to critical systems must be logged and retained according to the company’s data retention schedule.
- Security operations will review logs for suspicious activity and escalate incidents per the incident response plan.
- Alleged access control violations will be documented and investigated with HR following the [Disciplinary Policy for Security Breaches](../hr/disciplinary-policy-for-security-breaches.md), including timely evidence preservation and interviews with relevant personnel.
- Violations of this policy may result in disciplinary action up to and including termination, civil liability, or criminal prosecution. Individuals retain the right to appeal decisions using the process defined in the [Grievance Policy](../hr/grievance-policy.md).

## Training and Awareness

- All users must complete annual security awareness training that covers secure authentication practices, proper handling of credentials, and reporting procedures for suspected access violations.
- IT shall provide targeted training for administrators on privileged account management tools and procedures.

## Access Control Technologies

- Systems handling sensitive information must implement industry-standard authentication mechanisms such as LDAP, SAML, or OAuth2.
- Wherever feasible, single sign-on (SSO) shall be used to centralize authentication and streamline account management.
- Encryption must protect authentication data in transit and at rest, and default system credentials shall be changed prior to production use.

## Exceptions

- Exceptions to this policy require a documented risk assessment and written approval from the Chief Information Security Officer (CISO) or delegate. Approved exceptions must include compensating controls and an expiration date.

## Compliance and Review

This policy is reviewed at least annually or upon significant system changes to ensure ongoing effectiveness and alignment with legal, regulatory, and contractual requirements. Compliance with this policy supports relevant ISO/IEC 27001 controls, including A.9 Access Control, and may be audited at management’s discretion.

## Revision History

| Version | Date       | Description             | Author |
| ------- | ---------- | ----------------------- | ------ |
| 1.0     | 2023-01-01 | Initial policy release  | IT     |
| 2.0     | 2025-09-10 | Comprehensive expansion | IT     |
| 3.0     | 2025-09-10 | Implementation guidelines added | Policy Team |

## Implementation Guidelines
- All requests and approvals must be tracked in the ServiceDesk system.
- Data at rest must use AES-256 encryption; data in transit must use TLS 1.2+ with perfect forward secrecy.
- Security events shall log to the central SIEM and be retained for 12 months.
- Control owners perform quarterly self-assessments; Information Security conducts annual audits.
- Exceptions require written CISO approval and must include compensating controls.

