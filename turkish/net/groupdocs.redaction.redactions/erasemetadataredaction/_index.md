---
title: "EraseMetadataRedaction"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Belgedeki tüm meta verileri veya belirli MetadataFilters ile eşleşen meta verileri silen bir meta veri redaksiyonunu temsil eder."
type: docs
weight: 590
url: /tr/net/groupdocs.redaction.redactions/erasemetadataredaction/
---
## EraseMetadataRedaction class

Belgedeki tüm meta verileri veya belirli MetadataFilters ile eşleşen meta verileri silen bir meta veri redaksiyonunu temsil eder.

```csharp
public class EraseMetadataRedaction : MetadataRedaction
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [EraseMetadataRedaction](erasemetadataredaction#constructor)() | EraseMetadataRedaction sınıfının yeni bir örneğini başlatır, tüm meta verileri siler. |
| [EraseMetadataRedaction](erasemetadataredaction#constructor_1)(MetadataFilters) | EraseMetadataRedaction sınıfının yeni bir örneğini başlatır, meta verileri siler, belirli bir [`MetadataFilters`](../metadatafilters) kombinasyonunu eşleştirir. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/erasemetadataredaction/description) { get; } | Redaction ve parametrelerini tanımlayan bir dize döndürür. |
| [Filter](../../groupdocs.redaction.redactions/metadataredaction/filter) { get; set; } | Tüm ya da belirli meta verileri (örneğin Yazar veya Şirket) seçmek için kullanılan filtreyi alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/metadataredaction/applyto)(DocumentFormatInstance) | Redaction'ı verilen format örneğine uygular. |

### Açıklamalar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document metadata redactions: [Metadata redactions](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Örnekler

Aşağıdaki örnek, tüm ya da belirli meta verileri (boş değerlere ayarlayarak) nasıl sileceğinizi gösterir.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.docx"))
{
   // Yazar, Yönetici ve Şirketi sil
   redactor.Apply(new EraseMetadataRedaction(MetadataFilters.Author | MetadataFilters.Manager | MetadataFilters.Company));
   // Tüm meta verileri sil
   redactor.Apply(new EraseMetadataRedaction(MetadataFilters.All));
   redactor.Save();
}
```

### Ayrıca Bakınız

* class [MetadataRedaction](../metadataredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
