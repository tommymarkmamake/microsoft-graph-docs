---
title: "Create windowsFeatureUpdateCatalogItem"
description: "Create a new windowsFeatureUpdateCatalogItem object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create windowsFeatureUpdateCatalogItem
Namespace: microsoft.graph

Create a new [windowsFeatureUpdateCatalogItem](../resources/intune-windowsfeatureupdatecatalogitem.md) object.

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
POST ** Collection URI for microsoft.graph.windowsFeatureUpdateCatalogItem not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [windowsFeatureUpdateCatalogItem](../resources/intune-windowsfeatureupdatecatalogitem.md) object.

The following table shows the properties that are required when you create the [windowsFeatureUpdateCatalogItem](../resources/intune-windowsfeatureupdatecatalogitem.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description** Inherited from [windowsUpdateCatalogItem](../resources/intune-windowsupdatecatalogitem.md)|
|releaseDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [windowsUpdateCatalogItem](../resources/intune-windowsupdatecatalogitem.md)|
|version|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [windowsFeatureUpdateCatalogItem](../resources/intune-windowsfeatureupdatecatalogitem.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_windowsfeatureupdatecatalogitem_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.windowsFeatureUpdateCatalogItem not found
Content-Type: application/json
Content-length: 169

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateCatalogItem",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "version": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsFeatureUpdateCatalogItem"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateCatalogItem",
  "id": "05b8771b-771b-05b8-1b77-b8051b77b805",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "version": "String"
}
```
