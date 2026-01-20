# Domain Hardening — Identity Defense Control Plane

This folder documents the **domain hardening and identity defense layer** of the **lab.niv.local** enterprise platform.

This layer transforms the Active Directory environment from a functional directory service into a **cryptographically enforced and post-compromise resilient identity platform**.  
It hardens authentication, enforces tiered privilege boundaries, and aligns identity controls with network trust zones.

This is the layer where the identity fabric becomes **defensible infrastructure**.

---

## What This Layer Provides

- Cryptographically enforced authentication (AES-only Kerberos)  
- Removal of legacy authentication and relay paths  
- Tier-restricted logon across workstations, servers, and PAW  
- Privileged Access Workstation as the sole Tier-0 entry point  
- Local administrator governance through Restricted Groups  
- Post-compromise containment aligned with VLAN trust zones  
- Deterministic privilege boundaries between Tier 0 / 1 / 2  

---

## Active Control Planes

| Control Plane | Scope | Purpose |
|---------------|-------|---------|
| Auth Hardening | Domain | Modern authentication and anti-relay enforcement |
| T0 Logon Restrictions | DCs & PAW | Tier-0 credential confinement |
| T1 Logon Restrictions | Servers | Server admin tier isolation |
| T2 Logon Restrictions | Workstations | Endpoint tier isolation |
| T1T2 Mgmt Path Restriction | Servers & Workstations | Endpoint firewall posture and admin path alignment |
| T1 Server Local Admin | Servers | Tier-aligned local admin governance |
| T2 Local Admin Control | Workstations | Workstation admin governance |
| SEC Attack Surface Reduction | Endpoints | Post-compromise behavior reduction |


---

## Validation State

**Identity Defense Layer Active and Enforced**

- Kerberos operating exclusively with modern encryption  
- NTLM constrained and observable  
- SMB and LDAP relay vectors blocked  
- Tier-based logon boundaries enforced  
- PAW enclave established and protected  
- Workstation → server administrative paths denied  
- Local administrator roles governed by domain identity  

---

## Documentation

Formal implementation and verification documentation:

- [Domain Hardening Documentation (PDF)](./Domain-Hardening.pdf)

This document defines authentication hardening controls, tier enforcement design, local admin governance, network alignment, and validation evidence for the identity defense platform.

---