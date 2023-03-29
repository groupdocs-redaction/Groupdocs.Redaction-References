---
title: TextRedaction
second_title: GroupDocs.Redaction voor .NET API-referentie
description: Vertegenwoordigt een abstracte basisklasse voor redactie van documenttekst.
type: docs
weight: 640
url: /nl/net/groupdocs.redaction.redactions/textredaction/
---
## TextRedaction class

Vertegenwoordigt een abstracte basisklasse voor redactie van documenttekst.

```csharp
public abstract class TextRedaction : Redaction
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Krijgt de[`ReplacementOptions`](../replacementoptions) instantie, specificeert het type tekstvervanging. |
| virtual [Description](../../groupdocs.redaction/redaction/description) { get; } | Retourneert een tekenreeks die de redactie en de bijbehorende parameters beschrijft. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Haalt of stelt de[`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector) implementatie, vereist om tekst uit grafische inhoud te extraheren. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| abstract [ApplyTo](../../groupdocs.redaction/redaction/applyto)(DocumentFormatInstance) | Past de redactie toe op een bepaalde indelingsinstantie. |

### Opmerkingen

**Kom meer te weten**

* Meer informatie over het toepassen van redacties: [Basisprincipes van redactie](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Meer details over redactie van documenttekst: [Tekstredacties](https://docs.groupdocs.com/redaction/net/text-redactions/)

### Zie ook

* class [Redaction](../../groupdocs.redaction/redaction)
* naamruimte [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* montage [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->