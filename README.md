# Home Lab | SOC | Self-Hosted Infrastructure

Welcome to my personal home lab documentation. This project is a learning environment where I'm building, configuring, and managing a hybrid network infrastructure — with on-premises and cloud integration — as part of my journey into cybersecurity, cloud computing, and networking.

---

## Project Overview

This lab is designed to simulate a small enterprise network, integrating core IT and cybersecurity technologies. It includes firewalling, network segmentation, a Windows domain, log monitoring, and a hybrid cloud environment leveraging AWS.

### Goals:

- Build a functional and secure home lab environment.
- Gain hands-on experience with enterprise-level tools.
- Explore threat detection, logging, and network defense.
- Integrate AWS for hybrid infrastructure backup and expansion.

---

## Core Technologies

| Tech | Description |
|------|-------------|
| **pfSense** | Firewall/router used to manage VLANs and secure network traffic. |
| **Windows Server 2019** | Hosting Active Directory/AD DS for domain management. |
| **Suricata** | IDS/IPS for network-level threat detection. |
| **Splunk Free** | Log aggregation, searching, and analysis. |
| **AWS** | Cloud integration for hybrid network design and log backups. |
| **GitHub** | Documentation, version control, and public portfolio. |

---

## Network Architecture (Planned)

- **LAN (192.168.2.0/24)**: Core trusted network
- **VLANs**: Segmented for devices, labs, management, and IoT
- **DMZ**: For future external-facing services (e.g., web server)
- **VPN**: Remote access using OpenVPN or WireGuard

---

## Hybrid Cloud Plan (AWS)

- **S3**: Log backup and archival
- **EC2**: Optional virtual SOC components (e.g., ELK Stack or Splunk forwarder)
- **CloudWatch**: Potential integration for monitoring/logs
- **IAM**: Role-based access for security best practices

---

## Future Additions

- ELK Stack integration
- SIEM comparison (Splunk vs ELK vs Wazuh)
- Syslog server for network devices
- External SSD storage for logs
- Self-hosted web portal
- Honeypot deployment

---

## Why This Lab?

I'm studying cybersecurity with a focus on cloud networking and this lab is how I’m getting hands-on with the tools and technologies used in real-world SOC and DevSecOps environments. It’s also a showcase of my growing skills in infrastructure design, cloud integration, and threat detection.

---

## Contact

If you'd like to connect, collaborate, or offer feedback — find me on LinkedIn or shoot me a message via GitHub.

---

> **Note**: This documentation is a work in progress and will be updated as new features are added.