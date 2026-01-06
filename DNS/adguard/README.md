# AdGuard Home DNS Control Plane

This folder contains the active DNS enforcement platform for the homelab network, implemented using AdGuard Home.

AdGuard Home functions as the centralized DNS control plane for all internal devices. It enforces role-based DNS policy, telemetry suppression, and conditional filtering across a mixed-trust environment.

This deployment replaces the legacy Pi-hole based DNS filtering platform.

---

## Environment

- Deployed as a virtual machine within Proxmox  
- Authoritative DNS resolver for all LAN devices  
- Uses privacy-focused upstream DNS providers  
- Centralized DNS logging and monitoring via web dashboard  

---

## Documentation

Full architecture and configuration documentation is maintained separately and stored in this folder:

- Design and enforcement model  
- Zero Trust architecture  
- Device classification and policy model  
- Operational behavior and monitoring  

Refer to the documentation files in this directory for full implementation details.

---

## Folder Contents

| Path | Description |
|-----|------------|
| `/architecture/` | Design diagrams and enforcement flow |
| `/policies/` | Conditional DNS policy rules |
| `/inventory/` | Device inventory and role mappings |
| `/screenshots/` | Runtime enforcement and metrics evidence |
| `/docs/` | Full configuration and design documentation |

---

AdGuard Home is the active DNS policy enforcement platform for the network.
