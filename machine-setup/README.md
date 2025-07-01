🖥️ Ubuntu Homelab Machine Setup

This subproject documents the process of setting up my main Ubuntu homelab machine using a dual-boot configuration with Windows and secure remote SSH access

📄 Included
- **[`Homelab Setup Documentation (PDF)`](./HomeLab-Setup.pdf)**  – Full walkthrough covering installation, user setup, SSH configuration, remote access via Eero, and hardening tips.

🛠️ Highlights
- Dual-boot configuration: Ubuntu installed alongside Windows
- Created bootable USB with balenaEtcher
- Minimal Ubuntu install with third-party media & driver support
- Custom hostname and username
- SSH setup with key-based authentication and custom port
- Eero port forwarding configured for secure remote access
- Hardened sshd_config: disabled password login, enforced key auth, allowed only specific user

🔐 Remote Access
- SSH key-based login from Mac laptop
- Remote access via custom Eero domain
- Confirmed working access over mobile hotspot and other networks

🧩 Next Steps
- Begin installing core homelab services (Docker, file server, monitoring stack, etc.)
- Set up auto-start services and system monitoring tools
- Integrate with Active Directory and local DNS where applicable
