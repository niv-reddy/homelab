# Enterprise Active Directory Lab

This directory contains the full Active Directory–based identity and security lab platform.  
It is organized into modular layers so each component of the environment can be documented, rebuilt, and extended independently.

---

## Directory Structure

| Folder | Description |
|------|------------|
| [`Identity Foundation`](./00-forest-baseline/) | Core Active Directory forest and identity platform baseline |
| [`Network Trust Zones`](./01-segmentation/) | VLANs, routing, and internal network segmentation |
| [`Domain Hardening & Policy`](./02-hardening/) | GPO baselines, LAPS, and domain security policies |
| [`Enterprise Workloads`](./03-workloads/) | File servers, workstations, and application servers |
| [`Security Monitoring & SIEM`](./04-detection/) | Logging, Wazuh, SIEM pipelines, and alerting |
| [`Adversary Emulation & Blue Team`](./05-adversary-simulation/) | Kali, attack chains, and red/blue team simulations |

---