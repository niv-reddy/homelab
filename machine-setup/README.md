🖥️ Ubuntu Homelab Machine Setup

This subproject documents the process of setting up my main Ubuntu homelab machine using a dual-boot configuration with Windows and secure remote SSH access

📄 Included
- **[homelab-setup.pdf](./Homelab-Setup.pdf)**  – Full walkthrough covering installation, user setup, SSH configuration, remote access via Eero, and hardening tips.

🛠️ Highlights
- Dual-boot configuration: Ubuntu installed alongside Windows
- Created bootable USB with balenaEtcher
- Minimal Ubuntu install with third-party media & driver support
- Custom hostname: niv-homelab and user: nreddy
- SSH setup with key-based authentication and custom port (2222)
- Eero port forwarding configured for secure remote access
- Hardened sshd_config: disabled password login, enforced key auth, allowed only specific user

🔐 Remote Access
- SSH key-based login from Mac laptop
- Public IP access via Eero’s pXXXXXXX.eero.online domain
- Confirmed working access over mobile hotspot (work Wi-Fi restrictions present)
- Tailscale VPN was tested but removed for simplification

🧩 Next Steps
- Begin installing core homelab services (Docker, file server, monitoring stack, etc.)
- Set up auto-start services and system monitoring tools
- Integrate with Active Directory and local DNS where applicable
