---
title: "MetadataFilters"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar en lista över de vanligaste typerna av dokumentmetadata."
type: docs
weight: 640
url: /sv/net/groupdocs.redaction.redactions/metadatafilters/
---
## MetadataFilters enumeration

Representerar en lista över de vanligaste typerna av dokumentmetadata.

```csharp
[Flags]
public enum MetadataFilters
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Tom filterinställning, matchar inga metadataobjekt. |
| Author | `1` | Författare till dokumentet. |
| Category | `2` | Kategori för dokumentet. |
| Comments | `4` | Kommentar för dokumentet. |
| Company | `8` | Företag för författaren. |
| ContentStatus | `10` | Innehållsstatus. |
| CreatedTime | `20` | Skapad tid. |
| HyperlinkBase | `40` | Hyperlänkbas. |
| LastPrinted | `80` | Senast utskrivna datum och tid. |
| LastSavedBy | `100` | Senast sparad av användare. |
| LastSavedTime | `400` | Senast sparade datum och tid. |
| NameOfApplication | `800` | Namnet på programmet där dokumentet skapades. |
| Manager | `1000` | Författarens chefs namn. |
| RevisionNumber | `2000` | Revisionsnummer. |
| Subject | `4000` | Dokumentets ämne. |
| Template | `8000` | Dokumentmallens namn. |
| Title | `10000` | Dokumenttitel. |
| TotalEditingTime | `20000` | Total redigeringstid. |
| Version | `40000` | Dokumentets version. |
| Description | `80000` | Dokumentets beskrivning. |
| Keywords | `100000` | Dokumentets nyckelord. |
| ContentType | `200000` | Innehållstyp. |
| All | `7FFFFFFF` | Alla typer av metadataobjekt. |

### Anmärkningar

**Learn more**

* More details about document metadata redactions: [Metadata redactions](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Se även

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
