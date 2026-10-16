---
title: "RegexRedaction"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Stelt een tekstredactie voor die tekst in het document zoekt en vervangt door overeenstemming met de opgegeven reguliere expressie."
type: docs
weight: 750
url: /nl/net/groupdocs.redaction.redactions/regexredaction/
---
## RegexRedaction class

Stelt een tekstredactie voor die tekst in het document zoekt en vervangt door overeenstemming met de opgegeven reguliere expressie.

```csharp
public class RegexRedaction : TextRedaction
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [RegexRedaction](regexredaction#constructor_1)(Regex, ReplacementOptions) | Initialiseert een nieuw exemplaar van de RegexRedaction‑klasse. |
| [RegexRedaction](regexredaction#constructor)(string, ReplacementOptions) | Initialiseert een nieuw exemplaar van de RegexRedaction‑klasse. |

## Properties

| Naam | Beschrijving |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Haalt de [`ReplacementOptions`](../replacementoptions) instantie op, die het type tekstvervanging specificeert. |
| override [Description](../../groupdocs.redaction.redactions/regexredaction/description) { get; } | Retourneert een string die de redactie en de parameters beschrijft. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Haalt op of stelt de [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector) implementatie in, die nodig is om tekst uit grafische inhoud te extraheren. |
| [RegularExpression](../../groupdocs.redaction.redactions/regexredaction/regularexpression) { get; } | Haalt de reguliere expressie op die moet overeenkomen. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/regexredaction/applyto)(DocumentFormatInstance) | Past de redactie toe op een gegeven format‑instantie. |

### Opmerkingen

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

### Voorbeelden

Het volgende voorbeeld toont het vervangen van tekst met behulp van de reguliere expressie.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
      // vervang door tekst
      redactor.Apply(new RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", new ReplacementOptions("[removed]")));
      // vervang door een blauw, solide rechthoek
      redactor.Apply(new RegexRedaction(@"^\d+[,\.]{1}\d+$", new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Blue)));
      redactor.Save();
    }
```

### Zie ook

* class [TextRedaction](../textredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
