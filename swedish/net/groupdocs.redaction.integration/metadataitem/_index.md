---
title: "MetadataItem"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar ett metadataobjekt som är gemensamt för alla stödda format och används i metadata‑redigeringar."
type: docs
weight: 220
url: /sv/net/groupdocs.redaction.integration/metadataitem/
---
## MetadataItem class

Representerar ett metadataobjekt, gemensamt för alla stödda format och använt i metadata‑maskeringar.

```csharp
public class MetadataItem : ISerializable
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [MetadataItem](metadataitem)() | Initierar en ny instans. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ActualValue](../../groupdocs.redaction.integration/metadataitem/actualvalue) { get; } | Hämtar strängrepresentationen av metadataobjektets värde. |
| [Category](../../groupdocs.redaction.integration/metadataitem/category) { get; set; } | Hämtar eller anger en kategori för metadataobjektet, till exempel resurs‑ID för ett inbäddat resurs‑metadataobjekt. |
| virtual [DictionaryKey](../../groupdocs.redaction.integration/metadataitem/dictionarykey) { get; } | Hämtar en nyckel för ordboken för [`MetadataCollection`](../metadatacollection) med hjälp av dess OriginalName och annan data. |
| [Filter](../../groupdocs.redaction.integration/metadataitem/filter) { get; set; } | Hämtar eller anger ett värde för [`MetadataFilters`](../../groupdocs.redaction.redactions/metadatafilters) som tilldelas detta metadataobjekt och som används i objektfiltrering. |
| [IsCustom](../../groupdocs.redaction.integration/metadataitem/iscustom) { get; set; } | Hämtar eller anger ett värde som visar om detta objekt är anpassat (tillagt av dokumentets författare). |
| [OriginalName](../../groupdocs.redaction.integration/metadataitem/originalname) { get; set; } | Hämtar eller anger det ursprungliga namnet på metadataobjektet, så som det visas i dokumentet. |
| [Values](../../groupdocs.redaction.integration/metadataitem/values) { get; set; } | Hämtar eller anger metadataobjektets värde. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| virtual [CreateClone](../../groupdocs.redaction.integration/metadataitem/createclone)() | Skapar en djup klon av den aktuella instansen. |
| virtual [GetObjectData](../../groupdocs.redaction.integration/metadataitem/getobjectdata)(SerializationInfo, StreamingContext) | Returnerar information om serialiserbara egenskaper. |

### Se även

* namespace [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
