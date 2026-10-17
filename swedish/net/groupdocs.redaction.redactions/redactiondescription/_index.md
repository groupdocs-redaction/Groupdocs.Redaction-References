---
title: "RedactionDescription"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar information om en enskild förändringsåtgärd som utfördes under redigeringsprocessen."
type: docs
weight: 720
url: /sv/net/groupdocs.redaction.redactions/redactiondescription/
---
## RedactionDescription class

Representerar information om en enskild förändringsåtgärd som utfördes under redigeringsprocessen.

```csharp
public class RedactionDescription
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [RedactionDescription](redactiondescription#constructor_1)(RedactionType, RedactionActionType, string) | Initierar en ny instans av klassen RedactionDescription utan ersättningsinformation. |
| [RedactionDescription](redactiondescription#constructor)(RedactionType, RedactionActionType, RegionReplacementOptions, string) | Initierar en ny instans av klassen RedactionDescription med ersättningsinformation för bildområde. |
| [RedactionDescription](redactiondescription#constructor_2)(RedactionType, RedactionActionType, string, TextReplacement) | Initierar en ny instans av klassen RedactionDescription med ersättningsinformation. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ActionType](../../groupdocs.redaction.redactions/redactiondescription/actiontype) { get; } | Hämtar redigeringsoperationen: ersättning, rensning eller borttagning. |
| [Details](../../groupdocs.redaction.redactions/redactiondescription/details) { get; set; } | Hämtar eller anger valfri detaljinformation för objektet som redigeras. |
| [ImageAreaReplacement](../../groupdocs.redaction.redactions/redactiondescription/imageareareplacement) { get; } | Hämtar ersättningsinformationen för bildområdesredigeringar, returnerar null för textredigeringar. |
| [OriginalText](../../groupdocs.redaction.redactions/redactiondescription/originaltext) { get; } | Hämtar den matchade texten, om något uttryck har angetts. |
| [RedactionType](../../groupdocs.redaction.redactions/redactiondescription/redactiontype) { get; } | Hämtar typen av dokumentdata – text, metadata eller annotationer. |
| [Replacement](../../groupdocs.redaction.redactions/redactiondescription/replacement) { get; } | Hämtar ersättningsinformationen, kan vara null. |

### Anmärkningar

**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

### Se även

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
