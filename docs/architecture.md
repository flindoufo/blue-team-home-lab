# 🏗️ Laboratory Architecture

## Overview

The Blue Team Home Lab is designed as an isolated virtual
cybersecurity environment.

## Components

| Component | Role |
|---|---|
| Wazuh | SIEM / XDR / Security Monitoring |
| Windows | Endpoint |
| Sysmon | Windows telemetry |
| Ubuntu | Linux server |
| Suricata | Network Security Monitoring |
| Kali Linux | Controlled attack simulation |

## Network

Planned network:

`192.168.56.0/24`

Planned hosts:

| Host | IP | Role |
|---|---|---|
| Wazuh | 192.168.56.10 | SOC |
| Windows | 192.168.56.20 | Endpoint |
| Ubuntu | 192.168.56.30 | Server |
| Kali | 192.168.56.40 | Attack simulation |

> IP addresses above are planned laboratory addresses and may change
> during implementation.

## Data Flow

```text
Windows
   │
 Sysmon
   │
Wazuh Agent
   │
   ├───────────────┐
                   │
Ubuntu ────────────┤
                   ▼
                Wazuh
                   │
                   ▼
               SOC Analyst
```
