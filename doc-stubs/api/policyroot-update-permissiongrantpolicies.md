---
title: "Update permissionGrantPolicy"
description: "Update the properties of a permissionGrantPolicies object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update permissionGrantPolicy
Namespace: microsoft.graph

Update the properties of a permissionGrantPolicies object.

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
PATCH /policyRoot/permissionGrantPolicies
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object.

The following table shows the properties that are required when you update the [permissionGrantPolicy](../resources/permissiongrantpolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md)|
|displayName|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md)|



## Response

If successful, this method returns a `200 OK` response code and an updated [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_permissiongrantpolicies"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policyRoot/permissionGrantPolicies
Content-Type: application/json
Content-length: 163

{
  "@odata.type": "#microsoft.graph.permissionGrantPolicy",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK

Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.permissionGrantPolicy",
  "id": "10e6d77a-d77a-10e6-7ad7-e6107ad7e610",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String"
}
```
