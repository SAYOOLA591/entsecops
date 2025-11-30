# SOC Portfolio Project

The primary goal of this lab is to simulate a real-world security operations environment and provide hands-on cybersecurity experience. The main objectives are to understand the flow of attacks, implement proper logging and monitoring, and practice responding to various threats.

## 🔗 Infrastructure Architectural Diagram

![architect1](https://raw.githubusercontent.com/SAYOOLA591/active-directory-image/blob/main/Screenshot%202025-09-18%20112930.png)

## 🔗 Foundation: Lab Setup & Networking

This project simulates a real-world enterprise environment by integrating multiple security and infrastructure components into a single detection lab. The goal is to replicate how organisations deploy, monitor, and defend their networks, creating a hands-on environment for both learning and detection engineering.
We will build this environment using VMware to host all virtual machines, each representing critical pieces of an enterprise network. Every system will be configured with static IP addresses, ensuring reliable communication across the lab. This mirrors a real-world setup in which servers, firewalls, and endpoints are tied together within a structured network topology.

#

## 🔗 Active Directory & Identity Management
- **[Active Directory: Centralized Identity and Access Management](https://github.com/SAYOOLA591/Active-Directory/)**
  - Configured on Windows Server 2022 with AD, and deployed Microsoft Baseline Audit GPO with advanced audit policy recommendation, provisioning users into their respective Organisational Units (OUs) and connected endpoints to the Active Directory domain.

## 🔗 Network Security & Monitoring Deployment
- **[pfSense Firewall / Router](https://github.com/SAYOOLA591/pfsense/)**
  - Configured firewall and squid proxy simultaneously to act as the first line of defense, and squid proxy for monitoring HTTP/HTTPS requests and enabling content filtering.
- **[Zeek & Suricata: IDS/IPS](https://github.com/SAYOOLA591/zeek-suricata/)**
  - Deployed Zeek & Suricata to monitor the incoming TLS traffic fingerprint, enabling community rulesets, and a custom sliver C2 post-exploitation capabilities.
 
## 🔗 Splunk Configuration & Deployment
- **[SIEM Platform](https://github.com/SAYOOLA591/splunk-siem/)**
  - Deployed and Configured for threat hunting, network security monitoring, and comprehensive log management.
 
## 🔗 Attack Simulation & Telementry Management
- **[Kali And AtomicRedTeam Simulation](https://github.com/SAYOOLA591/telemetry-lab/)**
  - Simulated diverse attacks, essentially to generate different telemetry to enrich the lab.
