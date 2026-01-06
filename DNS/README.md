# DNS Layer

This directory contains all DNS-related infrastructure and policy enforcement systems used in the homelab network.

DNS is treated as a control plane for outbound traffic rather than a simple name resolution service. All devices resolve DNS through one of the platforms documented in this folder, enabling centralized filtering, telemetry suppression, and role-based policy enforcement.

## Directory Structure

```
dns/
├── pihole/     # Legacy DNS filtering deployment (deprecated)
├── adguard/    # Active DNS enforcement and Zero Trust policy platform
└── README.md   # This file
```

## Purpose

This layer provides:

- Centralized DNS resolution  
- Outbound domain control  
- Telemetry and tracking suppression  
- Role-based DNS policy enforcement  
- Centralized logging and visibility  

Pi-hole represents the original DNS filtering deployment.  
AdGuard Home is the current and actively maintained DNS policy enforcement platform.
