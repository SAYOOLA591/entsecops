# Enterprise Security Operation Projects Portfolio

The primary goal of this lab is to simulate a real-world security operations environment, providing hands-on experience in cybersecurity. The main objectives are to understand the flow of attacks, implement proper logging and monitoring, and practice responding to various threats.

## 🔗 Infrastructure Architectural Diagram

![architect1](https://github.com/user-attachments/assets/9eec6476-ec9e-4aac-a3a6-0cf8c7eca70f)

## 🔗 Foundation: Lab Setup & Networking

This project simulates a real-world enterprise environment by integrating multiple security and infrastructure components into a single detection lab. The goal is to replicate how organisations deploy, monitor, and defend their networks, creating a hands-on environment for both learning and detection engineering.
We will build this environment using VMware to host all virtual machines, each representing critical pieces of an enterprise network. Every system will be configured with static IP addresses, ensuring reliable communication across the lab. This mirrors a real-world setup where servers, firewalls, and endpoints are tied together under a structured network topology.

## 🔗 Core Lab Components

1. **Active Directory Domain Services (Windows Server 2022)**

   - Acts as the centralized identity provider.
   - Manages authentication, users, and groups.
   - Provides rich security event logs for monitoring.
   - Integrated with Windows 10 Pro client, simulating a typical enterprise workstation joined to the domain.
  
2. **Splunk (SIEM)**
   - Centralized log management and monitoring.
   - Ingests logs from pfSense, AD, Windows 10, Sysmon, Zeek, and Suricata.
   - Enables queries, dashboards, and alerting for detection and threat hunting.

3. **Intrusion Detection Systems (Zeek & Suricata)**
    - Zeek provides deep protocol analysis and behavioural visibility.
    - Suricata provides signature-based intrusion detection and alerts.
    - Together, they enhance network-layer visibility for malicious activity.

4. **Windows 10 Pro Client**
    - Domain-joined workstation for simulating real user activity.
    - Equipped with Sysmon for detailed endpoint telemetry (processes, registry, network connections).
    - Generates normal user behaviour as well as logs during simulated attacks

5. **Attacker Machine (Kali Linux)**
    - Simulates an external or insider threat.
    - Runs tools like Atomic Red Team to mimic techniques across the MITRE ATT&CK framework.
