# Identity Foundation — Forest Baseline

This folder documents the foundational Active Directory forest that serves as the identity root of trust for the enterprise AD lab platform.

This baseline establishes the core authentication, authorization, and directory services infrastructure that all other platform layers depend on.

---

## Baseline Overview

| Component | Value |
|----------|-----|
| Forest / Domain | lab.niv.local |
| Primary Domain Controller | DC01 |
| Operating System | Windows Server 2022 |
| DNS | Active Directory Integrated |
| Kerberos Realm | LAB.NIV.LOCAL |
| Time Authority | DC01 (PDC Emulator) |
| Snapshot Baseline | AD-FOREST-GOLD-BASELINE |

---

## What This Baseline Provides

- Centralized authentication and authorization  
- Kerberos ticketing and secure service identity  
- Authoritative DNS and reverse lookup  
- SYSVOL and Group Policy replication  
- Tiered administrative security boundaries  
- Structured OU and security group architecture  
- Snapshot-protected rollback baseline  

---

## Status

**Baseline Complete and Production-Clean**

Core directory health, replication, Kerberos ticketing, DNS resolution, and time authority validation have all been verified.

Detailed step-by-step implementation documentation is maintained separately in formal Word/PDF documentation.

---

## Documentation

The formal design specification and authoritative implementation record for this baseline is maintained in the following document:

- [Identity Root of Trust Baseline Documentation (PDF)](./Identity-Root-of-Trust-Baseline.pdf/)

This document defines the trust boundary architecture, Kerberos realm establishment, DNS authority model, tiered administrative control structure, and security governance baseline for the enterprise identity platform.
