---
title: "PageAreaRedaction"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar en komplex textredigering som påverkar textbilder och annotationer i ett område på sidan."
type: docs
weight: 680
url: /sv/net/groupdocs.redaction.redactions/pagearearedaction/
---
## PageAreaRedaction class

Representerar en komplex textuell redigering som påverkar text, bilder och kommentarer i ett område på sidan.

```csharp
public class PageAreaRedaction : RegexRedaction
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [PageAreaRedaction](pagearearedaction#constructor)(Regex, ReplacementOptions) | Initierar en ny instans av klassen PageAreaRedaction. |
| [PageAreaRedaction](pagearearedaction#constructor_1)(Regex, ReplacementOptions, RegionReplacementOptions) | Initierar en ny instans av klassen PageAreaRedaction. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Hämtar [`ReplacementOptions`](../replacementoptions)-instansen, som specificerar typen av textersättning. |
| override [Description](../../groupdocs.redaction.redactions/regexredaction/description) { get; } | Returnerar en sträng som beskriver redaction och dess parametrar. |
| [ImageOptions](../../groupdocs.redaction.redactions/pagearearedaction/imageoptions) { get; } | Hämtar [`RegionReplacementOptions`](../regionreplacementoptions)-alternativen med färg- och områdesparametrar. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Hämtar eller anger [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector)-implementeringen som krävs för att extrahera text från grafiskt innehåll. |
| [RegularExpression](../../groupdocs.redaction.redactions/regexredaction/regularexpression) { get; } | Hämtar det reguljära uttrycket att matcha. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/pagearearedaction/applyto)(DocumentFormatInstance) | Tillämpar redaction på en given formatinstans. |

### Anmärkningar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/net/use-page-area-redaction/)

### Se även

* class [RegexRedaction](../regexredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
