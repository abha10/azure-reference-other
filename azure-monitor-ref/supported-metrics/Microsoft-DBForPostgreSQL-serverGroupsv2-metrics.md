---
title: Supported metrics - Microsoft.DBForPostgreSQL/serverGroupsv2
description: Reference for Microsoft.DBForPostgreSQL/serverGroupsv2 metrics in Azure Monitor.
ms.topic: reference
ms.service: azure-monitor
ms.author: edbaynash
author: EdB-MSFT
ms.date: 07/12/2023
---
# Supported metrics for Microsoft.DBForPostgreSQL/serverGroupsv2  
<!-- Data source : naam-->


The following table lists the metrics available for the Microsoft.DBForPostgreSQL/serverGroupsv2 resource type.

  

**Table headings**
  
**Metric** - Metric display name follows by a description of the metric. The displayname appears in the Azure portal.  
**Name** - The name of the metric as referred to in the REST API.  
**Unit** - The default units used for the metric.  
**Aggregation** - The default aggregation type for this metric. Valid values: Average, Minimum, Maximum, Total, Count.  
**Dimensions** - Dimensions available. For more information, see (link to dimensions information).  
**DS Export**- Whether the metric is exportable to Azure Monitor Logs via Diagnostic Settings.  You can access all metrics via the REST API.  
  
  
|Metric|Name|Unit|Aggregation|Dimensions|DS Export|
|---|---|---|---|---|---|
|Active Connections<p><p>Active Connections |`active_connections` |Count |Average |ServerName |Yes|
|Reserved Memory percent<p><p>Percentage of Commit Memory Limit Reserved by Applications |`apps_reserved_memory_percent` |Percent |Average |ServerName |Yes|
|CPU Credits Consumed<p><p>Total number of credits consumed by the node. Only available when burstable compute is provisioned on the node. |`cpu_credits_consumed` |Count |Average |ServerName |Yes|
|CPU Credits Remaining<p><p>Total number of credits available to burst. Only available when burstable compute is provisioned on the node. |`cpu_credits_remaining` |Count |Average |ServerName |Yes|
|CPU percent<p><p>CPU percent |`cpu_percent` |Percent |Average |ServerName |Yes|
|IOPS<p><p>IO operations per second |`iops` |Count |Average |ServerName |Yes|
|Memory percent<p><p>Memory percent |`memory_percent` |Percent |Average |ServerName |Yes|
|Network Out<p><p>Network Out across active connections |`network_bytes_egress` |Bytes |Total |ServerName |Yes|
|Network In<p><p>Network In across active connections |`network_bytes_ingress` |Bytes |Total |ServerName |Yes|
|Replication lag<p><p>Allows to see how much read replica nodes are behind their counterparts in the primary cluster |`replication_lag` |MilliSeconds |Average |ServerName |Yes|
|Storage percent<p><p>Storage percent |`storage_percent` |Percent |Average |ServerName |Yes|
|Storage used<p><p>Storage used |`storage_used` |Bytes |Average |ServerName |Yes|
|VM Cached Bandwidth Consumed Percentage<p><p>Percentage of cached disk bandwidth consumed by the VM |`vm_cached_bandwidth_percent` |Percent |Average |ServerName |Yes|
|VM Cached IOPS Consumed Percentage<p><p>Percentage of cached disk IOPS consumed by the VM |`vm_cached_iops_percent` |Percent |Average |ServerName |Yes|
|VM Uncached Bandwidth Consumed Percentage<p><p>Percentage of uncached disk bandwidth consumed by the VM |`vm_uncached_bandwidth_percent` |Percent |Average |ServerName |Yes|
|VM Uncached IOPS Consumed Percentage<p><p>Percentage of uncached disk IOPS consumed by the VM |`vm_uncached_iops_percent` |Percent |Average |ServerName |Yes|


<!--Gen Date:  Wed Jul 12 2023 17:59:09 GMT+0300 (Israel Daylight Time)-->