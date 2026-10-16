---
title: "com.groupdocs.redaction.redactions"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Paketet tillhandahåller klasser för olika typer av rensningar."
type: docs
weight: 16
url: /sv/java/com.groupdocs.redaction.redactions/
---

Paketet tillhandahåller klasser för olika typer av rensningar.



## Klasser

| Klass | Beskrivning |
| --- | --- |
| [AnnotationRedaction](../com.groupdocs.redaction.redactions/annotationredaction) | Representerar en radering som ersätter annoteringstext (kommentarer osv.) som matchar ett givet reguljärt uttryck. |
| [CellColumnRedaction](../com.groupdocs.redaction.redactions/cellcolumnredaction) | Representerar en textradering som ersätter text i kalkylbladsdokument (CSV, Excel osv.). |
| [CellFilter](../com.groupdocs.redaction.redactions/cellfilter) | Tillhandahåller ett alternativ för att begränsa omfattningen av en CellColumnRedaction till ett arbetsblad och en kolumn. |
| [CustomRedactionContext](../com.groupdocs.redaction.redactions/customredactioncontext) | Tillhandahåller indata för [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler). |
| [CustomRedactionResult](../com.groupdocs.redaction.redactions/customredactionresult) | Representerar ett resultat som returneras av [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler). |
| [DeleteAnnotationRedaction](../com.groupdocs.redaction.redactions/deleteannotationredaction) | Representerar en textradering som tar bort annoteringar om texten matchar ett givet reguljärt uttryck (valfritt tar bort alla annoteringar). |
| [EraseMetadataRedaction](../com.groupdocs.redaction.redactions/erasemetadataredaction) | Representerar en metadata-radering som raderar all metadata eller metadata som matchar specifika MetadataFilters från dokumentet. |
| [ExactPhraseRedaction](../com.groupdocs.redaction.redactions/exactphraseredaction) | Representerar en textradering som ersätter exakt fras i dokumentets text, skiftlägesokänslig som standard. |
| [ImageAreaRedaction](../com.groupdocs.redaction.redactions/imagearearedaction) | Representerar en radering som placerar en färgad rektangel i ett givet område av ett bilddokument. |
| [MetadataFilters](../com.groupdocs.redaction.redactions/metadatafilters) | Representerar en lista över de vanligaste typerna av dokumentmetadata. |
| [MetadataRedaction](../com.groupdocs.redaction.redactions/metadataredaction) | Representerar en basabstrakt klass för dokumentmetadata‑redigeringar. |
| [MetadataSearchRedaction](../com.groupdocs.redaction.redactions/metadatasearchredaction) | Representerar en metadata‑redigering som söker och raderar metadata med hjälp av reguljära uttryck, matchande nycklar och/eller värden. |
| [PageAreaFilter](../com.groupdocs.redaction.redactions/pageareafilter) | Representerar ett redigeringsfilter som anger ett område inom en sida i ett dokument för att tillämpa redigering. |
| [PageAreaRedaction](../com.groupdocs.redaction.redactions/pagearearedaction) | Representerar en komplex textuell redigering som påverkar text, bilder och kommentarer i ett område på sidan. |
| [PageRangeFilter](../com.groupdocs.redaction.redactions/pagerangefilter) | Representerar ett redigeringsfilter som anger sidintervall i ett dokument för att tillämpa redigering. |
| [RedactionDescription](../com.groupdocs.redaction.redactions/redactiondescription) | Representerar information om en enskild förändringsåtgärd som utförs under redigeringsprocessen. |
| [RedactionFilter](../com.groupdocs.redaction.redactions/redactionfilter) | Representerar ett redigeringsfilter som anger omfattning i ett dokument för att tillämpa redigeringar. |
| [RedactionType](../com.groupdocs.redaction.redactions/redactiontype) | Representerar en typ av dokumentdata som påverkas av redigering. |
| [RegexRedaction](../com.groupdocs.redaction.redactions/regexredaction) | Representerar en textredigering som söker och ersätter text i dokumentet genom att matcha det angivna reguljära uttrycket. |
| [RegionReplacementOptions](../com.groupdocs.redaction.redactions/regionreplacementoptions) | Representerar färg- och områdesparametrar för ersättning av bildregion. |
| [RemovePageRedaction](../com.groupdocs.redaction.redactions/removepageredaction) | Representerar en redigering som tar bort en sida (bildspel, kalkylblad osv.) från ett dokument. |
| [ReplacementOptions](../com.groupdocs.redaction.redactions/replacementoptions) | Representerar alternativ för ersättning av matchad text. |
| [TextRedaction](../com.groupdocs.redaction.redactions/textredaction) | Representerar en basabstrakt klass för dokumenttextredigeringar. |
| [TextReplacement](../com.groupdocs.redaction.redactions/textreplacement) | Representerar information om en textuell ersättning. |

## Gränssnitt

| Gränssnitt | Beskrivning |
| --- | --- |
| [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler) | Definierar en anpassad redigeringsåteruppringning. |
| [IRedactionCallback](../com.groupdocs.redaction.redactions/iredactioncallback) | Definierar metoder som krävs för att ta emot information om varje redigeringsändring och eventuellt förhindra den. |

## Enumerationer

| Enum | Beskrivning |
| --- | --- |
| [PageSeekOrigin](../com.groupdocs.redaction.redactions/pageseekorigin) | Tillhandahåller fälten som representerar referenspunkter i ett dokument för sökning. |
| [RedactionActionType](../com.groupdocs.redaction.redactions/redactionactiontype) | Representerar åtgärder som kan vidtas för att utföra redigering. |
| [ReplacementType](../com.groupdocs.redaction.redactions/replacementtype) | Representerar en typ av ersättning för den matchade texten. |
