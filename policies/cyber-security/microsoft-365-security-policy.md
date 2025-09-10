# Microsoft 365 Security Policy

## Purpose

This policy defines security and compliance requirements for the organization's Microsoft 365 (M365) environment to protect data, manage risk, and meet regulatory obligations.

## Scope

This policy applies to all Microsoft 365 services, accounts, and devices used to access corporate data.

## Policy

1. The organization shall configure the Microsoft 365 tenant in accordance with Microsoft's security baseline and review Secure Score at least quarterly.
2. Conditional Access policies shall enforce multi-factor authentication and device compliance for all M365 access.
3. Data loss prevention, retention, and sensitivity labels shall be implemented using Microsoft Purview.
4. Microsoft Defender for Office 365 and Microsoft Defender for Endpoint shall be enabled and integrated with central monitoring.
5. Audit logs from Microsoft 365 shall be collected and retained in accordance with the Logging and Monitoring Policy.

## Technical Controls

- Enable Microsoft Entra ID Conditional Access to require MFA and block legacy authentication.
- Use Intune to manage and enforce device compliance for endpoints accessing M365.
- Configure Microsoft Purview DLP, retention, and sensitivity labels to protect and govern data.
- Integrate Microsoft Defender for Office 365 and Defender for Endpoint for threat protection and automatic response.
- Forward M365 audit logs and alerts to the centralized logging platform.

## Roles and Responsibilities

- **Employees and Contractors:** Use Microsoft 365 services in accordance with this policy and report security issues.
- **Management:** Provide resources to implement and maintain required Microsoft 365 controls.
- **Security and Compliance Teams:** Configure, monitor, and improve Microsoft 365 security settings and respond to incidents.

## Compliance

Failure to comply with this policy may result in disciplinary action and could expose the organization to legal or regulatory penalties.

## Review

This policy will be reviewed at least annually or upon significant changes to Microsoft 365 services or organizational requirements.

