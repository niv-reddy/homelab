# Trust Fabric Activation — Routed Identity Plane

This folder documents the activation of the routed identity trust fabric for the **lab.niv.local** enterprise platform.

This layer transitions the environment from isolated segmentation into a controlled, identity-aware routed security fabric.  
It introduces domain-joined systems, firewall-enforced inter-zone communication, and the first operational identity trust plane.

This is the layer where the forest baseline becomes *operational infrastructure*.

---

## Current Activated Systems

| System | Zone | VLAN | Purpose |
|-------|----|----|--------|
| DC01 | Server Trust Zone | 10 | Primary domain controller, DNS, Kerberos authority |
| FS01 | Server Trust Zone | 10 | Enterprise file server and workload platform |
| WIN10-01 | Workstation Trust Zone | 20 | User endpoint and policy enforcement target |
| pfSense FW | Routing Core | Backbone | Inter-zone trust enforcement point |

---

## What This Layer Provides

- Routed trust enforcement between VLAN trust zones  
- Identity-aware traffic control through firewall policy  
- Domain join activation for enterprise workloads and endpoints  
- Kerberos-validated authentication across routed boundaries  
- DNS authority enforcement from server trust zone  
- First controlled lateral-movement surface  

This layer converts segmentation into a functioning **enterprise trust fabric**.

---

## Trust Fabric Control Model

| Trust Plane | Allowed To |
|-----------|-----------|
| Workstation Zone (VLAN20) | Authenticate to Domain Controllers only |
| Server Zone (VLAN10) | Provide identity, file, and infrastructure services |
| Security/Admin Zone (VLAN30) | Observe, manage, and simulate activity (Not completed at this stage) |
| All Zones | Must pass through routed firewall enforcement |

---

## Validation State

**Trust Fabric Activated and Enforced**

- Domain join verified for all applicable systems  
- Kerberos ticket issuance validated  
- DNS resolution enforced across zones  
- Firewall policy controls validated  
- Inter-zone lateral movement constrained  
- Identity trust plane operational  

---

## Documentation

Formal implementation and verification documentation:

**Trust Fabric Activation Documentation (PDF)**

This document defines routed trust architecture, firewall enforcement models, inter-zone authentication flows, and validation evidence for the enterprise trust fabric.

---

## What This Means

At this point the environment is no longer a segmented lab.

It now operates as a real enterprise security platform with:

- A centralized identity root of trust  
- Routed trust boundaries  
- Controlled authentication flows  
- Enforced lateral movement constraints  
- An operational enterprise security fabric  

This platform now supports hardening, detection engineering, and adversary simulation.
