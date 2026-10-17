---
title: "groupdocs.redaction.redactions"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Typer under groupdocs.redaction.redactions."
type: docs
url: /sv/python-net/groupdocs.redaction.redactions/
is_root: false
weight: 60
---


Typer under `groupdocs.redaction.redactions`.

### Klasser
| Klass | Beskrivning |
| :- | :- |
| [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) | Representerar en maskering som ersätter annoteringstext (kommentarer osv) som matchar ett givet reguljärt uttryck. |
| [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/) | Representerar en textmaskering som ersätter text i ett kalkylbladsdokument (CSV, Excel osv). |
| [`CellFilter`](/redaction/python-net/groupdocs.redaction.redactions/cellfilter/) | Tillhandahåller ett alternativ för att begränsa omfattningen av en [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/) till ett arbetsblad och en kolumn. |
| [`CustomRedactionContext`](/redaction/python-net/groupdocs.redaction.redactions/customredactioncontext/) | Tillhandahåller kontext för anpassad maskeringsbearbetning. |
| [`CustomRedactionResult`](/redaction/python-net/groupdocs.redaction.redactions/customredactionresult/) | Representerar resultatet av en anpassad maskeringsoperation. |
| [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/) | Representerar en textmaskering som tar bort annoteringar om texten matchar ett givet reguljärt uttryck (valfritt tar bort alla annoteringar). |
| [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/) | Representerar en metadata-maskering som raderar all metadata eller metadata som matchar specifika MetadataFilters från dokumentet. |
| [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/) | Representerar en textmaskering som ersätter en exakt fras i dokumentets text, skiftlägesokänslig som standard. |
| [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/) | Tillhandahåller ett gränssnitt för att implementera anpassad maskeringslogik. |
| [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) | Definierar metoder som krävs för att ta emot information om varje raderingsändring och eventuellt förhindra den. |
| [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) | Representerar en radering som placerar en färgad rektangel i ett givet område av ett bilddokument. |
| [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) | Representerar en grundläggande abstrakt klass för dokumentmetadata‑raderingar. |
| [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) | Representerar en metadata‑radering som söker och raderar metadata med hjälp av reguljära uttryck, matchar nycklar och/eller värden. |
| [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/) | Representerar ett raderingsfilter som anger ett område inom en sida i ett dokument för att tillämpa radering. |
| [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/) | Representerar en komplex textuell radering som påverkar text, bilder och annotationer i ett område på sidan. |
| [`PageRangeFilter`](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/) | Representerar ett raderingsfilter som anger sidintervall i ett dokument för att tillämpa radering. |
| [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/) | Representerar information om en enskild ändringsåtgärd som utfördes under raderingsprocessen. |
| [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Representerar en textradering som söker och ersätter text i dokumentet genom att matcha angivet reguljärt uttryck. |
| [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/) | Representerar färg- och områdesparametrar för ersättning av bildregion. |
| [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/) | Representerar en radering som tar bort en sida (bildspel, kalkylblad osv.) från ett dokument. |
| [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) | Representerar alternativ för ersättning av matchad text. |
| [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) | Representerar en grundläggande abstrakt klass för dokumenttextraderingar. |
| [`TextReplacement`](/redaction/python-net/groupdocs.redaction.redactions/textreplacement/) | Representerar information om textuell ersättning. |

### Enumerationer
| Enum | Beskrivning |
| :- | :- |
| [`MetadataFilters`](/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) |  |
| [`PageSeekOrigin`](/redaction/python-net/groupdocs.redaction.redactions/pageseekorigin/) |  |
| [`RedactionActionType`](/redaction/python-net/groupdocs.redaction.redactions/redactionactiontype/) |  |
| [`RedactionFilter`](/redaction/python-net/groupdocs.redaction.redactions/redactionfilter/) | Representerar ett raderingsfilter som anger omfattning i ett dokument för att tillämpa raderingar. |
| [`RedactionType`](/redaction/python-net/groupdocs.redaction.redactions/redactiontype/) |  |
| [`ReplacementType`](/redaction/python-net/groupdocs.redaction.redactions/replacementtype/) |  |
