---
title: "List domainDnsRecords"
description: "Get the domainDnsRecord resources from the serviceConfigurationRecords navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List domainDnsRecords
Namespace: microsoft.graph

Get the domainDnsRecord resources from the serviceConfigurationRecords navigation property.

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
GET /domainDnsRecords
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

If successful, this method returns a `200 OK` response code and a collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_domaindnsrecord"
}
-->
``` http
GET https://graph.microsoft.com/beta/domainDnsRecords
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Microsoft.DirectoryServices.domainDnsRecord)"
}
-->
``` http
HTTP/1.1 200 OK

Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#Microsoft.DirectoryServices.domainDnsRecord",
      "id": "e7aade31-de31-e7aa-31de-aae731deaae7",
      "isOptional": "Boolean",
      "label": "String",
      "recordType": "String",
      "supportedService": "String",
      "ttl": "Integer"
    }
  ]
}
```
