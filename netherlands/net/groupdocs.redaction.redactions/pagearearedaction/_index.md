---
title: "PageAreaRedaction"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Stelt een complexe tekstuele redactie voor die tekst, afbeeldingen en annotaties in een gebied van de pagina beïnvloedt."
type: docs
weight: 680
url: /nl/net/groupdocs.redaction.redactions/pagearearedaction/
---
## PageAreaRedaction class

Stelt een complexe tekstuele redactie voor die tekst, afbeeldingen en annotaties in een gebied van de pagina beïnvloedt.

```csharp
public class PageAreaRedaction : RegexRedaction
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [PageAreaRedaction](pagearearedaction#constructor)(Regex, ReplacementOptions) | Initialiseert een nieuw exemplaar van de PageAreaRedaction-klasse. |
| [PageAreaRedaction](pagearearedaction#constructor_1)(Regex, ReplacementOptions, RegionReplacementOptions) | Initialiseert een nieuw exemplaar van de PageAreaRedaction-klasse. |

## Properties

| Naam | Beschrijving |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Haalt de [`ReplacementOptions`](../replacementoptions) instantie op, die het type tekstvervanging specificeert. |
| override [Description](../../groupdocs.redaction.redactions/regexredaction/description) { get; } | Retourneert een string die de redactie en de parameters beschrijft. |
| [ImageOptions](../../groupdocs.redaction.redactions/pagearearedaction/imageoptions) { get; } | Haalt de [`RegionReplacementOptions`](../regionreplacementoptions) opties op met kleur- en gebiedsparameters. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Haalt op of stelt de [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector) implementatie in, die nodig is om tekst uit grafische inhoud te extraheren. |
| [RegularExpression](../../groupdocs.redaction.redactions/regexredaction/regularexpression) { get; } | Haalt de reguliere expressie op die moet overeenkomen. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/pagearearedaction/applyto)(DocumentFormatInstance) | Past de redactie toe op een gegeven format‑instantie. |

### Opmerkingen

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/net/use-page-area-redaction/)

### Zie ook

* class [RegexRedaction](../regexredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
