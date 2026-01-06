# AdGuard  DNS Control Plane

This folder contains the active DNS enforcement platform for the homelab network, implemented using AdGuard.

AdGuard functions as the centralized DNS control plane for all internal devices. It enforces role-based DNS policy, telemetry suppression, and conditional filtering across a mixed-trust environment.

This deployment replaces the legacy Pi-hole based DNS filtering platform.

---

## Environment

- Deployed as a Linux container (LXC) within Proxmox  
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

**[`AdGuard Documentation (PDF)`](./AdGuard_Documentation.pdf)** – Full step-by-step process including hardware configuration, OS flashing, Pi-hole install, and Eero integration

---

AdGuard Home is the active DNS policy enforcement platform for the network.
