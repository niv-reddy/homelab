# Pi-hole DNS Filtering Setup

This subproject documents the deployment of a Pi-hole DNS filtering system in a home network environment. Pi-hole acts as a local DNS sinkhole, providing network-wide ad blocking, domain filtering, and DNS query monitoring.

## 📦 Overview

- Deployed on a Raspberry Pi 4 (8GB) with passive cooling and wired Ethernet
- Integrated with Eero mesh system via custom DNS settings
- Secure SSH access with public key authentication
- Uses Cloudflare (1.1.1.1) as upstream DNS provider
- Web admin dashboard for real-time monitoring and list management

## 📁 Documentation

- **[Pi-hole Setup Documentation (PDF)](./Pihole_Setup_Documentation.pdf)** – Full step-by-step process including hardware configuration, OS flashing, Pi-hole install, and Eero integration
- **[`Network Diagram (PNG)`](./assets/network-topology-diagram.png)** – Visual representation of DNS flow and device topology
- **Filtering Behavior** – Explanation of blocklists, DNS resolution, and common blocked domains (e.g. `iadsdk.apple.com`, trackers)

## 🛠️ Next Steps

- Enable DNS over HTTPS (DoH) or DNS over TLS (DoT)
- Expand filtering policies per-device using DHCP + tagging (future)
- Compare Pi-hole to pfBlockerNG or enterprise DNS solutions
