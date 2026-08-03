# Suspicious PowerShell Detection

## Objective

Identify PowerShell execution that may require additional security investigation.

## Data Source

Primary telemetry is collected from Windows endpoint activity and Sysmon process-related events and analyzed in Splunk.

## Detection Logic

The detection focuses on identifying PowerShell execution and reviewing associated process information and command-line activity.

**Actual SPL:** Add the exact SPL query used in the lab if available.

## Investigation

When PowerShell activity is identified, an analyst should review:

* Executed command
* User account
* Parent process
* Process path
* Timestamp
* Related endpoint activity
* Network connections associated with the process

PowerShell is commonly used for legitimate administration, so execution alone should not automatically be classified as malicious.

## Analyst Assessment

The surrounding context should be reviewed to determine whether the activity is expected administrative behavior or requires escalation.

