---
title: Azure Monitor Logs reference - SfBAssessmentRecommendation
description: Reference for SfBAssessmentRecommendation table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: edbaynash
author: EdB-MSFT
ms.date: 08/08/2023
---

# SfBAssessmentRecommendation

 Recommendations generated by Skype for Business assessments that are started through a scheduled task. When you schedule the assessment it runs by default every 7 days and upload the data into Azure Log Analytics

## Categories

- Workloads
## Solutions

- AzureResources
- SfBAssessment




## Columns

| Column | Type | Description |
| --- | --- | --- |
| ActionArea | string |  |
| ActionAreaId | string |  |
| AffectedObjectName | string |  |
| AffectedObjectType | string |  |
| AssessmentId | string |  |
| _BilledSize | real | The record size in bytes |
| Computer | string |  |
| CustomData | string |  |
| Description | string |  |
| Domain | string |  |
| FocusArea | string |  |
| FocusAreaId | string |  |
| Forest | string |  |
| _IsBillable | string | Specifies whether ingesting the data is billable. When _IsBillable is *false* ingestion isn't billed to your Azure account |
| LyncCentralMgmtStoreDatabase | string |  |
| LyncFEPool | string |  |
| LyncFrontEnd | string |  |
| LyncInternalDomain | string |  |
| LyncOrganization | string |  |
| LyncSimpleURLDomain | string |  |
| LyncSite | string |  |
| LyncUserStoreDatabase | string |  |
| Recommendation | string |  |
| RecommendationId | string |  |
| RecommendationResult | string |  |
| RecommendationWeight | real |  |
| SourceSystem | string | The type of agent the event was collected by. For example, *OpsManager* for Windows agent, either direct connect or Operations Manager, *Linux* for all Linux agents, or *Azure* for Azure Diagnostics |
| Technology | string |  |
| TimeGenerated | datetime |  |
| Type | string | The name of the table |
