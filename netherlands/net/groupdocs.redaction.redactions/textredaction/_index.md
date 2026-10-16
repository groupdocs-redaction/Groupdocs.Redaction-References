---
title: "TextRedaction"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Stelt een basis abstracte klasse voor documenttekst‑redacties voor."
type: docs
weight: 800
url: /nl/net/groupdocs.redaction.redactions/textredaction/
---
## TextRedaction class

Stelt een basis abstracte klasse voor documenttekst‑redacties voor.

```csharp
public abstract class TextRedaction : Redaction
```

## Properties

| Naam | Beschrijving |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Haalt de [`ReplacementOptions`](../replacementoptions) instantie op, die het type tekstvervanging specificeert. |
| virtual [Description](../../groupdocs.redaction/redaction/description) { get; } | Retourneert een string die de redactie en de parameters beschrijft. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Haalt op of stelt de [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector) implementatie in, die nodig is om tekst uit grafische inhoud te extraheren. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| abstract [ApplyTo](../../groupdocs.redaction/redaction/applyto)(DocumentFormatInstance) | Past de redactie toe op een gegeven format‑instantie. |

### Opmerkingen

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

### Zie ook

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
