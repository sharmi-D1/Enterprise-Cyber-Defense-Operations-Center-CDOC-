# CDOC Architecture

## Overview

The Cyber Defense Operations Center (CDOC) is implemented as a virtualized security environment using VMware Workstation. The environment contains Windows endpoints, centralized Splunk monitoring, endpoint telemetry collection, network analysis, and vulnerability assessment.

## Architecture Flow

```text
Windows Endpoints
       |
       +-- Windows Event Logs
       +-- Sysmon
       +-- Microsoft Defender
       |
       v
Splunk Universal Forwarder
       |
       v
Splunk Enterprise
       |
       +-- Security Monitoring
       +-- Detection Analysis

Wireshark
   |
   +-- Network Traffic Analysis

OpenVAS
   |
   +-- Vulnerability Assessment
```

## Components

| Component                  | Purpose                                |
| -------------------------- | -------------------------------------- |
| VMware Workstation         | Virtualized lab infrastructure         |
| Windows 10                 | Monitored enterprise endpoints         |
| Sysmon                     | Detailed endpoint telemetry            |
| Windows Event Logs         | Windows security and system events     |
| Microsoft Defender         | Endpoint security monitoring           |
| Splunk Universal Forwarder | Endpoint log forwarding                |
| Splunk Enterprise          | Centralized SIEM and security analysis |
| Wireshark                  | Network traffic analysis               |
| OpenVAS                    | Vulnerability assessment               |

## Data Flow

Windows endpoint telemetry is collected through Windows Event Logs and Sysmon and forwarded using the Splunk Universal Forwarder to Splunk Enterprise. Splunk is used for centralized security monitoring and detection analysis.

Wireshark is used independently for network traffic investigation, while OpenVAS is used for vulnerability scanning within the lab environment.

