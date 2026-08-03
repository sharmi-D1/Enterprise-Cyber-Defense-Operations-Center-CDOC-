# Splunk SIEM

## Overview

Splunk Enterprise is the central SIEM platform used in the CDOC for collecting, searching, and analyzing security telemetry from the Windows endpoints.

## Log Sources

The implemented environment uses:

* Windows Event Logs
* Sysmon telemetry
* Microsoft Defender security telemetry

## Log Collection

The Splunk Universal Forwarder is configured on the monitored endpoints to forward relevant telemetry to Splunk Enterprise.

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

## Security Analysis

Splunk is used for:

* Security event searching
* Endpoint activity analysis
* Detection development
* Investigation of suspicious activity
* Security monitoring dashboards

## Evidence

<img width="1918" height="966" alt="Screenshot 2026-06-04 190657" src="https://github.com/user-attachments/assets/869a6132-da05-4d99-94b7-767a6ad40624" />
<img width="1917" height="967" alt="Screenshot 2026-06-04 203738" src="https://github.com/user-attachments/assets/27dac932-9fd3-4bf0-8328-847a70746b61" />
<img width="1918" height="968" alt="Screenshot 2026-06-06 171424" src="https://github.com/user-attachments/assets/0c4ff2a8-e61b-408c-acf9-5bb084c0a45b" />
<img width="1918" height="968" alt="Screenshot 2026-06-06 171728" src="https://github.com/user-attachments/assets/47c5ce81-e274-4495-805f-57be5ecb9960" />
<img width="1917" height="970" alt="Screenshot 2026-06-11 172838" src="https://github.com/user-attachments/assets/d1d7fc24-76ee-42f8-902e-a396aa930db3" />
<img width="1913" height="976" alt="Screenshot 2026-06-11 173008" src="https://github.com/user-attachments/assets/1af92449-2b63-4047-9798-3684332c0cee" />
<img width="1918" height="970" alt="Screenshot 2026-06-11 195038" src="https://github.com/user-attachments/assets/483b9818-1051-4f65-b682-c41f3b72ef63" />


