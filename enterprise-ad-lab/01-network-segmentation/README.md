# Network Segmentation — Trust Zone Fabric

This folder documents the internal enterprise network segmentation layer of the lab.niv.local platform.

This layer establishes physical Layer-2 trust boundaries between infrastructure systems, user endpoints, and security tooling.  
It forms the first enforced lateral-movement control surface and becomes the foundation that all firewalling, routing, detection engineering, and adversary simulation layers will later depend on.

---

## Segmentation Overview

| Component | Value |
|---------|------|
| Segmentation Fabric | Proxmox vmbr1 (VLAN-aware trunk) |
| Enforcement Layer | Hypervisor Layer-2 VLAN segmentation |
| Routing Model | None (sealed trust zones) |
| Lateral Movement | Physically blocked |
| Isolation Method | VLAN tagging and bridge enforcement |

---

## Trust Zone Model

| Trust Zone | VLAN | CIDR | Purpose |
|----------|-----|------|--------|
| Server Trust Zone | 10 | 10.0.10.0/24 | Tier-0 identity and core infrastructure |
| Workstation Trust Zone | 20 | 10.0.20.0/24 | User endpoints and client systems |
| Security / Admin Trust Zone | 30 | 10.0.30.0/24 | Security tooling and privileged administration |

---

## What This Layer Provides

• Physical lateral-movement prevention  
• Hard separation of enterprise trust zones  
• Enforced security boundaries at Layer-2  
• Controlled foundation for firewall routing design  
• Segmented attack-surface modeling  
• Deterministic trust-plane isolation  

---

## Status

Segmentation Fabric Active and Enforced

Server and Workstation Trust Zones are fully segmented and sealed.  
No routing exists between VLANs.  
Layer-2 isolation has been verified and is operational.

---

## Documentation

Formal implementation and validation records are maintained in:

**Network Segmentation Documentation (PDF)**

This document defines the segmentation architecture, VLAN fabric design, trust zone classification, isolation validation, and enforcement boundaries for the enterprise lab platform.
