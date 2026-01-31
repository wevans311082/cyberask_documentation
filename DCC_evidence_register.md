# DCC Evidence Register

This register lists evidence artefacts supporting Defence Cyber Compliance (DCC) control requirements. Evidence owners must ensure artefacts are current and linked to the latest control expectations.

## Evidence Register

| Evidence ID | Control Reference | Evidence Description | Location | Owner | Update Trigger |
| ----------- | ----------------- | -------------------- | -------- | ----- | -------------- |
| DCC-1203-01 | 1203 / 1203.1 | Logical network diagram (M365/Entra, DC VM, endpoints, remote access). | `diagrams/logical-network-diagram.md` | Director | Update after material change to identity, remote access, or endpoint architecture. |
| DCC-1203-02 | 1203 / 1203.1 | Physical network diagram (hosting, endpoints, remote access path). | `diagrams/physical-network-diagram.md` | Director | Update after material change to physical devices, hosting, or remote access infrastructure. |
| DCC-2500-01 | 2500 / 2500.2 | Network resilience policy evidence and supporting artefacts. | `policies/cyber-security/network-security-policy.md` | Director | Update after policy revision or material control change. |

## Update Trigger
Update this register after any material change to DCC evidence, diagrams, or supporting policies.

## Revision Log
| Version | Date       | Description                                   | Author |
| ------- | ---------- | --------------------------------------------- | ------ |
| 1.0     | 2026-01-31 | Initial DCC evidence register created.        | Policy Team |
