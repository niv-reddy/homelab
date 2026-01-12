# Enterprise Network Identity Security Platform

This directory contains the full Active Directory–centered network identity security platform used to design, enforce, monitor, and validate enterprise trust boundaries.  

---

## Directory Structure

| Folder | Description |
|------|------------|
| [`Identity Foundation`](./00-forest-baseline/) | Core Active Directory forest and identity platform baseline |
| [`Network Trust Zones`](./01-network-segmentation/) | VLANs, routing, and internal network segmentation |
| [`Trust Fabric Activation`](./02-trust-fabric-activation/) | Routed identity planes and enterprise system onboarding |
| [`Domain Hardening & Policy`](./02-hardening/) | GPO baselines, LAPS, and domain security policies |
| [`Security Monitoring & SIEM`](./04-detection/) | Logging, Wazuh, SIEM pipelines, and alerting |
| [`Adversary Emulation & Blue Team`](./05-adversary-simulation/) | Kali, attack chains, and red/blue team simulations |
