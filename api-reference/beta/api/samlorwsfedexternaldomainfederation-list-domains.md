---
title: "List domains"
description: "Get the list of all externalDomainName objects for a samlOrWsFedExternalDomainFederation."
author: "namkedia"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: apiPageType
---

# List domains
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the list of all [externalDomainName](../resources/externaldomainname.md) objects for a [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md).

## Permissions

Choose the permission or permissions marked as least privileged for this API. Use a higher privileged permission or permissions [only if your app requires it](/graph/permissions-overview#best-practices-for-using-microsoft-graph-permissions). For details about delegated and application permissions, see [Permission types](/graph/permissions-overview#permission-types). To learn more about these permissions, see the [permissions reference](/graph/permissions-reference).

<!-- { "blockType": "permissions", "name": "samlorwsfedexternaldomainfederation_list_domains" } -->
[!INCLUDE [permissions-table](../includes/permissions/samlorwsfedexternaldomainfederation-list-domains-permissions.md)]

The work or school account needs to belong to one of the following [Microsoft Entra roles](/entra/identity/role-based-access-control/permissions-reference?toc=%2Fgraph%2Ftoc.json):

* Global Administrator
* External Identity Provider Administrator

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /directory/federationConfigurations/microsoft.graph.samlOrWsFedExternalDomainFederation/{samlOrWsFedExternalDomainFederation ID}/domains
```

## Request headers

|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required. Learn more about [authentication and authorization](/graph/auth/auth-concepts).|

## Request body

Don't supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [externalDomainName](../resources/externaldomainname.md) objects in the response body.

## Examples

### Request


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_externaldomainname_e1"
}
-->

``` http
GET https://graph.microsoft.com/beta/directory/federationConfigurations/microsoft.graph.samlOrWsFedExternalDomainFederation/f1e11a04-0244-4592-99df-b01cfaadce15/domains
```

# [Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-externaldomainname-e1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-externaldomainname-e1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### Response

The following example shows the response.
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.externalDomainName)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directory/federationConfigurations/microsoft.graph.samlOrWsFedExternalDomainFederation('f1e11a04-0244-4592-99df-b01cfaadce15')/domains",
    "value": [
        {
            "id": "fabrikam.com"
        },
        {
            "id": "contoso.com"
        }
    ]
}
```
