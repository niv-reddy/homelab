# 🌐 Home Network Setup

## 🔧 Overview
Upgraded my home network from a basic ISP router/modem combo to a wired-backhauled mesh system using Eero. All Ethernet ports were pre-run by the builder, then manually crimped and tested.

---

## 🛠️ Hardware
- **ISP Modem:** Xfinity Gateway (set to bridge mode)
- **Mesh System:** Eero 6+ (3 nodes total)
- **Switch:** TP-Link 8-Port Gigabit Unmanaged
- **Cabling:** In-wall CAT6 terminated with keystone jacks

---

## 🧱 Network Layout
- Modem → Main Eero Gateway → Switch
- Switch → Wall jacks → Secondary Eeros (wired backhaul)
- Devices connect to nearest Eero — mostly over Ethernet

---

## ⚙️ Configuration Highlights
- **Bridge Mode:** Enabled on ISP gateway
- **DNS:** Cloudflare (1.1.1.1 / 1.0.0.1)
- **UPnP:** Disabled
- **Guest Network:** Isolated via Eero app
- **Speed Test Results:**  
  - ~500+ Mbps wired  
  - ~300–400 Mbps wireless

---

## 🧪 Notes & Tools
- Crimped using T568B standard
- Tested each run with **Klein Scout Pro 3**
- Verified switch backhaul links via Eero app + speed testing

---

## 📸 Diagrams / Visuals *(To be added)*
- Network layout sketch
- Ethernet port map
- Crimping setup

---

Let me know if you want to add:
- Actual test results (Speedtest image, iperf output)
- Photos or diagrams (I can help format those)
