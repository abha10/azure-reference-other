---
title: Azure Monitor Logs reference - AzureActivity
description: Reference for AzureActivity table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: edbaynash
author: EdB-MSFT
ms.date: 08/08/2023
---

# AzureActivity

 Entries from the Azure Activity log that provides insight into any subscription-level or management group level events that have occurred in Azure.

## Categories

- Azure Resources
- Audit
- Security
## Solutions

- LogManagement
## Resource types

- Azure AD Domain Services
- IoT Hub
- Azure Monitor autoscale settings
- Azure Databricks Services
- Azure Arc Provisioned Clusters
- Azure Arc Enabled Kubernetes
- Virtual Machine Scale Sets
- System Center Virtual Machine Manager
- Azure Stack HCI
- VMware
- Event Grid System Topics
- Event Grid Partner Topics
- Service Fabric Clusters
- Event Grid Partner Namespaces
- Azure Blockchain Service
- Azure Data Explorer Clusters
- Container Registries
- SignalR
- Storage Accounts
- Cognitive Services
- Azure Spring Apps
- Batch Accounts
- Analysis Services
- Workload Monitor
- Time Series Insights Environments
- Event Grid Domains
- Logic Apps
- API Management services
- Automation account
- Stream Analytics jobs
- Search Services
- Virtual Networks
- Virtual Private Network Gateways
- Virtual Network Gateways
- Traffic Manager Profiles
- Public IP Addresses
- Network Security Groups
- Network Interfaces
- Load Balancers
- Front Doors
- ExpressRoute Circuits
- Device Provisioning Services
- Azure Database for MariaDB Servers
- Azure Database for PostgreSQL Servers V2
- Azure Database for PostgreSQL Servers
- Azure Database for MySQL Servers
- SQL Databases
- SQL Servers
- SQL Managed Instances
- Data Share
- Power BI Embedded
- Data Lake Analytics
- Data Lake Storage Gen1
- Data factories
- Desktop Virtualization workspaces
- Bastions
- Desktop Virtualization Application Groups
- SignalR Service WebPubSub
- Microsoft.Purview/accounts
- Nexus Storage Appliances
- Nexus Clusters
- Nexus BareMetal Machines
- Azure Managed Instance for Apache Cassandra
- Azure Load Testing
- Kubernetes Services
- Key Vaults
- Azure Managed Workspace for Grafana
- Firewalls
- Event Hubs
- Recovery Services Vaults
- Event Grid Topics
- Project CI Workspace
- Azure Cosmos DB
- Communication Services
- Azure CloudHsm
- CDN Profiles
- Azure Cache for Redis
- Azure Attestation
- Azure Autonomous Development Platform workspace
- App Services
- Application Gateways
- Microsoft App Configuration
- Azure Digital Twins
- Relay
- Service Bus
- Azure Traffic Collector
- Azure Resource Group
- Azure Subscription
- Default schema for a resource
- Desktop Virtualization Host Pools
- Synapse Workspaces
- Azure Storage Mover
- Azure Managed Lustre
- Microsoft Graph Logs
- Media Services
- Machine Learning
- Machine Learning
- Virtual machines
- HDInsight Clusters
- Experiment Workspace
- Dev Centers
- Azure Database for PostgreSQL Flexible Servers
- Azure Database for MySQL Flexible Servers
- Dynamics 365 Customer Insights
- Container Apps
- Network Watcher - Connection Monitor
- Microsoft Connected Vehicle Platform
- Microsoft Connected Cache
- Chaos Experiment
- Bot Services
- Azure Virtual Network Manager
- Application Insights
- Azure API for FHIR




## Columns

| Column | Type | Description |
| --- | --- | --- |
| ActivityStatus | string |  |
| ActivityStatusValue | string | Status of the operation in display-friendly format. Common values include Started, In Progress, Succeeded, Failed, Active, Resolved. |
| ActivitySubstatus | string |  |
| ActivitySubstatusValue | string | Substatus of the operation  in display-friendly format. E.g. OK (HTTP Status Code: 200). |
| Authorization | string | Blob of RBAC properties of the event. Usually includes the “action”, “role” and “scope” properties. Stored as string. The use of Authorization_d should be preferred going forward. |
| Authorization_d | dynamic | Blob of RBAC properties of the event. Usually includes the “action”, “role” and “scope” properties. Stored as dynamic column. |
| _BilledSize | real | The record size in bytes |
| Caller | string | GUID of the caller. |
| CallerIpAddress | string | IP address of the user who has performed the operation UPN claim or SPN claim based on availability. |
| Category | string |  |
| CategoryValue | string | Category of the activity log e.g. Administrative, Policy, Security. |
| Claims | string | The JWT token used by Active Directory to authenticate the user or application to perform this operation in Resource Manager. The use of claims_d should be preferred going forward. |
| Claims_d | dynamic | The JWT token used by Active Directory to authenticate the user or application to perform this operation in Resource Manager. |
| CorrelationId | string | Usually a GUID in the string format. Events that share a correlationId belong to the same uber action. |
| EventDataId | string | Unique identifier of an event. |
| EventSubmissionTimestamp | datetime | Timestamp when the event became available for querying. |
| Hierarchy | string | Management group hierarchy of the management group or subscription that event belongs to. |
| HTTPRequest | string | Blob describing the Http Request. Usually includes the “clientRequestId”, “clientIpAddress” and “method” (HTTP method. For example, PUT). |
| _IsBillable | string | Specifies whether ingesting the data is billable. When _IsBillable is *false* ingestion isn't billed to your Azure account |
| Level | string | Level of the event. One of the following values: Critical, Error, Warning, Informational and Verbose. |
| OperationId | string | GUID of the operation |
| OperationName | string |  |
| OperationNameValue | string | Identifier of the operation e.g. Microsoft.Storage/storageAccounts/listAccountSas/action. |
| Properties | string | Set of \<Key Value\> pairs (i.e. Dictionary) describing the details of the event. Stored as string. Usage of Properties_d is recommended instead. |
| Properties_d | dynamic | Set of \<Key Value\> pairs (i.e. Dictionary) describing the details of the event. Stored as dynamic column. |
| Resource | string |  |
| ResourceGroup | string | Resource group name of the impacted resource. |
| ResourceId | string |  |
| _ResourceId | string | A unique identifier for the resource that the record is associated with |
| ResourceProvider | string |  |
| ResourceProviderValue | string | Id of the resource provider for the impacted resource - e.g. Microsoft.Storage. |
| SourceSystem | string | The type of agent the event was collected by. For example, *OpsManager* for Windows agent, either direct connect or Operations Manager, *Linux* for all Linux agents, or *Azure* for Azure Diagnostics |
| SubscriptionId | string | Subscription ID of the impacted resource. |
| _SubscriptionId | string | A unique identifier for the subscription that the record is associated with |
| TenantId | string | The Log Analytics workspace ID |
| TimeGenerated | datetime | Timestamp when the event was generated by the Azure service processing the request corresponding the event. |
| Type | string | The name of the table |
