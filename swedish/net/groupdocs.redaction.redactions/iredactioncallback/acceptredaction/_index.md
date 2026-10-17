---
title: "AcceptRedaction"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Detta anrop utlöses precis innan någon redigering tillämpas på dokumentet och möjliggör att logga eller förbjuda det."
type: docs
weight: 10
url: /sv/net/groupdocs.redaction.redactions/iredactioncallback/acceptredaction/
---
## IRedactionCallback.AcceptRedaction method

Detta anrop utlöses precis innan någon redigering tillämpas på dokumentet och möjliggör att logga eller förbjuda det.

```csharp
public bool AcceptRedaction(RedactionDescription description)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| beskrivning | RedactionDescription | Innehåller information om en viss matchningstyp, kriterier, text och position |

### Returvärde

Returnera true för att acceptera eller false för att avvisa en viss matchningsredigering

### Se även

* class [RedactionDescription](../../redactiondescription)
* interface [IRedactionCallback](../../iredactioncallback)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
