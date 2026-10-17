---
title: "RemovePageRedaction"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar en redigering som tar bort en sida, bildspel, kalkylblad etc. från ett dokument."
type: docs
weight: 770
url: /sv/net/groupdocs.redaction.redactions/removepageredaction/
---
## RemovePageRedaction class

Representerar en redigering som tar bort en sida (bildspel, kalkylblad osv.) från ett dokument.

```csharp
public class RemovePageRedaction : Redaction
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [RemovePageRedaction](removepageredaction)(PageSeekOrigin, int, int) | Initierar en ny instans av klassen RemovePageRedaction. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Count](../../groupdocs.redaction.redactions/removepageredaction/count) { get; } | Hämtar antalet sidor som ska tas bort. |
| virtual [Description](../../groupdocs.redaction/redaction/description) { get; } | Returnerar en sträng som beskriver redaction och dess parametrar. |
| [Index](../../groupdocs.redaction.redactions/removepageredaction/index) { get; } | Hämtar startpositionsindex (0‑baserat). |
| [Origin](../../groupdocs.redaction.redactions/removepageredaction/origin) { get; } | Hämtar referensposition för sökning, början eller slutet av ett dokument. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/removepageredaction/applyto)(DocumentFormatInstance) | Tillämpar redaction på en given formatinstans. |

### Anmärkningar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about removing pages: [Remove page redaction](https://docs.groupdocs.com/redaction/net/remove-page-redaction/)

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
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
