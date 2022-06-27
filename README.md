# Welcome!

The goal of this repository is to share awesome KQL Queries that will help every Intune Administrator to filter for relevant informations and also present the data visually to interested parties in the form of a Azure Workbook.

This collection of KQL Querries include some of which I have created because there was a neccessitiy or usecase for it. Other Queries are from the Community that I found particulary interisting and worth to share. The ones from the community will also contain the weblink to the source and author.

Please feel free to share any feedback and suggestions on Twitter @ugurkocde!

-------------


  * [Audit (IntuneAuditLogs):](#audit--intuneauditlogs--)
  * [Compliance (IntuneDeviceComplianceOrg):](#compliance--intunedevicecomplianceorg--)
  * [Device (IntuneDevices):](#device--intunedevices--)
  * [Operational (IntuneOperationalLogs):](#operational--intuneoperationallogs--)
- [What is KQL?](#what-is-kql-)
- [How to get started with KQL and Intune:](#how-to-get-started-with-kql-and-intune-)
- [Useful Links from Microsoft and the Community for further deep-dive:](#useful-links-from-microsoft-and-the-community-for-further-deep-dive-)

-------------

I have created different categories based on the data tables from Intune to help you find the queries you want:

1. Audit
2. Compliance
3. Device
4. Operational

The data tables include the following informations:

## Audit (IntuneAuditLogs):

|       Column      |      Description      |
|:-----------------:|:---------------------:|
| Category          |                       |
| CorrelationId     |                       |
| Identity          |                       |
| OperationName     |                       |
| Properties        |                       |
| ResultDescription |                       |
| ResultType        |                       |
| SourceSystem      |                       |
| TimeGenerated     |                       |
| Type              | The name of the table |



## Compliance (IntuneDeviceComplianceOrg):

|          Column         |                                 Description                                 |
|:-----------------------:|:---------------------------------------------------------------------------:|
| ComplianceState         | The compliance state of the device.                                         |
| DeviceHealthThreatLevel | The device health threat level.                                             |
| DeviceId                | The Id of the device.                                                       |
| DeviceName              | The name of the device.                                                     |
| DeviceType              | The type of the device.                                                     |
| IMEI                    | The international mobile equipment identifier of the device.                |
| InGracePeriodUntil      | The device grace period end time.                                           |
| LastContact             | The date and time of last contact.                                          |
| ManagementAgents        | The management agents.                                                      |
| OS                      | The operating system of the device.                                         |
| OSDescription           | The operating system of the device.                                         |
| OSVersion               | The version of the operating system.                                        |
| OwnerType               | The type of owner.                                                          |
| _ResourceId             | A unique identifier for the resource that the record is associated with     |
| Result                  | The result of the operation.                                                |
| RetireAfterDatetime     | The retire after date time.                                                 |
| SerialNumber            | The serial number of the device                                             |
| SourceSystem            |                                                                             |
| _SubscriptionId         | A unique identifier for the subscription that the record is associated with |
| TenantId                |                                                                             |
| TimeGenerated           | Date and time when the report was generated.                                |
| Type                    | The name of the table                                                       |
| UPN                     | The user principal name.                                                    |
| UserEmail               | The user email address.                                                     |
| UserId                  | The Id of the user.                                                         |
| UserName                | The user name.                                                              |

## Device (IntuneDevices):

|          Column          |                                    Description                                   |
|:------------------------:|:--------------------------------------------------------------------------------:|
| AADTenantId              | The AAD Tenant ID                                                                |
| AndroidPatchLevel        | The Android patch level of the device                                            |
| BatchId                  | The unique ID for the exported report                                            |
| CategoryName             | The category name of the device                                                  |
| CompliantState           | The compliant state of the device                                                |
| CreatedDate              | The date and time of the device entry was created                                |
| DeviceId                 | The ID of the device                                                             |
| DeviceName               | The name of the device                                                           |
| DeviceRegistrationState  | The registration state of the device                                             |
| DeviceState              | The state of the device                                                          |
| EasID                    | The Emergency Alert System Identification of the device                          |
| EncryptionStatusString   | String describing whether the device is encrypted                                |
| GraphDeviceIsManaged     | Boolean describing whether the graph device is managed                           |
| IMEI                     | The international mobile equipment identifier of the device                      |
| InGracePeriodUntil       | The device grace period end time                                                 |
| IntuneAccountId          | The Intune Account ID                                                            |
| JailBroken               | String describing whether the device is jail broken                              |
| JoinType                 | The device join type                                                             |
| LastContact              | The date and time of last contact                                                |
| ManagedBy                | The authority that the device is managed by                                      |
| ManagedDeviceName        | The managed device name                                                          |
| Manufacturer             | The manufacturer of the device                                                   |
| MEID                     | The mobile equipment identifier of the device                                    |
| Model                    | The model of the device                                                          |
| OperationName            | The name of the operation                                                        |
| OS                       | The operating system of the device                                               |
| OSVersion                | The version of the operating system                                              |
| Ownership                | The ownership of the device                                                      |
| PhoneNumber              | The phone number                                                                 |
| PrimaryUser              | The ID of the primary user                                                       |
| ReferenceId              | The AAD Device ID                                                                |
| Result                   | The result of the operation                                                      |
| SerialNumber             | The serial number of the device                                                  |
| SkuFamily                | The stock-keeping unit family of the device                                      |
| SourceSystem             | Details of source system of the object being provisioned                         |
| Stats                    | Statistics about the export, including the number of records exported per export |
| StorageFree              | The free storage size of the device                                              |
| StorageTotal             | The total storage size of the device                                             |
| SubscriberCarrierNetwork | The subscriber carrier network                                                   |
| SupervisedStatusString   | String describing whether the device is supervised                               |
| TenantId                 |                                                                                  |
| TimeGenerated            | Date and time when the report was generated (UTC)                                |
| Type                     | The name of the table                                                            |
| UPN                      | The user principal name                                                          |
| UserEmail                | The user email address                                                           |
| UserName                 | The user name                                                                    |
| WifiMacAddress           | The WiFi MAC address of the device                                               |


## Operational (IntuneOperationalLogs):

|     Column    |      Description      |
|:-------------:|:---------------------:|
| Category      |                       |
| OperationName |                       |
| Properties    |                       |
| Result        |                       |
| SourceSystem  |                       |
| TimeGenerated |                       |
| Type          | The name of the table |


# What is KQL?

Kusto Query Language is a powerful tool to explore your data and discover patterns, identify anomalies and outliers, create statistical modeling, and more. The query uses schema entities that are organized in a hierarchy similar to SQL's: databases, tables, and columns.

A Kusto query is a read-only request to process data and return results. The request is stated in plain text, using a data-flow model that is easy to read, author, and automate. Kusto queries are made of one or more query statements.

Source: https://docs.microsoft.com/en-us/azure/data-explorer/kusto/query/


# How to get started with KQL and Intune:

Use the steps described on the following website to Connect your Endpoint Manager (Intune) with a Log Analytics Workspace to get started: https://shehanperera.com/2022/05/22/loganalytics-endpointmanager1/

!(https://shehanstechblog.files.wordpress.com/2022/05/image-46.png)


# Useful Links from Microsoft and the Community for further deep-dive:

MustLearnKQL from Rod Trent
More KQL Queries: https://github.com/rod-trent/MustLearnKQL and the Book (PDF): https://github.com/rod-trent/MustLearnKQL/blob/main/Book_Version/MustLearnKQL_Book.pdf

Example Queries:
https://github.com/reprise99/Sentinel-Queries
https://github.com/rod-trent/SentinelKQL