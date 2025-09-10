# Encryption Policy

This policy defines the requirements for encrypting sensitive information to protect confidentiality and integrity in line with CE/CE+ and ISO 27001 controls.

## Purpose
Ensure appropriate cryptographic safeguards are applied to data at rest and in transit.

## Scope
All systems, applications, and devices that store or transmit company data.

## Policy
- **Standards:** Use industry-accepted algorithms such as AES-256 for data at rest and TLS 1.2 or higher for data in transit.
- **Key Management:** Encryption keys must be stored securely, rotated annually, and access limited to authorized personnel.
- **Mobile Devices:** Portable media and laptops must employ full-disk encryption.
- **Cloud Services:** Enable encryption features provided by cloud vendors and manage keys under company control.
- **Exception Handling:** Any deviations require documented approval and compensating controls.

## Roles and Responsibilities
- **IT Security:** Defines approved cryptographic standards and manages key infrastructure.
- **System Owners:** Implement encryption according to this policy.
- **Users:** Protect passwords and report potential compromises.

## Review
This policy is reviewed annually or when new cryptographic standards emerge.
