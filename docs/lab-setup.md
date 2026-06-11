# Lab Setup

## Azure Resources

* Azure Virtual Machine (Windows Server 2025)
* Log Analytics Workspace
* Microsoft Sentinel
* Azure Monitor Agent

## Endpoint Telemetry

Sysmon was configured to collect:

* Process Creation Events
* Network Connections
* DNS Queries
* Registry Modifications

## Data Collection

A Data Collection Rule (DCR) was configured to forward Sysmon events to the Log Analytics Workspace.

## Detection Engineering

Custom KQL detections were developed and deployed as Microsoft Sentinel Analytics Rules to generate incidents from suspicious activity.
