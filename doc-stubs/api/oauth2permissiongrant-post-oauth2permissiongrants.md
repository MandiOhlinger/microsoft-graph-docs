---
title: "Create oAuth2PermissionGrant"
description: "Create a new oAuth2PermissionGrant object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create oAuth2PermissionGrant
Namespace: microsoft.graph

Create a new [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.

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
POST /oauth2PermissionGrants
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.

The following table shows the properties that are required when you create the [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).

|Property|Type|Description|
|:---|:---|:---|
|clientId|String|**TODO: Add Description**|
|consentType|String|**TODO: Add Description**|
|expiryTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|principalId|String|**TODO: Add Description**|
|resourceId|String|**TODO: Add Description**|
|scope|String|**TODO: Add Description**|
|startTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_oauth2permissiongrant_from_oauth2permissiongrants"
}
-->
``` http
POST https://graph.microsoft.com/beta/oauth2PermissionGrants
Content-Type: application/json
Content-length: 282

{
  "@odata.type": "#Microsoft.DirectoryServices.oAuth2PermissionGrant",
  "clientId": "String",
  "consentType": "String",
  "expiryTime": "String (timestamp)",
  "principalId": "String",
  "resourceId": "String",
  "scope": "String",
  "startTime": "String (timestamp)"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.oAuth2PermissionGrant"
}
-->
``` http
HTTP/1.1 201 Created

Content-Type: application/json
{
  "@odata.type": "#Microsoft.DirectoryServices.oAuth2PermissionGrant",
  "clientId": "String",
  "consentType": "String",
  "expiryTime": "String (timestamp)",
  "id": "a89f3bb1-3bb1-a89f-b13b-9fa8b13b9fa8",
  "principalId": "String",
  "resourceId": "String",
  "scope": "String",
  "startTime": "String (timestamp)"
}
```
