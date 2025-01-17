---
title: Supported metrics - Microsoft.HealthcareApis/services
description: Reference for Microsoft.HealthcareApis/services metrics in Azure Monitor.
ms.topic: reference
ms.service: azure-monitor
ms.author: edbaynash
author: EdB-MSFT
ms.date: 07/12/2023
---
# Supported metrics for Microsoft.HealthcareApis/services  
<!-- Data source : arm-->


The following table lists the metrics available for the Microsoft.HealthcareApis/services resource type.

  

**Table headings**
  
**Metric** - Metric display name follows by a description of the metric. The displayname appears in the Azure portal.  
**Name** - The name of the metric as referred to in the REST API.  
**Unit** - The default units used for the metric.  
**Aggregation** - The default aggregation type for this metric. Valid values: Average, Minimum, Maximum, Total, Count.  
**Dimensions** - Dimensions available. For more information, see (link to dimensions information).  
**DS Export**- Whether the metric is exportable to Azure Monitor Logs via Diagnostic Settings.  You can access all metrics via the REST API.  
  
  
|Metric|Name|Unit|Aggregation|Dimensions|DS Export|
|---|---|---|---|---|---|
|Availability<p><p>The availability rate of the service. |`Availability` |Percent |Average |No Dimensions |Yes|
|Cosmos DB Collection Size<p><p>The size of the backing Cosmos DB collection, in bytes. |`CosmosDbCollectionSize` |Bytes |Total |No Dimensions |Yes|
|Cosmos DB Index Size<p><p>The size of the backing Cosmos DB collection's index, in bytes. |`CosmosDbIndexSize` |Bytes |Total |No Dimensions |Yes|
|Cosmos DB RU usage<p><p>The RU usage of requests to the service's backing Cosmos DB. |`CosmosDbRequestCharge` |Count |Total |Operation, ResourceType |Yes|
|Service Cosmos DB requests<p><p>The total number of requests made to a service's backing Cosmos DB. |`CosmosDbRequests` |Count |Sum |Operation, ResourceType |Yes|
|Service Cosmos DB throttle rate<p><p>The total number of 429 responses from a service's backing Cosmos DB. |`CosmosDbThrottleRate` |Count |Sum |Operation, ResourceType |Yes|
|Number of Incoming Messages<p><p>The total number of messages received by the Azure IoT Connector for FHIR prior to any normalization. |`IoTConnectorDeviceEvent` |Count |Sum |Operation, ConnectorName |Yes|
|Average Normalize Stage Latency<p><p>The average time between an event's ingestion time and the time the event is processed for normalization. |`IoTConnectorDeviceEventProcessingLatencyMs` |Milliseconds |Average |Operation, ConnectorName |Yes|
|Number of Measurements<p><p>The number of normalized value readings received by the FHIR conversion stage of the Azure IoT Connector for FHIR. |`IoTConnectorMeasurement` |Count |Sum |Operation, ConnectorName |Yes|
|Number of Message Groups<p><p>The total number of unique groupings of measurements across type, device, patient, and configured time period generated by the FHIR conversion stage. |`IoTConnectorMeasurementGroup` |Count |Sum |Operation, ConnectorName |Yes|
|Average Group Stage Latency<p><p>The time period between when the IoT Connector received the device data and when the data is processed by the FHIR conversion stage. |`IoTConnectorMeasurementIngestionLatencyMs` |Milliseconds |Average |Operation, ConnectorName |Yes|
|Number of Normalized Messages<p><p>The total number of mapped normalized values outputted from the normalization stage of the the Azure IoT Connector for FHIR. |`IoTConnectorNormalizedEvent` |Count |Sum |Operation, ConnectorName |Yes|
|Total Error Count<p><p>The total number of errors logged by the Azure IoT Connector for FHIR |`IoTConnectorTotalErrors` |Count |Sum |Name, Operation, ErrorType, ErrorSeverity, ConnectorName |Yes|
|Total Errors<p><p>The total number of internal server errors encountered by the service. |`TotalErrors` |Count |Sum |Protocol, StatusCode, StatusCodeClass, StatusCodeText |Yes|
|Total Latency<p><p>The response latency of the service. |`TotalLatency` |Milliseconds |Average |Protocol |Yes|
|Total Requests<p><p>The total number of requests received by the service. |`TotalRequests` |Count |Sum |Protocol |Yes|


<!--Gen Date:  Wed Jul 12 2023 17:59:09 GMT+0300 (Israel Daylight Time)-->