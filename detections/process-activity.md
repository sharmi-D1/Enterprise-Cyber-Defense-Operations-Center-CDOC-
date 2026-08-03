# Process Activity Detection

## Objective

Monitor endpoint process creation and execution to identify potentially unusual process activity.

## Data Source

Sysmon process telemetry collected from Windows endpoints and analyzed through Splunk.

## Detection Logic

The detection focuses on process execution information and associated endpoint context.

**Actual SPL:** Add the exact SPL query used in the lab if available.

## Investigation

The analyst should review:

* Process name
* Process path
* Command line
* Parent process
* Executing user
* Process creation time
* Related network activity

## Analyst Assessment

Process activity should be evaluated against the normal behavior of the endpoint. Suspicious parent-child relationships, unusual execution paths, or unexpected command-line activity may warrant further investigation.

Process telemetry provides important context for analyzing endpoint behavior and supporting other detections.
