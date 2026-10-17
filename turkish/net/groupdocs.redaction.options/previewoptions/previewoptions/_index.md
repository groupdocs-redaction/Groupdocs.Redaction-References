---
title: "PreviewOptions"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Çıktı akışını kapatan PreviewOptions sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/groupdocs.redaction.options/previewoptions/previewoptions/
---
## PreviewOptions(CreatePageStream) {#constructor}

PreviewOptions sınıfının yeni bir örneğini başlatır, çıktı akışının kapanmasına neden olur.

```csharp
public PreviewOptions(CreatePageStream createPageStream)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| createPageStream | CreatePageStream | Belirli bir sayfa önizlemesi için bir akış oluşturur |

### Ayrıca Bakınız

* delegate [CreatePageStream](../../createpagestream)
* class [PreviewOptions](../../previewoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

---

## PreviewOptions(CreatePageStream, ReleasePageStream) {#constructor_1}

PreviewOptions sınıfının yeni bir örneğini başlatır, çıktı akışının daha sonraki kullanım için istemciye geri gönderilmesini sağlar.

```csharp
public PreviewOptions(CreatePageStream createPageStream, ReleasePageStream releasePageStream)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| createPageStream | CreatePageStream | Belirli bir sayfa önizlemesi için bir akış oluşturur |
| releasePageStream | ReleasePageStream | Sayfa önizlemesi oluşturmanın tamamlandığını bildirir ve çıktı akışını alır |

### Ayrıca Bakınız

* delegate [CreatePageStream](../../createpagestream)
* delegate [ReleasePageStream](../../releasepagestream)
* class [PreviewOptions](../../previewoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
