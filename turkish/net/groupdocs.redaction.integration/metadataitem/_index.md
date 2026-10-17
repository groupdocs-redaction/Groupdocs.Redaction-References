---
title: "MetadataItem"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Desteklenen tüm formatlar için ortak olan ve metadata redaksiyonlarında kullanılan bir metadata öğesini temsil eder."
type: docs
weight: 220
url: /tr/net/groupdocs.redaction.integration/metadataitem/
---
## MetadataItem class

Tüm desteklenen formatlar için ortak olan ve metadata redaksiyonlarında kullanılan bir metadata öğesini temsil eder.

```csharp
public class MetadataItem : ISerializable
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [MetadataItem](metadataitem)() | Yeni bir örnek başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ActualValue](../../groupdocs.redaction.integration/metadataitem/actualvalue) { get; } | Metadata öğesi değerinin dize temsilini alır. |
| [Category](../../groupdocs.redaction.integration/metadataitem/category) { get; set; } | Metadata öğesinin bir kategorisini alır veya ayarlar, örneğin gömülü kaynak metadata öğesi için kaynak kimliği. |
| virtual [DictionaryKey](../../groupdocs.redaction.integration/metadataitem/dictionarykey) { get; } | [`MetadataCollection`](../metadatacollection) için, OriginalName ve diğer verileri kullanarak bir sözlük anahtarı alır. |
| [Filter](../../groupdocs.redaction.integration/metadataitem/filter) { get; set; } | Bu metadata öğesine atanan ve öğe filtrelemesinde kullanılan [`MetadataFilters`](../../groupdocs.redaction.redactions/metadatafilters) değerini alır veya ayarlar. |
| [IsCustom](../../groupdocs.redaction.integration/metadataitem/iscustom) { get; set; } | Bu öğenin özel olup olmadığını (belgenin yazarları tarafından eklenmiş) gösteren bir değeri alır veya ayarlar. |
| [OriginalName](../../groupdocs.redaction.integration/metadataitem/originalname) { get; set; } | Metadata öğesinin belgede göründüğü orijinal adını alır veya ayarlar. |
| [Values](../../groupdocs.redaction.integration/metadataitem/values) { get; set; } | Metadata öğesi değerini alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| virtual [CreateClone](../../groupdocs.redaction.integration/metadataitem/createclone)() | Mevcut örneğin derin bir kopyasını oluşturur. |
| virtual [GetObjectData](../../groupdocs.redaction.integration/metadataitem/getobjectdata)(SerializationInfo, StreamingContext) | Serileştirilebilir özellikler hakkında bilgi döndürür. |

### Ayrıca Bakınız

* namespace [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
