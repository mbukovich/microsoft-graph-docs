---
title: "accessPackageMultipleChoiceQuestion resource type"
description: "Subclass of accessPackageQuestion that has multiple choice as the question's answer format"
author: "markwahl-msft"
localization_priority: Normal
ms.prod: "microsoft-identity-platform"
doc_type: resourcePageType
---

# accessPackageMultipleChoiceQuestion resource type

Namespace: microsoft.graph

A child of `accessPackageQuestion` which presents multiple answer options a requestor must choose an answer from.

Inherits from [accessPackageQuestion](../resources/accesspackagequestion.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowsMultipleSelection|Boolean|Whether requestor can select multiple choices as their answer.|
|choices|[accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md) collection|List of answer choices.|
|id|String|ID of the question. Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md)|
|isRequired|Boolean|Whether the requestor is required to supply an answer or not. Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md)|
|sequence|Int32|Relative position of this question when displaying a list of questions to the requestor. Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md)|
|text|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|The text of the question to show the requestor. Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md)|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageMultipleChoiceQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
  "id": "String (identifier)",
  "isRequired": "Boolean",
  "text": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  },
  "sequence": "Integer",
  "choices": [
    {
      "@odata.type": "microsoft.graph.accessPackageAnswerChoice"
    }
  ],
  "allowsMultipleSelection": "Boolean"
}
```
