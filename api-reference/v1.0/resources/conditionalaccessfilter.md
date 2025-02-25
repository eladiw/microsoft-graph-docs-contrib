---
title: "conditionalAccessFilter resource type"
description: "Represents filter in the policy scope."
ms.localizationpriority: medium
author: "SanDeo-MSFT"
ms.prod: "identity-and-sign-in"
doc_type: resourcePageType
---

# conditionalAccessFilter resource type

Namespace: microsoft.graph

Represents filter in the policy scope.

## Properties

| Property     | Type        | Description |
|:-------------|:------------|:------------|
| mode | filterMode | Mode to use for the filter. Possible values are `include` or `exclude`. |
| rule | String | Rule syntax is similar to that used for membership rules for groups in Azure Active Directory (Azure AD). For details, see [rules with multiple expressions](/azure/active-directory/enterprise-users/groups-dynamic-membership#rules-with-multiple-expressions) |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "mode",
    "rule"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessFilter",
  "baseType": null
}-->

```json
{
  "mode": "String",
  "rule": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessFilter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


