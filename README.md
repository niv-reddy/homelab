# Homelab Setup

This repository documents my personal homelab build, starting with a full home network infrastructure upgrade. Each subfolder contains detailed setup documentation for a specific component of the lab.

---

## Contents

| Folder | Description |
|--------|-------------|
| [`Home Network/`](./home-network-upgrade/) | Full Home Network Upgrade:<br>- Mesh setup<br>- Crimping<br>- Switch<br>- Structured documentation |
| [`DNS/`](./DNS/) | Centralized DNS Control Plane using AdGuard:<br>- Role-based policy enforcement<br>- Telemetry suppression<br>- Zero Trust device segmentation |
| [AD Lab/](./enterprise-identity-network-security-lab/) | Enterprise Identity & Security Platform:<br>- Immutable AD forest root of trust (lab.niv.local)<br>- Tiered admin model (Tier 0/1/2) with OU & security group control planes<br>- Segmented trust zones through VLAN (Servers / Workstations / Security)<br>- Hardened domain baselines (GPO, LAPS, access restrictions)<br>- SIEM-ready logging & detection engineering (Wazuh)<br>- Adversary emulation & blue-team simulation framework<br>- Snapshot-anchored recovery & reproducible build layers |
