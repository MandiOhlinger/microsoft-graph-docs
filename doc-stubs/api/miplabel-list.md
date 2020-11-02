---
title: "List mipLabels"
description: "Get a list of the mipLabel objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List mipLabels
Namespace: microsoft.graph

Get a list of the [mipLabel](../resources/miplabel.md) objects and their properties.

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
GET /mipLabels
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

If successful, this method returns a `200 OK` response code and a collection of [mipLabel](../resources/miplabel.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_miplabel"
}
-->
``` http
GET https://graph.microsoft.com/beta/mipLabels
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Microsoft.DirectoryServices.mipLabel)"
}
-->
``` http
HTTP/1.1 200 OK

Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#Microsoft.DirectoryServices.mipLabel",
      "id": "f3e65f60-5f60-f3e6-605f-e6f3605fe6f3",
      "deletedDateTime": "String (timestamp)",
      "labelId": "String",
      "displayName": "String",
      "protectGroupAction": {
        "@odata.type": "microsoft.graph.mipProtectGroupLabelAction"
      }
    }
  ]
}
```
