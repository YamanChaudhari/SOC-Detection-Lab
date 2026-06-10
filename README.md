# SOC Detection Lab

## Overview

This project demonstrates the creation of a Security Operations Center (SOC) Detection Lab using Splunk Enterprise, Sysmon, Universal Forwarder, and Atomic Red Team.

The objective of this lab was to collect endpoint telemetry, simulate adversary techniques, investigate logs, create detections, and build a custom Splunk dashboard for monitoring and threat hunting.

---

## Lab Architecture

Windows 11 Endpoint

↓ Sysmon

↓ Universal Forwarder

Splunk Enterprise

↓ Detection Queries

SOC Dashboard

---

## Tools Used

* Splunk Enterprise
* Sysmon
* Splunk Universal Forwarder
* Atomic Red Team
* Windows 11
* VMware Workstation

---

## ATT&CK Techniques Tested

| ATT&CK ID | Technique                              |
| --------- | -------------------------------------- |
| T1033     | System Owner/User Discovery            |
| T1082     | System Information Discovery           |
| T1016     | System Network Configuration Discovery |
| T1112     | Modify Registry                        |
| T1059.001 | PowerShell                             |

---

## Detection Queries

### PowerShell Activity

Detects PowerShell execution events.

### Reconnaissance Activity

Detects discovery commands such as:

* whoami.exe
* systeminfo.exe
* ipconfig.exe
* reg.exe

### Registry Activity

Monitors registry-related commands.

### Network Activity

Monitors Sysmon Event ID 3 network connections.

---

## Dashboard Features

The custom Splunk dashboard includes:

* Top Processes
* PowerShell Activity
* Reconnaissance Activity
* Registry Activity
* Network Activity

---

## Skills Demonstrated

* Security Monitoring
* Log Analysis
* Splunk Searching (SPL)
* Sysmon Configuration
* MITRE ATT&CK Mapping
* Detection Engineering
* Threat Hunting Fundamentals
* Dashboard Development

---

## Project Outcome

Successfully built a SOC Detection Lab capable of collecting Windows telemetry, detecting ATT&CK techniques, investigating process activity, monitoring network connections, and visualizing security events through a custom Splunk dashboard.
