---
title: MetadataSearchRedaction
second_title: GroupDocs.Redaction voor .NET API-referentie
description: Vertegenwoordigt een redactie van metagegevens die metagegevens doorzoekt en redigeert met behulp van reguliere expressies overeenkomende sleutels en/of waarden.
type: docs
weight: 540
url: /nl/net/groupdocs.redaction.redactions/metadatasearchredaction/
---
## MetadataSearchRedaction class

Vertegenwoordigt een redactie van metagegevens die metagegevens doorzoekt en redigeert met behulp van reguliere expressies, overeenkomende sleutels en/of waarden.

```csharp
public class MetadataSearchRedaction : MetadataRedaction
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [MetadataSearchRedaction](metadatasearchredaction#constructor_2)(Regex, string) | Initialiseert een nieuwe instantie van de MetadataSearchRedaction-klasse, waarbij waarde wordt gebruikt om te matchen met geredigeerde items. |
| [MetadataSearchRedaction](metadatasearchredaction#constructor)(string, string) | Initialiseert een nieuwe instantie van de MetadataSearchRedaction-klasse, waarbij waarde wordt gebruikt om te matchen met geredigeerde items. |
| [MetadataSearchRedaction](metadatasearchredaction#constructor_3)(Regex, string, Regex) | Initialiseert een nieuwe instantie van de klasse MetadataSearchRedaction, waarbij de naam en waarde van het item worden gebruikt om overeen te komen met de geredigeerde items. |
| [MetadataSearchRedaction](metadatasearchredaction#constructor_1)(string, string, string) | Initialiseert een nieuwe instantie van de klasse MetadataSearchRedaction, waarbij de naam en waarde van het item worden gebruikt om overeen te komen met de geredigeerde items. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/metadatasearchredaction/description) { get; } | Retourneert een tekenreeks die de redactie en de bijbehorende parameters beschrijft. |
| [Filter](../../groupdocs.redaction.redactions/metadataredaction/filter) { get; set; } | Haalt of stelt het filter in, dat wordt gebruikt om alle of specifieke metadata te selecteren, bijvoorbeeld Auteur of Bedrijf. |
| [KeyExpression](../../groupdocs.redaction.redactions/metadatasearchredaction/keyexpression) { get; } | Haalt de reguliere expressie op die overeenkomt met de naam (sleutel) van het metadata-item. |
| [Replacement](../../groupdocs.redaction.redactions/metadatasearchredaction/replacement) { get; } | Krijgt de tekstuele vervangingswaarde. |
| [ValueExpression](../../groupdocs.redaction.redactions/metadatasearchredaction/valueexpression) { get; } | Haalt de reguliere expressie op die overeenkomt met de waardetekst van een metadata-item. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/metadataredaction/applyto)(DocumentFormatInstance) | Past de redactie toe op een bepaalde indelingsinstantie. |

### Opmerkingen

**Kom meer te weten**

* Meer informatie over het toepassen van redacties: [Basisprincipes van redactie](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Meer details over redactie van metadata van documenten: [Bewerkingen van metagegevens](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Voorbeelden

In het volgende voorbeeld ziet u hoe u bepaalde tekst in specifieke metadata kunt doorzoeken en redigeren.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.docx"))
{
   MetadataSearchRedaction redaction = new MetadataSearchRedaction("Company Ltd.", "--company--");
   // Indien niet ingesteld, geldt dit voor alle metadata-items
   redaction.Filter = MetadataFilters.Company;
   redactor.Apply(redaction);
   redactor.Save();
}
```

### Zie ook

* class [MetadataRedaction](../metadataredaction)
* naamruimte [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* montage [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->