---
title: Azure Monitor Logs reference - DeviceSkypeSignIn
description: Reference for DeviceSkypeSignIn table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: edbaynash
author: EdB-MSFT
ms.date: 08/08/2023
---

# DeviceSkypeSignIn

 

## Categories

- Workloads
## Solutions

- Surface Hub




## Columns

| Column | Type | Description |
| --- | --- | --- |
| _BilledSize | real | The record size in bytes |
| Computer | string |  |
| EventId | int |  |
| EventName | string |  |
| HealthServiceId | string |  |
| _IsBillable | string | Specifies whether ingesting the data is billable. When _IsBillable is *false* ingestion isn't billed to your Azure account |
| Opcode | int |  |
| ProviderId | string |  |
| SourceSystem | string | The type of agent the event was collected by. For example, *OpsManager* for Windows agent, either direct connect or Operations Manager, *Linux* for all Linux agents, or *Azure* for Azure Diagnostics |
| TimeGenerated | datetime |  |
| Type | string | The name of the table |
