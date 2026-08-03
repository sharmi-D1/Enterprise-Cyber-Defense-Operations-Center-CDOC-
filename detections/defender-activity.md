# Microsoft Defender Activity Detection

## Objective

Monitor security-relevant Microsoft Defender activity on Windows endpoints.

## Data Source

Microsoft Defender and Windows endpoint security telemetry collected for analysis in Splunk.

## Detection Logic

The detection focuses on Defender-related events that may indicate changes in endpoint protection or other security-relevant activity.

**Actual SPL:** Add the exact SPL query used in the lab if available.

## Investigation

The analyst should review:

* Defender event type
* Affected endpoint
* User or process associated with the event
* Timestamp
* Related process activity
* Other endpoint security events

## Analyst Assessment

Defender-related events should be evaluated in context. Administrative changes may be legitimate, while unexpected security-control changes can require further investigation.

The detection provides additional visibility into endpoint security activity within the monitored Windows environment.
