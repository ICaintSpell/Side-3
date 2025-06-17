# 🧱 Homelab SIEM/SOC Setup with OpenVPN Integration

Welcome to the ultimate guide for building a feature-rich, cybersecurity-focused homelab that simulates a real-world Security Operations Center (SOC). This setup includes:

- 🔐 **pfSense Firewall**  
- 🌐 **OpenVPN for secure remote access**  
- 🛡 **Suricata IDS/IPS**  
- 📊 **Splunk SIEM**  
- ☁️ **Azure Sentinel integration**  
- 📁 **Log forwarding from AD, Linux, and pfSense**  
- 🧠 **Threat Intelligence correlation**  
- 🔄 **Backups to GitHub**  
- 🌍 **Optional: Web, domain, and mail server log aggregation**

## 🧰 Requirements

- At least 2 physical or virtual machines  
- VirtualBox or bare-metal hardware  
- pfSense ISO, Windows Server ISO, Ubuntu Server ISO  
- Splunk (Free or Enterprise trial)  
- Azure account (free tier or subscription)  
- GitHub account  
- Internet connection

## 📦 Features

- **VPN access** with OpenVPN for secure external access to your lab  
- **Network segmentation** via pfSense and VLANs  
- **Traffic inspection and alerting** using Suricata  
- **SIEM dashboards and alerts** through Splunk and Azure Sentinel  
- **Centralized logging** from Windows Server, Linux, pfSense  
- **Threat detection and mitigation**  
- **GitHub integration** for documentation and configuration backup  



## 📈 Future Improvements

- Automate deployment via Ansible or Terraform  
- Expand to cloud-native SIEM (ELK stack, Wazuh)  
- Use GitHub Actions for automated backups  

## 💬 Feedback & Contributions

Pull requests and suggestions are welcome! Help improve the guide and expand its capabilities.

🛠️ Update: Multi-Subnet Firewall Rule Implementation & OpenWRT WAN Access
📅 Date: June 17, 2025
🔧 Home Lab Project: Network Segmentation & Access Control

✅ What I Did:
Successfully diagnosed and resolved an access issue between segmented subnets in my home lab.

Configured OpenWRT (Netgear R6220) to allow secure web-based (LuCI) and SSH management from outside its default LAN.

Enabled admin access from both the 192.168.4.0/24 (main LAN) and 192.168.3.0/24 (XPS/dev lab) networks.

Verified functionality via IP 192.168.2.28 (OpenWRT WAN interface) from multiple subnets.

Added granular firewall traffic rules in OpenWRT to:

Allow LuCI over TCP (80/443) from trusted internal subnets

Allow SSH (22) for secure CLI access

Maintained NAT separation and ensured no exposure to the public internet.

🧠 What I Learned:
OpenWRT does not allow WAN-to-LAN access by default, even from internal routed networks — must explicitly define rules.

Firewall rule design requires directional awareness (source zone, dest zone).

Multi-subnet environments benefit from clear IP schema and labeling.

📍 Next Steps:
Begin testing Suricata IDS/IPS deployment on either pfSense or OpenWRT

Log and analyze traffic patterns between segmented zones

Prepare for VPN and VLAN integration in phase 2 of the home lab

Document topology and firewall rules for repository clarity
---


This document is a living blueprint of the evolving Paige Home Lab. Configs and implementations are updated as new services come online.
© 2025 John Wesley Paige Jr.
