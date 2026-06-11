# Azure Sentinel Threat Hunting Lab

## Overview

This project demonstrates the creation of a cloud-based Security Operations Center (SOC) lab using Microsoft Azure, Microsoft Sentinel, Sysmon, Azure Monitor Agent, and Log Analytics Workspace.

The objective of the lab was to simulate real-world detection engineering and threat hunting workflows by collecting endpoint telemetry, developing KQL detections, and generating security incidents through Microsoft Sentinel.

## Technologies Used

* Microsoft Azure
* Microsoft Sentinel
* Azure Monitor Agent (AMA)
* Log Analytics Workspace
* Sysmon
* Kusto Query Language (KQL)

## Data Sources

* Sysmon Event ID 1 – Process Creation
* Sysmon Event ID 3 – Network Connection
* Sysmon Event ID 13 – Registry Modification
* Sysmon Event ID 22 – DNS Query

## Detection Use Cases

### PowerShell Network Correlation Detection

Correlates PowerShell execution with network activity to identify potentially suspicious command execution and outbound communication.

### Registry Persistence Detection

Detects modifications to Windows Run registry keys commonly used for persistence.

## Key Outcomes

* Built a cloud-native SOC lab using Microsoft Sentinel
* Integrated Sysmon telemetry into Azure Log Analytics
* Developed KQL detections and analytics rules
* Generated and investigated security incidents
* Mapped detections to MITRE ATT&CK techniques

## Cloud Monitoring

* Azure Activity Log ingestion
* Cloud resource deployment monitoring
* VM lifecycle monitoring
* Resource modification detections


## Architecture

Windows Server 2025 VM
        ↓
      Sysmon
        ↓
Azure Monitor Agent
        ↓
Log Analytics Workspace
        ↓
Microsoft Sentinel
        ↓
Analytics Rules
        ↓
Alerts & Incidents
