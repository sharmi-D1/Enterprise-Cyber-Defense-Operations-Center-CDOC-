# Encoded PowerShell Detection

## Objective

Identify PowerShell execution containing encoded command activity that may require investigation.

## Data Source

Sysmon process telemetry and Windows endpoint logs collected in Splunk.

## Detection Logic

The detection searches PowerShell process activity for indicators associated with encoded command execution.

**Actual SPL:** Add the exact SPL query used in the lab if available.

## Investigation

The analyst should review:

* PowerShell command-line information
* Executing user
* Parent process
* Process creation time
* Associated network connections
* Related endpoint events

Encoded commands can have legitimate administrative uses, so the presence of encoding alone should be treated as a suspicious indicator rather than definitive proof of malicious activity.

## Analyst Assessment

The analyst correlates the PowerShell event with surrounding endpoint telemetry to determine whether the activity is legitimate, suspicious, or requires escalation.

