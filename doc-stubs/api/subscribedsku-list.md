---
title: "List subscribedSkus"
description: "Get a list of the subscribedSku objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List subscribedSkus
Namespace: microsoft.graph

Get a list of the [subscribedSku](../resources/subscribedsku.md) objects and their properties.

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
GET /subscribedSkus
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

If successful, this method returns a `200 OK` response code and a collection of [subscribedSku](../resources/subscribedsku.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}
-->
``` http
GET https://graph.microsoft.com/beta/subscribedSkus
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Microsoft.DirectoryServices.subscribedSku)"
}
-->
``` http
HTTP/1.1 200 OK

Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#Microsoft.DirectoryServices.subscribedSku",
      "capabilityStatus": "String",
      "consumedUnits": "Integer",
      "id": "3d8d59de-59de-3d8d-de59-8d3dde598d3d",
      "prepaidUnits": {
        "@odata.type": "microsoft.graph.licenseUnitsDetail"
      },
      "servicePlans": [
        {
          "@odata.type": "microsoft.graph.servicePlanInfo"
        }
      ],
      "skuId": "Guid",
      "skuPartNumber": "String",
      "appliesTo": "String"
    }
  ]
}
```
