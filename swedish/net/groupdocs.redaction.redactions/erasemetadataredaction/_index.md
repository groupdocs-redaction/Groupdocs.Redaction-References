---
title: "EraseMetadataRedaction"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar en metadata‑redigering som raderar all metadata eller metadata som matchar specifika MetadataFilters från dokumentet."
type: docs
weight: 590
url: /sv/net/groupdocs.redaction.redactions/erasemetadataredaction/
---
## EraseMetadataRedaction class

Representerar en metadata‑redigering som raderar all metadata eller metadata som matchar specifika MetadataFilters från dokumentet.

```csharp
public class EraseMetadataRedaction : MetadataRedaction
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [EraseMetadataRedaction](erasemetadataredaction#constructor)() | Initierar en ny instans av klassen EraseMetadataRedaction och raderar all metadata. |
| [EraseMetadataRedaction](erasemetadataredaction#constructor_1)(MetadataFilters) | Initierar en ny instans av klassen EraseMetadataRedaction, raderar metadata och matchar en specifik kombination av [`MetadataFilters`](../metadatafilters). |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/erasemetadataredaction/description) { get; } | Returnerar en sträng som beskriver redaction och dess parametrar. |
| [Filter](../../groupdocs.redaction.redactions/metadataredaction/filter) { get; set; } | Hämtar eller anger filtret som används för att välja all eller specifik metadata, till exempel Author eller Company. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/metadataredaction/applyto)(DocumentFormatInstance) | Tillämpar redaction på en given formatinstans. |

### Anmärkningar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document metadata redactions: [Metadata redactions](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Exempel

Följande exempel visar hur man raderar (sätter till tomma värden) all eller specifik metadata.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.docx"))
{
   // Radera Author, Manager och Company
   redactor.Apply(new EraseMetadataRedaction(MetadataFilters.Author | MetadataFilters.Manager | MetadataFilters.Company));
   // Radera all metadata
   redactor.Apply(new EraseMetadataRedaction(MetadataFilters.All));
   redactor.Save();
}
```

### Se även

* class [MetadataRedaction](../metadataredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
