---
title: RegexRedaction
second_title: GroupDocs.Redaction voor .NET API-referentie
description: Vertegenwoordigt een tekstredactie die tekst in het document zoekt en vervangt door overeenkomende reguliere expressies.
type: docs
weight: 590
url: /nl/net/groupdocs.redaction.redactions/regexredaction/
---
## RegexRedaction class

Vertegenwoordigt een tekstredactie die tekst in het document zoekt en vervangt door overeenkomende reguliere expressies.

```csharp
public class RegexRedaction : TextRedaction
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [RegexRedaction](regexredaction#constructor_1)(Regex, ReplacementOptions) | Initialiseert een nieuw exemplaar van de klasse RegexRedaction. |
| [RegexRedaction](regexredaction#constructor)(string, ReplacementOptions) | Initialiseert een nieuw exemplaar van de klasse RegexRedaction. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Krijgt de[`ReplacementOptions`](../replacementoptions) instantie, specificeert het type tekstvervanging. |
| override [Description](../../groupdocs.redaction.redactions/regexredaction/description) { get; } | Retourneert een tekenreeks die de redactie en de bijbehorende parameters beschrijft. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Haalt of stelt de[`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector) implementatie, vereist om tekst uit grafische inhoud te extraheren. |
| [RegularExpression](../../groupdocs.redaction.redactions/regexredaction/regularexpression) { get; } | Haalt de overeenkomende reguliere expressie op. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/regexredaction/applyto)(DocumentFormatInstance) | Past de redactie toe op een bepaalde indelingsinstantie. |

### Opmerkingen

**Kom meer te weten**

* Meer informatie over het toepassen van redacties: [Basisprincipes van redactie](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Meer details over redactie van documenttekst: [Tekstredacties](https://docs.groupdocs.com/redaction/net/text-redactions/)

### Voorbeelden

Het volgende voorbeeld demonstreert het vervangen van tekst met behulp van de reguliere expressie.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
      // vervangen door tekst
      redactor.Apply(new RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", new ReplacementOptions("[removed]")));
      // vervang door blauwe vaste rechthoek
      redactor.Apply(new RegexRedaction(@"^\d+[,\.]{1}\d+$", new ReplacementOptions(System.Drawing.Color.Blue)));
      redactor.Save();
    }
```

### Zie ook

* class [TextRedaction](../textredaction)
* naamruimte [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* montage [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->