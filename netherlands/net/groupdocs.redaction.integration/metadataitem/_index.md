---
title: "MetadataItem"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Stelt een metadata‑item voor dat gemeenschappelijk is voor alle ondersteunde formaten en wordt gebruikt bij metadata‑redacties."
type: docs
weight: 220
url: /nl/net/groupdocs.redaction.integration/metadataitem/
---
## MetadataItem class

Stelt een metadata-item voor, gemeenschappelijk voor alle ondersteunde formaten en gebruikt bij metadata-redigeringen.

```csharp
public class MetadataItem : ISerializable
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [MetadataItem](metadataitem)() | Initialiseert een nieuw exemplaar. |

## Properties

| Naam | Beschrijving |
| --- | --- |
| [ActualValue](../../groupdocs.redaction.integration/metadataitem/actualvalue) { get; } | Haalt de tekenreeksrepresentatie op van de waarde van het metadata‑item. |
| [Category](../../groupdocs.redaction.integration/metadataitem/category) { get; set; } | Haalt op of stelt een categorie in van het metadata‑item, bijvoorbeeld resource‑ID voor een ingebed resource‑metadata‑item. |
| virtual [DictionaryKey](../../groupdocs.redaction.integration/metadataitem/dictionarykey) { get; } | Haalt een woordenboek‑sleutel op voor [`MetadataCollection`](../metadatacollection), met gebruik van de OriginalName en andere gegevens. |
| [Filter](../../groupdocs.redaction.integration/metadataitem/filter) { get; set; } | Haalt op of stelt een waarde in van [`MetadataFilters`](../../groupdocs.redaction.redactions/metadatafilters), toegewezen aan dit metadata‑item dat wordt gebruikt bij item‑filtratie. |
| [IsCustom](../../groupdocs.redaction.integration/metadataitem/iscustom) { get; set; } | Haalt op of stelt een waarde in die aangeeft of dit item aangepast is (toegevoegd door de auteurs van het document). |
| [OriginalName](../../groupdocs.redaction.integration/metadataitem/originalname) { get; set; } | Haalt op of stelt een oorspronkelijke naam in van het metadata‑item, zoals het in het document voorkomt. |
| [Values](../../groupdocs.redaction.integration/metadataitem/values) { get; set; } | Haalt op of stelt de waarde van het metadata‑item in. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| virtual [CreateClone](../../groupdocs.redaction.integration/metadataitem/createclone)() | Maakt een diepe kloon van de huidige instantie. |
| virtual [GetObjectData](../../groupdocs.redaction.integration/metadataitem/getobjectdata)(SerializationInfo, StreamingContext) | Retourneert informatie over serialiseerbare eigenschappen. |

### Zie ook

* namespace [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
