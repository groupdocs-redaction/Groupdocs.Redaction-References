---
title: "GroupDocs.Redaction.Redactions"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Redactions‑namnrymden tillhandahåller klasser för olika typer av maskeringar."
type: docs
weight: 80
url: /sv/net/groupdocs.redaction.redactions/
---
Redactions‑namnrymden tillhandahåller klasser för olika typer av maskeringar.

## Klasser

| Klass | Beskrivning |
| --- | --- |
| [AnnotationRedaction](./annotationredaction) | Representerar en radering som ersätter annoteringstext (kommentarer osv.) som matchar ett givet reguljärt uttryck. |
| [CellColumnRedaction](./cellcolumnredaction) | Representerar en textradering som ersätter text i kalkylbladsdokument (CSV, Excel osv.). |
| [CellFilter](./cellfilter) | Tillhandahåller ett alternativ för att begränsa omfattningen av en [`CellColumnRedaction`](../groupdocs.redaction.redactions/cellcolumnredaction) till ett arbetsblad och en kolumn. |
| [CustomRedactionContext](./customredactioncontext) | Tillhandahåller kontext för anpassad raderingsbehandling. |
| [CustomRedactionResult](./customredactionresult) | Representerar resultatet av en anpassad raderingsoperation. |
| [DeleteAnnotationRedaction](./deleteannotationredaction) | Representerar en textradering som tar bort annoteringar om texten matchar ett givet reguljärt uttryck (valfritt tar bort alla annoteringar). |
| [EraseMetadataRedaction](./erasemetadataredaction) | Representerar en metadata‑redigering som raderar all metadata eller metadata som matchar specifika MetadataFilters från dokumentet. |
| [ExactPhraseRedaction](./exactphraseredaction) | Representerar en textredigering som ersätter exakt fras i dokumentets text, skiftlägesokänslig som standard. |
| [ImageAreaRedaction](./imagearearedaction) | Representerar en redigering som placerar en färgad rektangel i ett givet område av ett bilddokument. |
| [MetadataRedaction](./metadataredaction) | Representerar en bas‑abstrakt klass för dokumentmetadata‑redigeringar. |
| [MetadataSearchRedaction](./metadatasearchredaction) | Representerar en metadata‑redigering som söker och raderar metadata med reguljära uttryck, och matchar nycklar och/eller värden. |
| [PageAreaFilter](./pageareafilter) | Representerar ett redigeringsfilter som anger ett område inom en sida i ett dokument för att tillämpa redigering. |
| [PageAreaRedaction](./pagearearedaction) | Representerar en komplex textuell redigering som påverkar text, bilder och kommentarer i ett område på sidan. |
| [PageRangeFilter](./pagerangefilter) | Representerar ett redigeringsfilter som anger ett sidintervall i ett dokument för att tillämpa redigering. |
| [RedactionDescription](./redactiondescription) | Representerar information om en enskild förändringsåtgärd som utfördes under redigeringsprocessen. |
| [RedactionFilter](./redactionfilter) | Representerar ett redigeringsfilter som anger omfattning i ett dokument för att tillämpa redigeringar. |
| [RegexRedaction](./regexredaction) | Representerar en textredigering som söker och ersätter text i dokumentet genom att matcha det angivna reguljära uttrycket. |
| [RegionReplacementOptions](./regionreplacementoptions) | Representerar färg‑ och områdesparametrar för bildområdesersättning. Se [`ImageAreaRedaction`](../groupdocs.redaction.redactions/imagearearedaction). |
| [RemovePageRedaction](./removepageredaction) | Representerar en redigering som tar bort en sida (bildspel, kalkylblad osv.) från ett dokument. |
| [ReplacementOptions](./replacementoptions) | Representerar alternativ för ersättning av matchande text. |
| [TextRedaction](./textredaction) | Representerar en bas‑abstrakt klass för dokumenttext‑redigeringar. |
| [TextReplacement](./textreplacement) | Representerar information om en textuell ersättning. |
## Gränssnitt

| Gränssnitt | Beskrivning |
| --- | --- |
| [ICustomRedactionHandler](./icustomredactionhandler) | Tillhandahåller ett gränssnitt för att implementera anpassad redigeringslogik. |
| [IRedactionCallback](./iredactioncallback) | Definierar metoder som krävs för att ta emot information om varje redigeringsändring och eventuellt förhindra den. |
## Uppräkning

| Uppräkning | Beskrivning |
| --- | --- |
| [MetadataFilters](./metadatafilters) | Representerar en lista över de vanligaste typerna av dokumentmetadata. |
| [PageSeekOrigin](./pageseekorigin) | Tillhandahåller fälten som representerar referenspunkter i ett dokument för sökning. |
| [RedactionActionType](./redactionactiontype) | Representerar åtgärder som kan vidtas för att utföra redigering. |
| [RedactionType](./redactiontype) | Representerar en typ av dokumentdata som påverkas av redigering. |
| [ReplacementType](./replacementtype) | Representerar en typ av ersättning för den matchade texten. |

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
