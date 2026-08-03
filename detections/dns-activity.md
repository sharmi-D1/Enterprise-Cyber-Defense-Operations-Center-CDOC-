# DNS Activity Detection

## Objective

Monitor DNS activity from Windows endpoints and identify potentially unusual domain-resolution behavior.

## Data Source

Endpoint DNS-related telemetry collected through Sysmon and analyzed in Splunk.

## Detection Logic

The detection focuses on DNS query activity and associated endpoint information.

**Actual SPL:** Add the exact SPL query used in the lab if available.

## Investigation

The analyst should review:

* Queried domain
* Source endpoint
* Query timestamp
* Frequency of queries
* Related process activity
* Related network connections

## Analyst Assessment

DNS activity should be evaluated in context. Unusual domains or unexpected query patterns may require additional investigation, particularly when correlated with suspicious process or network activity.

DNS telemetry provides useful context when investigating endpoint behavior and network activity.
