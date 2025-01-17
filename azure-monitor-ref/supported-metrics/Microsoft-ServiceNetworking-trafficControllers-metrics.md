---
title: Supported metrics - Microsoft.ServiceNetworking/trafficControllers
description: Reference for Microsoft.ServiceNetworking/trafficControllers metrics in Azure Monitor.
ms.topic: reference
ms.service: azure-monitor
ms.author: edbaynash
author: EdB-MSFT
ms.date: 07/17/2023
---
# Supported metrics for Microsoft.ServiceNetworking/trafficControllers  
<!-- Data source : naam-->


The following table lists the metrics available for the Microsoft.ServiceNetworking/trafficControllers resource type.

  

**Table headings**
  
**Metric** - Metric display name follows by a description of the metric. The displayname appears in the Azure portal.  
**Name** - The name of the metric as referred to in the REST API.  
**Unit** - The default units used for the metric.  
**Aggregation** - The default aggregation type for this metric. Valid values: Average, Minimum, Maximum, Total, Count.  
**Dimensions** - Dimensions available. For more information, see (link to dimensions information).  
**DS Export**- Whether the metric is exportable to Azure Monitor Logs via Diagnostic Settings.  You can access all metrics via the REST API.  
  
  
|Metric|Name|Unit|Aggregation|Dimensions|DS Export|
|---|---|---|---|---|---|
|Backend Connection Timeouts<p><p>Count of requests that timed out waiting for a response from the backend target (includes all retry requests initiated from Application Gateway for Containers to the backend target) |`BackendConnectionTimeouts` |Count |Total |Microsoft.regionName, BackendService |Yes|
|Backend Healthy Targets<p><p>Count of healthy backend targets |`BackendHealthyTargets` |Count |Average |Microsoft.regionName, BackendService |Yes|
|Backend HTTP Response Status<p><p>HTTP response status returned by the backend target to Application Gateway for Containers |`BackendHTTPResponseStatus` |Count |Total |Microsoft.regionName, BackendService, HttpResponseCode |Yes|
|Total Connection Idle Timeouts<p><p>Count of connections closed, between client and Application Gateway for Containers frontend, due to exceeding idle timeout |`ClientConnectionIdleTimeouts` |Count |Total |Microsoft.regionName, Frontend |Yes|
|Connection Timeouts<p><p>Count of connections closed due to timeout between clients and Application Gateway for Containers |`ConnectionTimeouts` |Count |Total |Microsoft.regionName, Frontend |Yes|
|HTTP Response Status<p><p>HTTP response status returned by Application Gateway for Containers |`HTTPResponseStatus` |Count |Total |Microsoft.regionName, Frontend, HttpResponseCode |Yes|
|Total Requests<p><p>Count of requests Application Gateway for Containers has served |`TotalRequests` |Count |Total |Microsoft.regionName, Frontend |Yes|


<!--Gen Date:  Mon Jul 17 2023 12:39:39 GMT+0300 (Israel Daylight Time)-->