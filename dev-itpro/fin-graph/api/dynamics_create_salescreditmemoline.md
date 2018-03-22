---
title: Create salesCreditMemoLines | Microsoft Docs
description: Creates a sales credit memo line object in Dynamics 365 for Financials.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen

ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 01/05/2018
ms.author: solsen
---

# Create salesCreditMemoLines
Create a sales credit memo line object in Dynamics 365 for Financials.

## HTTP request

```
POST /financials/companies({id})/salesCreditMemos({id})/salesCreditMemoLines
```

## Request headers

|Header|Value|
|------|-----|
|Authorization  |Bearer {token}. Required.    |
|Content-Type   |application/json    |

## Request body
In the request body, supply a JSON representation of a **salesCreditMemoLines** object.

## Response
If successful, this method returns ```201 Created``` response code and a **salesCreditMemoLines** object in the response body.

## Example

**Request**

Here is an example of a request.

```json
POST https://api.financials.dynamics.com/v1.0/api/beta/companies({id})/salesCreditMemos({id})/salesCreditMemoLines
Content-type: application/json

{
"itemId": "id-value",
"lineType": "Item",
"quantity": 9
}
```
## See also
[Graph Reference](../api/dynamics_graph_reference.md)  
[Working with [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)] in Microsoft Graph](../resources/dynamics_overview.md)  
[Enabling the APIs for Microsoft Dynamics NAV](../enabling-apis-for-dynamics-nav.md)  
[Endpoints for the APIs](../endpoints-apis-for-dynamics.md)  
[Error Codes](../dynamics_error_codes.md)  
[Sales credit memo line](../resources/dynamics_salescreditmemoline.md)  
[Get sales credit memo line](../api/dynamics_salescreditmemoline_get.md)  
[Update sales credit memo line](../api/dynamics_salescreditmemoline_update.md)  
[Delete sales credit memo line](../api/dynamics_salescreditmemoline_delete.md)  