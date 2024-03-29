---
title: RemovePageRedaction
second_title: GroupDocs.Redaction för .NET API-referens
description: Representerar en redigering som tar bort en sida bild kalkylblad etc. från ett dokument.
type: docs
weight: 610
url: /sv/net/groupdocs.redaction.redactions/removepageredaction/
---
## RemovePageRedaction class

Representerar en redigering som tar bort en sida (bild, kalkylblad, etc.) från ett dokument.

```csharp
public class RemovePageRedaction : Redaction
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [RemovePageRedaction](removepageredaction)(PageSeekOrigin, int, int) | Initierar en ny instans av klassen RemovePageRedaction. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Count](../../groupdocs.redaction.redactions/removepageredaction/count) { get; } | Hämtar antalet sidor att ta bort. |
| virtual [Description](../../groupdocs.redaction/redaction/description) { get; } | Returnerar en sträng som beskriver redaktionen och dess parametrar. |
| [Index](../../groupdocs.redaction.redactions/removepageredaction/index) { get; } | Hämtar startpositionsindex (0-baserat). |
| [Origin](../../groupdocs.redaction.redactions/removepageredaction/origin) { get; } | Får sökreferensposition, början eller slutet av ett dokument. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/removepageredaction/applyto)(DocumentFormatInstance) | Tillämpar redigeringen på en given formatinstans. |

### Anmärkningar

**Läs mer**

* Mer information om att tillämpa redigeringar: [Grundläggande om redigering](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Mer information om att ta bort sidor: [Ta bort sidredigering](https://docs.groupdocs.com/redaction/net/remove-page-redaction/)

### Exempel

Följande exempel visar hur man tar bort den sista sidan i dokumentet.

```csharp
using (Redactor redactor = new Redactor(@"C:\test.pdf"))
{
   redactor.Apply(new RemovePageRedaction(PageSeekOrigin.End, 0, 1));
   redactor.Save()
}
```

### Se även

* class [Redaction](../../groupdocs.redaction/redaction)
* namnutrymme [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* hopsättning [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
