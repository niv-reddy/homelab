# Enterprise Network Identity Security Platform

This directory contains the full Active Directory–centered network identity security platform used to design, enforce, monitor, and validate enterprise trust boundaries.  

---

## Directory Structure

| Folder | Description |
|------|------------|
| [`Identity Foundation`](./00-forest-baseline/) | Core Active Directory forest, DNS, Kerberos, and tiered identity baseline |
| [`Network Trust Zones`](./01-network-segmentation/) | VLAN segmentation and physical isolation of server, workstation, and security zones |
| [`Trust Fabric Activation`](./02-trust-fabric-activation/) | Routed identity rails and onboarding of domain workloads through Firewall |
| [`Domain Hardening & Policy`](./03-domain-hardening/) | Authentication hardening, tier enforcement, and post-compromise containment |
| [`Security Monitoring & SIEM`](./04-detection/) | Logging, Wazuh, SIEM pipelines, and alerting |
| [`Adversary Emulation & Blue Team`](./05-adversary-simulation/) | Kali, attack chains, and red/blue team simulations |
