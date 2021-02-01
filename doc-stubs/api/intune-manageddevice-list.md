---
title: "List managedDevices"
description: "Get a list of the managedDevice objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List managedDevices
Namespace: microsoft.graph

Get a list of the [managedDevice](../resources/manageddevice.md) objects and their properties.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/managedDevices
GET /users/{usersId}/managedDevices
GET /deviceManagement/managedDevices
GET /deviceManagement/comanagedDevices
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [managedDevice](../resources/manageddevice.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_manageddevice"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/managedDevices
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedDevice)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDevice",
      "id": "05fe4723-4723-05fe-2347-fe052347fe05",
      "userId": "String",
      "deviceName": "String",
      "hardwareInformation": {
        "@odata.type": "microsoft.graph.hardwareInformation"
      },
      "ownerType": "String",
      "managedDeviceOwnerType": "String",
      "deviceActionResults": [
        {
          "@odata.type": "microsoft.graph.deviceActionResult"
        }
      ],
      "managementState": "String",
      "enrolledDateTime": "String (timestamp)",
      "lastSyncDateTime": "String (timestamp)",
      "chassisType": "String",
      "operatingSystem": "String",
      "deviceType": "String",
      "complianceState": "String",
      "jailBroken": "String",
      "managementAgent": "String",
      "osVersion": "String",
      "easActivated": "Boolean",
      "easDeviceId": "String",
      "easActivationDateTime": "String (timestamp)",
      "aadRegistered": "Boolean",
      "azureADRegistered": "Boolean",
      "deviceEnrollmentType": "String",
      "lostModeState": "String",
      "activationLockBypassCode": "String",
      "emailAddress": "String",
      "azureActiveDirectoryDeviceId": "String",
      "azureADDeviceId": "String",
      "deviceRegistrationState": "String",
      "deviceCategoryDisplayName": "String",
      "isSupervised": "Boolean",
      "exchangeLastSuccessfulSyncDateTime": "String (timestamp)",
      "exchangeAccessState": "String",
      "exchangeAccessStateReason": "String",
      "remoteAssistanceSessionUrl": "String",
      "remoteAssistanceSessionErrorDetails": "String",
      "isEncrypted": "Boolean",
      "userPrincipalName": "String",
      "model": "String",
      "manufacturer": "String",
      "imei": "String",
      "complianceGracePeriodExpirationDateTime": "String (timestamp)",
      "serialNumber": "String",
      "phoneNumber": "String",
      "androidSecurityPatchLevel": "String",
      "userDisplayName": "String",
      "configurationManagerClientEnabledFeatures": {
        "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
      },
      "wiFiMacAddress": "String",
      "deviceHealthAttestationState": {
        "@odata.type": "microsoft.graph.deviceHealthAttestationState"
      },
      "subscriberCarrier": "String",
      "meid": "String",
      "totalStorageSpaceInBytes": "Integer",
      "freeStorageSpaceInBytes": "Integer",
      "managedDeviceName": "String",
      "partnerReportedThreatState": "String",
      "retireAfterDateTime": "String (timestamp)",
      "usersLoggedOn": [
        {
          "@odata.type": "microsoft.graph.loggedOnUser"
        }
      ],
      "preferMdmOverGroupPolicyAppliedDateTime": "String (timestamp)",
      "autopilotEnrolled": "Boolean",
      "requireUserEnrollmentApproval": "Boolean",
      "managementCertificateExpirationDate": "String (timestamp)",
      "iccid": "String",
      "udid": "String",
      "roleScopeTagIds": [
        "String"
      ],
      "windowsActiveMalwareCount": "Integer",
      "windowsRemediatedMalwareCount": "Integer",
      "notes": "String",
      "configurationManagerClientHealthState": {
        "@odata.type": "microsoft.graph.configurationManagerClientHealthState"
      },
      "configurationManagerClientInformation": {
        "@odata.type": "microsoft.graph.configurationManagerClientInformation"
      },
      "ethernetMacAddress": "String",
      "physicalMemoryInBytes": "Integer",
      "processorArchitecture": "String",
      "specificationVersion": "String",
      "joinType": "String",
      "skuFamily": "String",
      "skuNumber": "Integer",
      "managementFeatures": "String"
    }
  ]
}
```
