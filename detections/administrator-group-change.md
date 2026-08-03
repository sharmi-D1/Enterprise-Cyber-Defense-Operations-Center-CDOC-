# Administrator Group Change Detection

## Objective

Monitor changes to privileged Windows administrator group membership.

## Data Source

Windows Security Event Logs collected in Splunk.

## Detection Logic

The detection identifies events associated with changes to administrator-group membership.

**Actual SPL:** Add the exact SPL query used in the lab if available.

## Investigation

The analyst should examine:

* Account added or removed
* Administrator group affected
* User performing the change
* Endpoint involved
* Timestamp
* Related authentication or process activity

## Analyst Assessment

Privileged group changes should be validated against authorized administrative activity. Unexpected membership changes may indicate unauthorized privilege modification and should receive additional investigation.

This detection provides visibility into changes affecting privileged access within the Windows environment.
