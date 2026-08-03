# Splunk Log Collection

## 1. Objective

The objective of the log collection setup was to centralize security-relevant Windows endpoint telemetry in Splunk Enterprise. This allows endpoint events to be searched and analyzed from a centralized SIEM rather than reviewing logs individually on each Windows system.

## 2. Endpoint Configuration

The Windows endpoints were configured as monitored systems within the VMware Workstation laboratory environment. Relevant Windows security and system telemetry was generated through Windows Event Logs, while Sysmon provided additional endpoint activity information.

Microsoft Defender also provided endpoint security telemetry where applicable.

## 3. Splunk Universal Forwarder

The Splunk Universal Forwarder was used as the endpoint log collection and forwarding component. It collects the configured Windows telemetry and forwards the events to the Splunk Enterprise instance for centralized analysis.

## 4. Configured Data Sources

The implemented environment uses the following endpoint telemetry sources:

* Windows Event Logs
* Sysmon
* Microsoft Defender telemetry

These sources provide information related to Windows security events, process activity, PowerShell activity, authentication, DNS, network connections, and other endpoint events available in the configured logs.

## 5. Forwarding Configuration

The Universal Forwarder was configured to forward the required endpoint telemetry from the Windows systems to the Splunk Enterprise environment.

```text
Windows Endpoint
      |
      +-- Windows Event Logs
      +-- Sysmon
      +-- Defender
      |
      v
Splunk Universal Forwarder
      |
      v
Splunk Enterprise
```

## 6. Splunk Receiving Configuration

Splunk Enterprise acts as the centralized receiving and analysis platform. Forwarded endpoint events are indexed and made available for searching and security analysis.

The exact receiving configuration should correspond to the configuration used in the actual lab.

## 7. Verification

Log collection was verified by checking whether endpoint events were successfully received and searchable within Splunk. The received telemetry was then used for security monitoring and detection development.

## 8. Evidence

screenshots/logcollections
