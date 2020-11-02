---
title: "Create resourceSpecificPermissionGrant"
description: "Create a new resourceSpecificPermissionGrant object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create resourceSpecificPermissionGrant
Namespace: microsoft.graph

Create a new [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from most to least privileged)|
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
POST /permissionGrants
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object.

The following table shows the properties that are required when you create the [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|clientId|String|**TODO: Add Description**|
|clientAppId|String|**TODO: Add Description**|
|resourceAppId|String|**TODO: Add Description**|
|permissionType|String|**TODO: Add Description**|
|permission|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_resourcespecificpermissiongrant_from_permissiongrants"
}
-->
``` http
POST https://graph.microsoft.com/beta/permissionGrants
Content-Type: application/json
Content-length: 270

{
  "@odata.type": "#Microsoft.DirectoryServices.resourceSpecificPermissionGrant",
  "deletedDateTime": "String (timestamp)",
  "clientId": "String",
  "clientAppId": "String",
  "resourceAppId": "String",
  "permissionType": "String",
  "permission": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.resourceSpecificPermissionGrant"
}
-->
``` http
HTTP/1.1 201 Created

Content-Type: application/json
{
  "@odata.type": "#Microsoft.DirectoryServices.resourceSpecificPermissionGrant",
  "id": "c493c033-c033-c493-33c0-93c433c093c4",
  "deletedDateTime": "String (timestamp)",
  "clientId": "String",
  "clientAppId": "String",
  "resourceAppId": "String",
  "permissionType": "String",
  "permission": "String"
}
```
