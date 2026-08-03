# Detection Engineering

This directory contains the security detection use cases implemented using Splunk and endpoint telemetry collected from the Windows environment.

## Detection Use Cases

| Detection                  | Purpose                                              |
| -------------------------- | ---------------------------------------------------- |
| Suspicious PowerShell      | Identify potentially suspicious PowerShell execution |
| Encoded PowerShell         | Identify encoded PowerShell activity                 |
| Local User Creation        | Identify new local account creation                  |
| Administrator Group Change | Monitor changes to privileged group membership       |
| Defender Activity          | Monitor security-related Defender activity           |
| Process Activity           | Analyze endpoint process execution                   |
| DNS Activity               | Investigate DNS-related endpoint activity            |
| Network Activity           | Analyze endpoint network connections                 |

## Detection Structure

Each detection document contains:

* Detection objective
* Data source
* SPL query
* Relevant event information
* Detection logic
* Expected results
* Investigation considerations
* Screenshot evidence

All detection content is based on the telemetry and detection work implemented within the CDOC lab.

