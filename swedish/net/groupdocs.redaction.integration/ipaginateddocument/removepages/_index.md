---
title: "RemovePages"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Tar bort en eller flera sidor beroende på dess startpositionsförskjutning och antal."
type: docs
weight: 10
url: /sv/net/groupdocs.redaction.integration/ipaginateddocument/removepages/
---
## IPaginatedDocument.RemovePages method

Tar bort en eller flera sidor beroende på dess startposition, offset och antal.

```csharp
public RedactionResult RemovePages(PageSeekOrigin origin, int index, int count)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ursprung | PageSeekOrigin | Sök ursprungsposition, början eller slutet av dokumentet |
| index | Int32 | Startpositionsindex (0-baserat) |
| antal | Int32 | Antal sidor att ta bort |

### Returvärde

Resultat av sidborttagning

### Se även

* class [RedactionResult](../../../groupdocs.redaction/redactionresult)
* enum [PageSeekOrigin](../../../groupdocs.redaction.redactions/pageseekorigin)
* interface [IPaginatedDocument](../../ipaginateddocument)
* namespace [GroupDocs.Redaction.Integration](../../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
