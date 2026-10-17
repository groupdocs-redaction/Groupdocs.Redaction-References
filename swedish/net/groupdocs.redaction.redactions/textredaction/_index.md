---
title: "TextRedaction"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar en bas‑abstrakt klass för dokumenttext‑redigeringar."
type: docs
weight: 800
url: /sv/net/groupdocs.redaction.redactions/textredaction/
---
## TextRedaction class

Representerar en bas‑abstrakt klass för dokumenttext‑redigeringar.

```csharp
public abstract class TextRedaction : Redaction
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Hämtar [`ReplacementOptions`](../replacementoptions)-instansen, som specificerar typen av textersättning. |
| virtual [Description](../../groupdocs.redaction/redaction/description) { get; } | Returnerar en sträng som beskriver redaction och dess parametrar. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Hämtar eller anger [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector)-implementeringen som krävs för att extrahera text från grafiskt innehåll. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| abstract [ApplyTo](../../groupdocs.redaction/redaction/applyto)(DocumentFormatInstance) | Tillämpar redaction på en given formatinstans. |

### Anmärkningar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

### Se även

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
