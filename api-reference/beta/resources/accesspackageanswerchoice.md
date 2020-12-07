---
title: "accessPackageAnswerChoice resource type"
description: "An answer option for an accessPackageMultipleChoiceQuestion."
author: "markwahl-msft"
localization_priority: Normal
ms.prod: "microsoft-identity-platform"
doc_type: resourcePageType
---

# accessPackageAnswerChoice resource type

Namespace: microsoft.graph

Indicates an answer option for an [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md). Multiple accessPackageAnswerChoices can be added to an [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|:---|:---|
|actualValue|String|The actual value of the selected choice. This is typically a string value which is understable by applications.|Yes|No|
|displayValue|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|The localized display values shown to the requestor and approvers.|Yes|No|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAnswerChoice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAnswerChoice",
  "actualValue": "String",
  "displayValue": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  }
}
```