---
title: MetadataItem
second_title: GroupDocs.Redaction untuk Referensi .NET API
description: Mewakili item metadata umum untuk semua format yang didukung dan digunakan dalam redaksi metadata.
type: docs
weight: 210
url: /id/net/groupdocs.redaction.integration/metadataitem/
---
## MetadataItem class

Mewakili item metadata, umum untuk semua format yang didukung dan digunakan dalam redaksi metadata.

```csharp
public class MetadataItem : ISerializable
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [MetadataItem](metadataitem)() | Menginisialisasi instance baru. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [ActualValue](../../groupdocs.redaction.integration/metadataitem/actualvalue) { get; } | Mendapat representasi string dari nilai item metadata. |
| [Category](../../groupdocs.redaction.integration/metadataitem/category) { get; set; } | Mendapat atau menyetel kategori item metadata, misalnya ID sumber daya untuk item metadata sumber tersemat. |
| virtual [DictionaryKey](../../groupdocs.redaction.integration/metadataitem/dictionarykey) { get; } | Mendapat kunci kamus untuk[`MetadataCollection`](../metadatacollection) , menggunakan OriginalName dan data lainnya. |
| [Filter](../../groupdocs.redaction.integration/metadataitem/filter) { get; set; } | Mendapat atau menetapkan nilai[`MetadataFilters`](../../groupdocs.redaction.redactions/metadatafilters) , ditetapkan ke item metadata ini yang digunakan dalam pemfilteran item. |
| [IsCustom](../../groupdocs.redaction.integration/metadataitem/iscustom) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah item ini khusus (ditambahkan oleh penulis dokumen). |
| [OriginalName](../../groupdocs.redaction.integration/metadataitem/originalname) { get; set; } | Mendapat atau menyetel nama asli item metadata, seperti yang muncul di dokumen. |
| [Values](../../groupdocs.redaction.integration/metadataitem/values) { get; set; } | Mendapat atau menyetel nilai item metadata. |

## Metode

| Nama | Keterangan |
| --- | --- |
| virtual [CreateClone](../../groupdocs.redaction.integration/metadataitem/createclone)() | Membuat tiruan dalam dari instance saat ini. |
| virtual [GetObjectData](../../groupdocs.redaction.integration/metadataitem/getobjectdata)(SerializationInfo, StreamingContext) | Mengembalikan informasi tentang properti serializable. |

### Lihat juga

* ruang nama [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* perakitan [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->