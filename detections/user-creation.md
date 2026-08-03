# Local User Creation Detection

## Objective

Identify the creation of new local Windows user accounts that may represent unauthorized account activity.

## Data Source

Windows Security Event Logs collected and analyzed through Splunk.

## Detection Logic

The detection identifies Windows account-creation activity and provides the analyst with the associated account and event information.

**Actual SPL:** Add the exact SPL query used in the lab if available.

## Investigation

The analyst should review:

* Newly created username
* Account creation time
* Account-creating user
* Hostname
* Related account activity
* Whether the account was expected

## Analyst Assessment

New account creation should be compared with expected administrative activity. An unexpected account, particularly on a sensitive endpoint, may require further investigation.

The detection provides visibility into account-management activity and supports centralized monitoring of Windows security events.

