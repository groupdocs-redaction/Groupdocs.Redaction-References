---
title: "ReplacementOptions"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar alternativ för ersättning av matchande text."
type: docs
weight: 780
url: /sv/net/groupdocs.redaction.redactions/replacementoptions/
---
## ReplacementOptions class

Representerar alternativ för ersättning av matchande text.

```csharp
public class ReplacementOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [ReplacementOptions](replacementoptions#constructor)(Color) | Initierar en ny instans av klassen ReplacementOptions med färgad rektangel som alternativ. |
| [ReplacementOptions](replacementoptions#constructor_1)(string) | Initierar en ny instans av klassen ReplacementOptions med ersättningstext som alternativ. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ActionType](../../groupdocs.redaction.redactions/replacementoptions/actiontype) { get; } | Hämtar ersättningsåtgärden: rita ruta eller ersätta text. |
| [BoxColor](../../groupdocs.redaction.redactions/replacementoptions/boxcolor) { get; set; } | Hämtar eller anger färgen för ett DrawBox-alternativ (ignoreras annars). |
| [CustomRedaction](../../groupdocs.redaction.redactions/replacementoptions/customredaction) { get; set; } | Hämtar eller anger en anpassad raderings [`ICustomRedactionHandler`](../icustomredactionhandler) hanterare som tillåter användare att definiera sin egen raderingslogik. |
| [Filters](../../groupdocs.redaction.redactions/replacementoptions/filters) { get; set; } | Hämtar eller anger en array av filter som ska tillämpas med denna radering. |
| [Replacement](../../groupdocs.redaction.redactions/replacementoptions/replacement) { get; set; } | Hämtar eller anger det textuella ersättningsvärdet. |

### Anmärkningar

**Learn more**

* More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)
* More details about redaction filters: [Use PDF redaction filters](https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/)

### Se även

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
