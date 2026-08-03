# Network Activity Detection

## Objective

Monitor endpoint network connections and identify potentially unusual communication from Windows systems.

## Data Source

Sysmon network-related telemetry and other available endpoint network events analyzed through Splunk.

## Detection Logic

The detection focuses on network connection events and their associated endpoint context.

**Actual SPL:** Add the exact SPL query used in the lab if available.

## Investigation

The analyst should review:

* Source endpoint
* Destination address
* Destination port
* Process responsible for the connection
* User context
* Timestamp
* Related DNS activity

## Analyst Assessment

Network connections should be assessed using endpoint and network context. An unusual destination or unexpected process initiating a connection may warrant further investigation.

Wireshark can provide packet-level visibility when deeper network analysis is required.
