---
title: "RegexRedaction"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar en textredigering som söker och ersätter text i dokumentet genom att matcha det angivna reguljära uttrycket."
type: docs
weight: 750
url: /sv/net/groupdocs.redaction.redactions/regexredaction/
---
## RegexRedaction class

Representerar en textredigering som söker och ersätter text i dokumentet genom att matcha det angivna reguljära uttrycket.

```csharp
public class RegexRedaction : TextRedaction
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [RegexRedaction](regexredaction#constructor_1)(Regex, ReplacementOptions) | Initierar en ny instans av klassen RegexRedaction. |
| [RegexRedaction](regexredaction#constructor)(string, ReplacementOptions) | Initierar en ny instans av klassen RegexRedaction. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Hämtar [`ReplacementOptions`](../replacementoptions)-instansen, som specificerar typen av textersättning. |
| override [Description](../../groupdocs.redaction.redactions/regexredaction/description) { get; } | Returnerar en sträng som beskriver redaction och dess parametrar. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Hämtar eller anger [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector)-implementeringen som krävs för att extrahera text från grafiskt innehåll. |
| [RegularExpression](../../groupdocs.redaction.redactions/regexredaction/regularexpression) { get; } | Hämtar det reguljära uttrycket att matcha. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/regexredaction/applyto)(DocumentFormatInstance) | Tillämpar redaction på en given formatinstans. |

### Anmärkningar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

### Exempel

Följande exempel visar hur man ersätter text med hjälp av det reguljära uttrycket.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
      // ersätt med text
      redactor.Apply(new RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", new ReplacementOptions("[removed]")));
      // ersätt med blå solid rektangel
      redactor.Apply(new RegexRedaction(@"^\d+[,\.]{1}\d+$", new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Blue)));
      redactor.Save();
    }
```

### Se även

* class [TextRedaction](../textredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
