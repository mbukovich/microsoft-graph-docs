---
title: "List temporaryAccessPassMethods"
description: "Get the temporaryAccessPassAuthenticationMethod resources from the temporaryAccessPassMethods navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List temporaryAccessPassMethods
Namespace: microsoft.graph

Get the temporaryAccessPassAuthenticationMethod resources from the temporaryAccessPassMethods navigation property.

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
GET /user/authentication/temporaryAccessPassMethods
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

If successful, this method returns a `200 OK` response code and a collection of [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_temporaryaccesspassauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/user/authentication/temporaryAccessPassMethods
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.strongAuthentication.temporaryAccessPassAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.strongAuthentication.temporaryAccessPassAuthenticationMethod",
      "id": "30fd0dfc-0dfc-30fd-fc0d-fd30fc0dfd30",
      "temporaryAccessPass": "String",
      "createdDateTime": "String (timestamp)",
      "startDateTime": "String (timestamp)",
      "lifetimeInMinutes": "Integer"
    }
  ]
}
```
