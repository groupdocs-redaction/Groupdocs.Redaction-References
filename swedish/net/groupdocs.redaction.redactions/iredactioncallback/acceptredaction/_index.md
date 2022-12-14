---
title: AcceptRedaction
second_title: GroupDocs.Redaction för .NET API-referens
description: Det här anropet utlöses precis innan någon redigering tillämpas på dokumentet och gör det möjligt att logga eller förbjuda det.
type: docs
weight: 10
url: /sv/net/groupdocs.redaction.redactions/iredactioncallback/acceptredaction/
---
## IRedactionCallback.AcceptRedaction method

Det här anropet utlöses precis innan någon redigering tillämpas på dokumentet och gör det möjligt att logga eller förbjuda det.

```csharp
public bool AcceptRedaction(RedactionDescription description)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| description | RedactionDescription | Innehåller information om speciell matchningstyp, kriterier, text och position |

### Returvärde

Återgå sant för att acceptera eller falskt för att avböja en viss matchningsredigering

### Se även

* class [RedactionDescription](../../redactiondescription)
* interface [IRedactionCallback](../../iredactioncallback)
* namnutrymme [GroupDocs.Redaction.Redactions](../../iredactioncallback)
* hopsättning [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
