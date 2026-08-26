# 🔐 Blue Team Home Lab

![Status](https://img.shields.io/badge/status-in%20development-yellow)
![Focus](https://img.shields.io/badge/focus-blue%20team-blue)
![Environment](https://img.shields.io/badge/environment-isolated%20lab-green)

---

## 🎯 About the Project

The **Blue Team Home Lab** is a practical cybersecurity laboratory
created to develop hands-on skills in defensive security operations.

The project focuses on building, monitoring and investigating a
controlled environment that simulates a small enterprise security
operation.

The goal is not simply to deploy security tools, but to understand
the complete defensive workflow:

**Detection → Triage → Investigation → Response → Documentation → Improvement**

---

## 🧠 Learning Objectives

This project aims to develop practical knowledge in:

- SOC Operations
- SIEM
- Log Analysis
- Endpoint Detection
- Network Security Monitoring
- Detection Engineering
- MITRE ATT&CK
- Threat Hunting
- Incident Response
- Security Documentation
- Security Automation

---

## 🛠️ Technology Stack

### Security

- Wazuh
- Sysmon
- Suricata
- Sigma
- MITRE ATT&CK

### Operating Systems

- Windows
- Linux
- Kali Linux

### Infrastructure

- Virtualization
- Isolated Network
- Security Monitoring
- Log Collection

---

## 🏗️ Architecture

The laboratory will consist of an isolated virtual environment
containing endpoints, servers, an attack simulation machine and a
central security monitoring platform.

```text
                         ┌──────────────────┐
                         │      WAZUH       │
                         │    SIEM / XDR    │
                         └────────┬─────────┘
                                  │
                   ┌──────────────┼──────────────┐
                   │              │              │
                   ▼              ▼              ▼
             ┌──────────┐   ┌──────────┐   ┌──────────┐
             │ Windows  │   │  Ubuntu  │   │ Suricata │
             │ Endpoint │   │  Server  │   │ Network  │
             └────┬─────┘   └────┬─────┘   └────┬─────┘
                  │              │              │
                Sysmon        Linux Logs        │
                  │              │              │
                  └──────────────┼──────────────┘
                                 │
                                 ▼
                            SOC Analyst
                                 ▲
                                 │
                           ┌─────┴─────┐
                           │   Kali    │
                           │  Attack   │
                           │ Simulation│
                           └───────────┘
```

> All attack simulations are performed exclusively inside the
> isolated laboratory environment.

---

## 📊 Project Progress

### Infrastructure

- [ ] Virtualization environment
- [ ] Isolated network
- [ ] Windows endpoint
- [ ] Ubuntu server
- [ ] Kali Linux
- [ ] Wazuh server

### SOC

- [ ] Wazuh agents
- [ ] Log collection
- [ ] Initial dashboards
- [ ] Alert investigation

### Endpoint Security

- [ ] Sysmon
- [ ] Process telemetry
- [ ] Network telemetry
- [ ] PowerShell monitoring

### Network Security

- [ ] Suricata
- [ ] Network monitoring
- [ ] Network scanning detection
- [ ] Network investigation

### Detection Engineering

- [ ] Custom Wazuh rules
- [ ] Sigma rules
- [ ] MITRE ATT&CK mapping

### Threat Hunting

- [ ] Hunting methodology
- [ ] First hypothesis
- [ ] First hunt
- [ ] Hunt documentation

### Incident Response

- [ ] Incident templates
- [ ] Response playbooks
- [ ] Containment procedures
- [ ] Recovery procedures

### Capstone

- [ ] End-to-end scenario
- [ ] Detection
- [ ] Investigation
- [ ] Response
- [ ] Final report

---

## 🧪 Labs

| # | Lab | Status |
|---|---|---|
| 01 | SSH Brute Force | 🔴 Planned |
| 02 | Network Scanning | 🔴 Planned |
| 03 | Suspicious PowerShell | 🔴 Planned |
| 04 | Persistence | 🔴 Planned |
| 05 | Credential Attack | 🔴 Planned |
| 06 | Capstone | 🔴 Planned |

---

## 🚨 Incident Reports

Incident investigations will be documented using a standardized
incident response format.

| ID | Incident | Severity | Status |
|---|---|---|---|
| INC-001 | SSH Brute Force | — | Planned |
| INC-002 | Network Scanning | — | Planned |
| INC-003 | Suspicious PowerShell | — | Planned |
| INC-004 | Persistence | — | Planned |

---

## 📚 Documentation

- [Project Roadmap](docs/roadmap.md)
- [Learning Log](docs/learning-log.md)
- [Methodology](docs/methodology.md)
- [Architecture](docs/architecture.md)
- [Glossary](docs/glossary.md)

---

## 📈 Learning in Public

This repository documents the evolution of the project from initial
infrastructure deployment to detection engineering, threat hunting
and incident response.

The goal is to document not only successful results, but also:

- technical challenges;
- troubleshooting;
- failed approaches;
- investigations;
- lessons learned;
- improvements.

---

## ⚠️ Disclaimer

This project is intended exclusively for educational purposes and
controlled laboratory environments.

No attack simulation described in this repository should be performed
against systems, networks or accounts without explicit authorization.

---

## 👤 Project

Built as part of my transition into cybersecurity, with a focus on
Blue Team, SOC Operations and Security Engineering.
