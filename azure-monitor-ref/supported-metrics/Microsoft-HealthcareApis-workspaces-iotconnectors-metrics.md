---
title: Supported metrics - Microsoft.HealthcareApis/workspaces/iotconnectors
description: Reference for Microsoft.HealthcareApis/workspaces/iotconnectors metrics in Azure Monitor.
ms.topic: reference
ms.service: azure-monitor
ms.author: edbaynash
author: EdB-MSFT
ms.date: 07/12/2023
---
# Supported metrics for Microsoft.HealthcareApis/workspaces/iotconnectors  
<!-- Data source : arm-->


The following table lists the metrics available for the Microsoft.HealthcareApis/workspaces/iotconnectors resource type.

  

**Table headings**
  
**Metric** - Metric display name follows by a description of the metric. The displayname appears in the Azure portal.  
**Name** - The name of the metric as referred to in the REST API.  
**Unit** - The default units used for the metric.  
**Aggregation** - The default aggregation type for this metric. Valid values: Average, Minimum, Maximum, Total, Count.  
**Dimensions** - Dimensions available. For more information, see (link to dimensions information).  
**DS Export**- Whether the metric is exportable to Azure Monitor Logs via Diagnostic Settings.  You can access all metrics via the REST API.  
  
  
|Metric|Name|Unit|Aggregation|Dimensions|DS Export|
|---|---|---|---|---|---|
|Number of Incoming Messages<p><p>The total number of messages received by the MedTech service prior to any normalization |`DeviceEvent` |Count |Sum |Operation, ResourceName |Yes|
|Average Normalize Stage Latency<p><p>The average time between an event's ingestion time and the time the event is processed for normalization. |`DeviceEventProcessingLatencyMs` |Milliseconds |Average |Operation, ResourceName |Yes|
|Number of Dropped Events<p><p>The number of input device events with no normalized events |`DroppedEvent` |Count |Sum |Operation, ResourceName |Yes|
|Number of FHIR resources saved<p><p>The total number of FHIR resources saved by the MedTech service |`FhirResourceSaved` |Count |Sum |Operation, ResourceName, Name |Yes|
|MedTech Service Health Status<p><p>Health checks which indicate the overall health of the MedTech service |`IotConnectorStatus` |Percent |Average |Operation, ResourceName, HealthCheckName |Yes|
|Number of Measurements<p><p>The number of normalized value readings received by the FHIR conversion stage of the MedTech service |`Measurement` |Count |Sum |Operation, ResourceName |Yes|
|Number of Message Groups<p><p>The total number of unique groupings of measurements across type, device, patient, and configured time period generated by the FHIR conversion stage. |`MeasurementGroup` |Count |Sum |Operation, ResourceName |Yes|
|Average Group Stage Latency<p><p>The time period between when the MedTech service received the device data and when the data is processed by the FHIR conversion stage. |`MeasurementIngestionLatencyMs` |Milliseconds |Average |Operation, ResourceName |Yes|
|Number of Normalized Messages<p><p>The total number of mapped normalized values outputted from the normalization stage of the MedTech service |`NormalizedEvent` |Count |Sum |Operation, ResourceName |Yes|
|Total Error Count<p><p>The total number of errors logged by the MedTech service |`TotalErrors` |Count |Sum |Name, Operation, ErrorType, ErrorSeverity, ResourceName |Yes|


<!--Gen Date:  Wed Jul 12 2023 17:59:09 GMT+0300 (Israel Daylight Time)-->