---
title: "orgContact resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# orgContact resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [directoryObject](../resources/directoryobject.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List orgContacts](../api/orgcontact-list.md)|[orgContact](../resources/orgcontact.md) collection|Get a list of the [orgContact](../resources/orgcontact.md) objects and their properties.|
|[Create orgContact](../api/orgcontact-post-contacts.md)|[orgContact](../resources/orgcontact.md)|Create a new [orgContact](../resources/orgcontact.md) object.|
|[Get orgContact](../api/orgcontact-get.md)|[orgContact](../resources/orgcontact.md)|Read the properties and relationships of an [orgContact](../resources/orgcontact.md) object.|
|[Update orgContact](../api/orgcontact-update.md)|[orgContact](../resources/orgcontact.md)|Update the properties of an [orgContact](../resources/orgcontact.md) object.|
|[Delete orgContact](../api/orgcontact-delete.md)|None|Deletes an [orgContact](../resources/orgcontact.md) object.|
|[delta](../api/orgcontact-delta.md)|[orgContact](../resources/orgcontact.md) collection|**TODO: Add Description**|
|[checkMemberGroups](../api/orgcontact-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/orgcontact-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/orgcontact-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/orgcontact-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/orgcontact-restore.md)|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|
|[List directoryObjects](../api/orgcontact-list-directreports.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObject resources from the directReports navigation property.|
|[Add directoryObject](../api/orgcontact-post-directreports.md)|[directoryObject](../resources/directoryobject.md)|Add directReports by posting to the directReports collection.|
|[List directoryObjects](../api/orgcontact-list-manager.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObject resources from the manager navigation property.|
|[Add directoryObject](../api/orgcontact-post-manager.md)|[directoryObject](../resources/directoryobject.md)|Add manager by posting to the manager collection.|
|[List directoryObjects](../api/orgcontact-list-memberof.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObject resources from the memberOf navigation property.|
|[Add directoryObject](../api/orgcontact-post-memberof.md)|[directoryObject](../resources/directoryobject.md)|Add memberOf by posting to the memberOf collection.|
|[List directoryObjects](../api/orgcontact-list-transitivememberof.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObject resources from the transitiveMemberOf navigation property.|
|[Add directoryObject](../api/orgcontact-post-transitivememberof.md)|[directoryObject](../resources/directoryobject.md)|Add transitiveMemberOf by posting to the transitiveMemberOf collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|addresses|[physicalOfficeAddress](../resources/physicalofficeaddress.md) collection|**TODO: Add Description**|
|companyName|String|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|department|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|givenName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|jobTitle|String|**TODO: Add Description**|
|mail|String|**TODO: Add Description**|
|mailNickname|String|**TODO: Add Description**|
|onPremisesLastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](../resources/onpremisesprovisioningerror.md) collection|**TODO: Add Description**|
|onPremisesSyncEnabled|Boolean|**TODO: Add Description**|
|phones|[phone](../resources/phone.md) collection|**TODO: Add Description**|
|proxyAddresses|String collection|**TODO: Add Description**|
|surname|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|directReports|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|manager|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|
|memberOf|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|transitiveMemberOf|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.orgContact",
  "baseType": "Microsoft.DirectoryServices.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.orgContact",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "addresses": [
    {
      "@odata.type": "microsoft.graph.physicalOfficeAddress"
    }
  ],
  "companyName": "String",
  "department": "String",
  "displayName": "String",
  "givenName": "String",
  "jobTitle": "String",
  "mail": "String",
  "mailNickname": "String",
  "onPremisesSyncEnabled": "Boolean",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError"
    }
  ],
  "phones": [
    {
      "@odata.type": "microsoft.graph.phone"
    }
  ],
  "proxyAddresses": [
    "String"
  ],
  "surname": "String"
}
```
