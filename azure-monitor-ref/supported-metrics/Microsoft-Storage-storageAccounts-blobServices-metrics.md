---
title: Supported metrics - Microsoft.Storage/storageAccounts/blobServices
description: Reference for Microsoft.Storage/storageAccounts/blobServices metrics in Azure Monitor.
ms.topic: reference
ms.service: azure-monitor
ms.author: edbaynash
author: EdB-MSFT
ms.date: 07/12/2023
---
# Supported metrics for Microsoft.Storage/storageAccounts/blobServices  
<!-- Data source : naam-->


The following table lists the metrics available for the Microsoft.Storage/storageAccounts/blobServices resource type.

  

**Table headings**
  
**Metric** - Metric display name follows by a description of the metric. The displayname appears in the Azure portal.  
**Name** - The name of the metric as referred to in the REST API.  
**Unit** - The default units used for the metric.  
**Aggregation** - The default aggregation type for this metric. Valid values: Average, Minimum, Maximum, Total, Count.  
**Dimensions** - Dimensions available. For more information, see (link to dimensions information).  
**DS Export**- Whether the metric is exportable to Azure Monitor Logs via Diagnostic Settings.  You can access all metrics via the REST API.  
  
  
|Metric|Name|Unit|Aggregation|Dimensions|DS Export|
|---|---|---|---|---|---|
|Availability<p><p>The percentage of availability for the storage service or the specified API operation. Availability is calculated by taking the TotalBillableRequests value and dividing it by the number of applicable requests, including those that produced unexpected errors. All unexpected errors result in reduced availability for the storage service or the specified API operation. |`Availability` |Percent |Average |GeoType, ApiName, Authentication |Yes|
|Blob Capacity<p><p>The amount of storage used by the storage account's Blob service in bytes. |`BlobCapacity` |Bytes |Average |BlobType, Tier |No|
|Blob Count<p><p>The number of blob objects stored in the storage account. |`BlobCount` |Count |Average |BlobType, Tier |No|
|Blob Provisioned Size<p><p>The amount of storage provisioned in the storage account's Blob service in bytes. |`BlobProvisionedSize` |Bytes |Average |BlobType, Tier |No|
|Blob Container Count<p><p>The number of containers in the storage account. |`ContainerCount` |Count |Average |No Dimensions |Yes|
|Egress<p><p>The amount of egress data. This number includes egress to external client from Azure Storage as well as egress within Azure. As a result, this number does not reflect billable egress. |`Egress` |Bytes |Total |GeoType, ApiName, Authentication |Yes|
|Index Capacity<p><p>The amount of storage used by Azure Data Lake Storage Gen2 hierarchical index. |`IndexCapacity` |Bytes |Average |No Dimensions |No|
|Ingress<p><p>The amount of ingress data, in bytes. This number includes ingress from an external client into Azure Storage as well as ingress within Azure. |`Ingress` |Bytes |Total |GeoType, ApiName, Authentication |Yes|
|Success E2E Latency<p><p>The average end-to-end latency of successful requests made to a storage service or the specified API operation, in milliseconds. This value includes the required processing time within Azure Storage to read the request, send the response, and receive acknowledgment of the response. |`SuccessE2ELatency` |MilliSeconds |Average |GeoType, ApiName, Authentication |Yes|
|Success Server Latency<p><p>The average time used to process a successful request by Azure Storage. This value does not include the network latency specified in SuccessE2ELatency. |`SuccessServerLatency` |MilliSeconds |Average |GeoType, ApiName, Authentication |Yes|
|Transactions<p><p>The number of requests made to a storage service or the specified API operation. This number includes successful and failed requests, as well as requests which produced errors. Use ResponseType dimension for the number of different type of response. |`Transactions` |Count |Total |ResponseType, GeoType, ApiName, Authentication, TransactionType |Yes|


<!--Gen Date:  Wed Jul 12 2023 17:59:09 GMT+0300 (Israel Daylight Time)-->