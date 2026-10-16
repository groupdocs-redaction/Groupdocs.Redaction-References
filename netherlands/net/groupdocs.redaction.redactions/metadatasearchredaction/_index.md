---
title: "MetadataSearchRedaction"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Stelt een metadata-redactie voor die metadata zoekt en redigeert met behulp van reguliere expressies die overeenkomen met sleutels en/of waarden."
type: docs
weight: 660
url: /nl/net/groupdocs.redaction.redactions/metadatasearchredaction/
---
## MetadataSearchRedaction class

Stelt een metadata‑redactie voor die metadata zoekt en redigeert met behulp van reguliere expressies, waarbij sleutels en/of waarden overeenkomen.

```csharp
public class MetadataSearchRedaction : MetadataRedaction
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [MetadataSearchRedaction](metadatasearchredaction#constructor_2)(Regex, string) | Initialiseert een nieuw exemplaar van de MetadataSearchRedaction-klasse, waarbij een waarde wordt gebruikt om te matchen met te redigeren items. |
| [MetadataSearchRedaction](metadatasearchredaction#constructor)(string, string) | Initialiseert een nieuw exemplaar van de MetadataSearchRedaction-klasse, waarbij een waarde wordt gebruikt om te matchen met te redigeren items. |
| [MetadataSearchRedaction](metadatasearchredaction#constructor_3)(Regex, string, Regex) | Initialiseert een nieuw exemplaar van de MetadataSearchRedaction-klasse, waarbij itemnaam en -waarde worden gebruikt om te matchen met te redigeren items. |
| [MetadataSearchRedaction](metadatasearchredaction#constructor_1)(string, string, string) | Initialiseert een nieuw exemplaar van de MetadataSearchRedaction-klasse, waarbij itemnaam en -waarde worden gebruikt om te matchen met te redigeren items. |

## Properties

| Naam | Beschrijving |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/metadatasearchredaction/description) { get; } | Retourneert een string die de redactie en de parameters beschrijft. |
| [Filter](../../groupdocs.redaction.redactions/metadataredaction/filter) { get; set; } | Haalt de filter op of stelt deze in, die wordt gebruikt om alle of specifieke metadata te selecteren, bijvoorbeeld Auteur of Bedrijf. |
| [KeyExpression](../../groupdocs.redaction.redactions/metadatasearchredaction/keyexpression) { get; } | Haalt de reguliere expressie op om de naam (sleutel) van een metadata-item te matchen. |
| [Replacement](../../groupdocs.redaction.redactions/metadatasearchredaction/replacement) { get; } | Haalt de tekstuele vervangingswaarde op. |
| [ValueExpression](../../groupdocs.redaction.redactions/metadatasearchredaction/valueexpression) { get; } | Haalt de reguliere expressie op om de waardetekst van een metadata-item te matchen. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/metadataredaction/applyto)(DocumentFormatInstance) | Past de redactie toe op een gegeven format‑instantie. |

### Opmerkingen

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document metadata redactions: [Metadata redactions](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Voorbeelden

Het volgende voorbeeld toont hoe bepaalde tekst in specifieke metadata te zoeken en te redigeren.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.docx"))
{
   MetadataSearchRedaction redaction = new MetadataSearchRedaction("Company Ltd.", "--company--");
   // Indien niet ingesteld, wordt toegepast op alle metadata‑items
   redaction.Filter = MetadataFilters.Company;
   redactor.Apply(redaction);
   redactor.Save();
}
```

### Zie ook

* class [MetadataRedaction](../metadataredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
