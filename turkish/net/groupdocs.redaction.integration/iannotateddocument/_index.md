---
title: "IAnnotatedDocument"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Yorumlar gibi ek açıklamalara erişim için gerekli yöntemleri tanımlar. Ek açıklama redaksiyonlarını gerçekleştirmek için DocumentFormatInstance./documentformatinstancederived sınıfı tarafından uygulanması gerekir."
type: docs
weight: 120
url: /tr/net/groupdocs.redaction.integration/iannotateddocument/
---
## IAnnotatedDocument interface

Yorumlar gibi ek açıklamalara erişim için gerekli yöntemleri tanımlar. Ek açıklama redaksiyonlarını gerçekleştirmek için [`DocumentFormatInstance`](../documentformatinstance)-türetilmiş sınıf tarafından uygulanması gerekir.

```csharp
public interface IAnnotatedDocument
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [DeleteAnnotations](../../groupdocs.redaction.integration/iannotateddocument/deleteannotations)(Regex) | Belge içinde düzenli ifadeye uyan tüm ek açıklamaları siler. |
| [RedactAnnotation](../../groupdocs.redaction.integration/iannotateddocument/redactannotation)(Regex, string) | Belge içindeki tüm ek açıklamalarda eşleşen metni değiştirir. |

### Açıklamalar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document annotation redactions: [Annotation redactions](https://docs.groupdocs.com/redaction/net/annotation-redactions/)
* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Ayrıca Bakınız

* namespace [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
