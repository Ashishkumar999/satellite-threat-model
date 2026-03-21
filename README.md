# 🛰️ Satellite Threat Model

Beginner Space Cybersecurity Project – Satellite Threat Modeling

---

## 📌 Overview

This project presents a beginner-level satellite threat model that analyzes cybersecurity risks across the three major space system segments:

- Ground Segment
- Communication Segment
- Space Segment

The objective is to understand how attackers could target satellite infrastructure and how security controls can mitigate those risks.

---

## 🎯 Project Objective

This project demonstrates:

- Identification of satellite system assets
- Entry point discovery
- Attack surface analysis
- Attack chain modeling
- Security control recommendations

This serves as an entry-level portfolio project in Space Cybersecurity.

---

## 🧩 System Architecture
Mission Control
↓
Command Server
↓
Ground Station Network
↓
RF Antenna (Uplink)
↓
Satellite Communication System
↓
Onboard Computer (OBC)
↓
Satellite Subsystems
↓
Payload
↓
Telemetry Downlink
↓
Ground Station Receiver

## 🧩 System Architecture Diagram

<img width="127" height="1331" alt="satellite-architecture" src="https://github.com/user-attachments/assets/12f6320c-6a60-4746-91d1-a478de22653b" />
---

## 🎯 Assets Identified

| Asset | Importance |
|------|-----------|
| Satellite | Mission-critical system |
| Command Server | Controls satellite behavior |
| Ground Station | Communication infrastructure |
| Telemetry Data | Satellite health monitoring |
| RF Communication Link | Command and data transfer |

---

## 🚪 Entry Points

Potential attacker entry points include:

- Mission control dashboards (web interfaces)
- Ground station internal networks
- Command APIs
- RF uplink/downlink communication channels

---

## ⚠️ Threat Analysis

### 🌍 Ground Segment Threats

- Web vulnerabilities (XSS, SQL Injection)
- Weak authentication mechanisms
- Phishing attacks targeting operators
- Insider access misuse

### 📡 Communication Segment Threats

- RF jamming
- Signal spoofing
- Replay attacks
- Signal interception

### 🛰 Space Segment Threats

- Firmware vulnerabilities
- Command injection
- Payload manipulation
- Unauthorized subsystem control

---

## 🔗 Attack Chain Example 1 — Ground Station Compromise
Attacker
↓
Phishing Email
↓
Credential Theft
↓
Ground Station Access
↓
Command Server Compromise
↓
Malicious Commands Sent
↓
Satellite Executes Commands


---

## 🔗 Attack Chain Example 2 — RF Spoofing Attack
Attacker
↓
Fake RF Signal Transmission
↓
Satellite Receiver Accepts Signal
↓
Fake Commands Executed
↓
Satellite Behavior Altered


---

## 🛡 Security Controls

| Area | Control |
|------|--------|
| Command System | Authentication & Authorization |
| Communication Link | Encryption |
| Ground Infrastructure | Network segmentation & firewall protection |
| Monitoring | Logging and anomaly detection |

---

## 📊 Risk Summary

| Risk | Impact |
|------|--------|
| Ground station compromise | Full satellite control |
| RF spoofing | Unauthorized command execution |
| RF jamming | Communication disruption |
| Firmware exploitation | Satellite takeover risk |

---

## 🚀 Future Improvements

Planned next steps:

- Add RF signal analysis using RTL-SDR
- Implement CCSDS telemetry packet parsing
- Simulate command injection scenarios
- Expand threat model using STRIDE methodology

---

## 👨‍💻 Author

Ashish Kumar Giri  
Cybersecurity Engineer (VAPT → Space Cybersecurity)

---

## ⭐ Project Status

Completed as part of Space Cybersecurity learning roadmap (Month 1)

