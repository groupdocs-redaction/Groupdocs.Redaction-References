---
title: "EraseMetadataRedaction"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Stelt een metadata‑redactie voor die alle metadata of metadata die overeenkomen met specifieke MetadataFilters uit het document verwijdert."
type: docs
weight: 590
url: /nl/net/groupdocs.redaction.redactions/erasemetadataredaction/
---
## EraseMetadataRedaction class

Stelt een metadata‑redactie voor die alle metadata of metadata die overeenkomen met specifieke MetadataFilters uit het document verwijdert.

```csharp
public class EraseMetadataRedaction : MetadataRedaction
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [EraseMetadataRedaction](erasemetadataredaction#constructor)() | Initialiseert een nieuw exemplaar van de EraseMetadataRedaction-klasse, waarbij alle metadata worden gewist. |
| [EraseMetadataRedaction](erasemetadataredaction#constructor_1)(MetadataFilters) | Initialiseert een nieuw exemplaar van de EraseMetadataRedaction-klasse, waarbij metadata worden gewist, passend bij een specifieke combinatie van [`MetadataFilters`](../metadatafilters). |

## Properties

| Naam | Beschrijving |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/erasemetadataredaction/description) { get; } | Retourneert een string die de redactie en de parameters beschrijft. |
| [Filter](../../groupdocs.redaction.redactions/metadataredaction/filter) { get; set; } | Haalt de filter op of stelt deze in, die wordt gebruikt om alle of specifieke metadata te selecteren, bijvoorbeeld Auteur of Bedrijf. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/metadataredaction/applyto)(DocumentFormatInstance) | Past de redactie toe op een gegeven format‑instantie. |

### Opmerkingen

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document metadata redactions: [Metadata redactions](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Voorbeelden

Het volgende voorbeeld laat zien hoe alle of specifieke metadata te wissen (instellen op lege waarden).

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.docx"))
{
   // Wis Auteur, Manager en Bedrijf
   redactor.Apply(new EraseMetadataRedaction(MetadataFilters.Author | MetadataFilters.Manager | MetadataFilters.Company));
   // Wis alle metadata
   redactor.Apply(new EraseMetadataRedaction(MetadataFilters.All));
   redactor.Save();
}
```

### Zie ook

* class [MetadataRedaction](../metadataredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
