# Logical Network Diagram

## Overview
The logical network diagram captures identity, endpoint, and remote-access flows across Cyber Ask Ltd systems, including Microsoft 365/Entra, the Windows Server domain controller VM, and managed endpoints.

```mermaid
flowchart TB
    Internet((Internet))
    M365[Microsoft 365 Services]
    Entra[Microsoft Entra ID]
    VPN[Remote Access VPN]
    DCVM[Windows Server Domain Controller VM]
    Endpoints[Corporate Endpoints
    (Director laptop, admin workstation)]
    SaaS[Third-Party SaaS Apps]

    Internet --> M365
    Internet --> SaaS
    Internet --> VPN

    M365 <--> Entra
    Entra <--> DCVM
    DCVM --> Endpoints

    VPN --> DCVM
    VPN --> Endpoints

    Endpoints --> M365
    Endpoints --> SaaS
```

## Key Notes
- Microsoft Entra ID synchronises identities with the Windows Server domain controller VM.
- Remote access is brokered through VPN with MFA and least-privilege access to internal resources.
- Endpoints access Microsoft 365 services over encrypted channels and are protected by Windows Defender.

## Update Trigger
Update this diagram after any material change to identity architecture, remote access, or endpoint inventory.

## Revision Log
| Version | Date       | Description                                  | Author |
| ------- | ---------- | -------------------------------------------- | ------ |
| 1.0     | 2026-01-31 | Initial logical network diagram created.     | Policy Team |
