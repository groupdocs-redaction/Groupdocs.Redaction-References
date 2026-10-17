---
title: "Redigera"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Tillämpar anpassad maskering på specifikt dokumentinnehåll. För närvarande stöds detta endast för PDF PageAreaRedactiongroupdocs.redaction.redactions/pagearearedaction. Användare kan definiera sin egen maskeringslogik, såsom AIbased maskering, som kan vara mer avancerad än enkla patternbased metoder."
type: docs
weight: 10
url: /sv/net/groupdocs.redaction.redactions/icustomredactionhandler/redact/
---
## ICustomRedactionHandler.Redact method

Tillämpar anpassad maskering på specifikt dokumentinnehåll. För närvarande stöds detta endast för PDF [`PageAreaRedaction`](../../pagearearedaction). Användare kan definiera sin egen maskeringslogik, såsom AI-based maskering, som kan vara mer avancerad än enkla pattern-based metoder.

```csharp
public CustomRedactionResult Redact(CustomRedactionContext context)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kontext | CustomRedactionContext | Innehåller dokumentinnehållet som ska maskeras samt relaterad metadata. |

### Returvärde

Ett [`CustomRedactionResult`](../../customredactionresult) som indikerar om maskeringen ska tillämpas och det modifierade innehållet.

### Se även

* class [CustomRedactionResult](../../customredactionresult)
* class [CustomRedactionContext](../../customredactioncontext)
* interface [ICustomRedactionHandler](../../icustomredactionhandler)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
