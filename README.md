## Overview
This project demonstrates a simulated enterprise network breach using a VirtualBox-based homelab.  
The lab was designed to replicate common attacker techniques and defensive detection methods in a controlled environment.

I acted as both the attacker and defender to better understand the full attack lifecycle, from initial access through detection and response.

---

## Lab Environment

### Infrastructure
- Kali Linux (Attacker)
- Windows Domain Controller
- Corporate Server
- Windows Client
- Linux Client

### Security Stack
- Wazuh (SIEM / host-based intrusion detection)

### VirtualBox Lab Overview
![VirtualBox Lab Overview](Screenshots/VirtualBox%20VMs.png)
<img width="3832" height="2248" alt="VirtualBox VMs" src="https://github.com/user-attachments/assets/bec78f85-2709-4165-9cff-35b24b8a8aee" /># Enterprise Security Homelab – Attack & Detection Simulation

---

## Attack Scenario (High-Level)

The following actions were simulated during the attack:

- Password dictionary attack to gain initial corporate access
- Internal network reconnaissance and service discovery
- Phishing-based credential harvesting
- Domain credential discovery and privilege escalation
- Lateral movement using remote management protocols
- Sensitive file access and exfiltration
- Persistence via administrative backdoor account

---

## Detection & Monitoring

- Wazuh agents deployed across hosts
- Detection of authentication anomalies and privilege escalation
- Monitoring of administrative account changes

## Tools Used

### Offensive
- Hydra
- Nmap
- NetExec
- Evil-WinRM
- xfreerdp
- SSH

### Defensive
- Wazuh
- Windows Event Logs
- Linux system logs

---

## Disclaimer
This project was conducted in a controlled lab environment for educational purposes only.
