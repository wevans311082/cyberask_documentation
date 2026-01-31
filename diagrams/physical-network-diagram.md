# Physical Network Diagram

## Overview
The physical network diagram reflects hardware, connectivity, and hosting boundaries, including the domain controller VM, endpoints, and remote access path.

```mermaid
flowchart TB
    Internet((Internet))
    ISP[ISP Modem/Router]
    Firewall[Firewall / Secure Gateway]
    Hypervisor[Host Device
    (VM hypervisor)]
    DCVM[Windows Server DC VM]
    Endpoint1[Director Laptop]
    Endpoint2[Admin Workstation]
    VPN[Remote Access VPN]
    Cloud[Microsoft 365/Entra Cloud]

    Internet --> ISP --> Firewall
    Firewall --> Hypervisor
    Hypervisor --> DCVM
    Firewall --> Endpoint1
    Firewall --> Endpoint2
    Firewall --> VPN

    VPN --> Firewall
    Firewall --> Cloud
    Endpoint1 --> Cloud
    Endpoint2 --> Cloud
```

## Key Notes
- The domain controller VM runs on a secured hypervisor host behind the firewall.
- Endpoints connect through the secure gateway for internal services and cloud services.
- Remote access terminates at the VPN gateway before reaching internal resources.

## Update Trigger
Update this diagram after any material change to physical devices, hosting location, or remote access infrastructure.

## Revision Log
| Version | Date       | Description                                   | Author |
| ------- | ---------- | --------------------------------------------- | ------ |
| 1.0     | 2026-01-31 | Initial physical network diagram created.     | Policy Team |
