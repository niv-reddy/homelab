# DNS Layer

This directory contains all DNS-related infrastructure and policy enforcement systems used in the homelab network.

DNS is treated as a control plane for outbound traffic rather than a simple name resolution service. All devices resolve DNS through one of the platforms documented in this folder, enabling centralized filtering, telemetry suppression, and role-based policy enforcement.

## Directory Structure

| Folder | Description |
|--------|-------------|
| [`pihole/`](./pihole/) | Legacy Pi-hole DNS filtering deployment (deprecated) |
| [`adguard/`](./adguard/) | Active Zero Trust DNS policy enforcement layer using AdGuard Home |


## Purpose

This layer provides:

- Centralized DNS resolution  
- Outbound domain control  
- Telemetry and tracking suppression  
- Role-based DNS policy enforcement  
- Centralized logging and visibility  

Pi-hole represents the original DNS filtering deployment.  
AdGuard is the current and actively maintained DNS policy enforcement platform.
