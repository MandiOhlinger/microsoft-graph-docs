---
title: "Create directoryRoleTemplate"
description: "Create a new directoryRoleTemplate object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create directoryRoleTemplate
Namespace: microsoft.graph

Create a new [directoryRoleTemplate](../resources/directoryroletemplate.md) object.

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
POST /directoryRoleTemplates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [directoryRoleTemplate](../resources/directoryroletemplate.md) object.

The following table shows the properties that are required when you create the [directoryRoleTemplate](../resources/directoryroletemplate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [directoryRoleTemplate](../resources/directoryroletemplate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_directoryroletemplate_from_directoryroletemplates"
}
-->
``` http
POST https://graph.microsoft.com/beta/directoryRoleTemplates
Content-Type: application/json
Content-length: 175

{
  "@odata.type": "#Microsoft.DirectoryServices.directoryRoleTemplate",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.directoryRoleTemplate"
}
-->
``` http
HTTP/1.1 201 Created

Content-Type: application/json
{
  "@odata.type": "#Microsoft.DirectoryServices.directoryRoleTemplate",
  "id": "97f9f97d-f97d-97f9-7df9-f9977df9f997",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String"
}
```
