---
title: Azure Monitor Logs reference - DnsInventory
description: Reference for DnsInventory table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: edbaynash
author: EdB-MSFT
ms.date: 08/08/2023
---

# DnsInventory

 

## Categories

- Network
## Solutions

- DNS Analytics (Preview)
## Resource types

- Virtual machines
- VMware
- Azure Stack HCI
- System Center Virtual Machine Manager




## Columns

| Column | Type | Description |
| --- | --- | --- |
| _BilledSize | real | The record size in bytes |
| Computer | string |  |
| DnsSecSigned | string |  |
| DomainName | string |  |
| DynamicUpdate | string |  |
| ForestName | string |  |
| _IsBillable | string | Specifies whether ingesting the data is billable. When _IsBillable is *false* ingestion isn't billed to your Azure account |
| NameServers | string |  |
| _ResourceId | string | A unique identifier for the resource that the record is associated with |
| ResourceRecordName | string |  |
| ResourceRecordType | string |  |
| ServerIPs | string |  |
| SourceSystem | string | The type of agent the event was collected by. For example, *OpsManager* for Windows agent, either direct connect or Operations Manager, *Linux* for all Linux agents, or *Azure* for Azure Diagnostics |
| _SubscriptionId | string | A unique identifier for the subscription that the record is associated with |
| SubType | string |  |
| TimeGenerated | datetime |  |
| Type | string | The name of the table |
| ZoneName | string |  |
