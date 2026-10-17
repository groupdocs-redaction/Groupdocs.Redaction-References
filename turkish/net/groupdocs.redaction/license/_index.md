---
title: "License"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Lisans uygulamak için yöntemler sağlar."
type: docs
weight: 270
url: /tr/net/groupdocs.redaction/license/
---
## License class

Lisans uygulamak için yöntemler sağlar.

```csharp
public class License
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [License](license)() | License sınıfının bir örneğini başlatır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [SetLicense](../../groupdocs.redaction/license/setlicense#setlicense)(Stream) | GroupDocs.Redaction lisansını bir akıştan ayarlar. |
| [SetLicense](../../groupdocs.redaction/license/setlicense#setlicense_1)(string) | GroupDocs.Redaction lisansını bir dosya yolundan ayarlar. |

### Açıklamalar

**Learn more**

* More about licensing: [GroupDocs Licensing FAQ](https://purchase.groupdocs.com/faqs/licensing)
* More about **GroupDocs.Redaction** licensing: [Evaluation Limitations and Licensing](https://docs.groupdocs.com/redaction/net/evaluation-limitations-and-licensing/)

### Örnekler

Aşağıdaki örnek, GroupDocs.Redaction için lisansın nasıl ayarlanacağını gösterir.

```csharp
GroupDocs.Redaction.License license = new GroupDocs.Redaction.License();
// alternatif olarak bir akış kullanabilirsiniz:
license.SetLicense(licensePath);
```

### Ayrıca Bakınız

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
