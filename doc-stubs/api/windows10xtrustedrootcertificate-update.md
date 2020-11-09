---
title: "Update windows10XTrustedRootCertificate"
description: "Update the properties of a windows10XTrustedRootCertificate object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update windows10XTrustedRootCertificate
Namespace: microsoft.graph

Update the properties of a [windows10XTrustedRootCertificate](../resources/windows10xtrustedrootcertificate.md) object.

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
PATCH ** Entity URI for microsoft.graph.windows10XTrustedRootCertificate not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [windows10XTrustedRootCertificate](../resources/windows10xtrustedrootcertificate.md) object.

The following table shows the properties that are required when you create the [windows10XTrustedRootCertificate](../resources/windows10xtrustedrootcertificate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|version|Int32|**TODO: Add Description** Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-devicemanagementresourceaccessprofilebase.md)|
|displayName|String|**TODO: Add Description** Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-devicemanagementresourceaccessprofilebase.md)|
|description|String|**TODO: Add Description** Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-devicemanagementresourceaccessprofilebase.md)|
|creationDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-devicemanagementresourceaccessprofilebase.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-devicemanagementresourceaccessprofilebase.md)|
|roleScopeTagIds|String collection|**TODO: Add Description** Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-devicemanagementresourceaccessprofilebase.md)|
|trustedRootCertificate|Binary|**TODO: Add Description**|
|certFileName|String|**TODO: Add Description**|
|destinationStore|certificateDestinationStore|**TODO: Add Description**. Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [windows10XTrustedRootCertificate](../resources/windows10xtrustedrootcertificate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_windows10xtrustedrootcertificate"
}
-->
``` http
PATCH https://graph.microsoft.com/beta** Entity URI for microsoft.graph.windows10XTrustedRootCertificate not found
Content-Type: application/json
Content-length: 345

{
  "@odata.type": "#microsoft.graph.windows10XTrustedRootCertificate",
  "version": "Integer",
  "displayName": "String",
  "description": "String",
  "creationDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "trustedRootCertificate": "Binary",
  "certFileName": "String",
  "destinationStore": "String"
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
  "@odata.type": "#microsoft.graph.windows10XTrustedRootCertificate",
  "id": "db5cb92a-b92a-db5c-2ab9-5cdb2ab95cdb",
  "version": "Integer",
  "displayName": "String",
  "description": "String",
  "creationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "trustedRootCertificate": "Binary",
  "certFileName": "String",
  "destinationStore": "String"
}
```
