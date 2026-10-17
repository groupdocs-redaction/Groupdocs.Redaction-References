---
title: "LoadOptions"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Bir dosyayı açmak için kullanılacak seçenekleri sağlar."
type: docs
weight: 380
url: /tr/net/groupdocs.redaction.options/loadoptions/
---
## LoadOptions class

Bir dosyayı açmak için kullanılacak seçenekleri sağlar.

```csharp
public class LoadOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [LoadOptions](loadoptions#constructor)() | LoadOptions sınıfının yeni bir örneğini başlatır. |
| [LoadOptions](loadoptions#constructor_1)(bool) | Belirtilen ön rasterleştirme bayrağı ile LoadOptions sınıfının yeni bir örneğini başlatır. |
| [LoadOptions](loadoptions#constructor_2)(FileType) | Belirtilen dosya türü ile LoadOptions sınıfının yeni bir örneğini başlatır. |
| [LoadOptions](loadoptions#constructor_3)(string) | Belirtilen şifre ile LoadOptions sınıfının yeni bir örneğini başlatır. |
| [LoadOptions](loadoptions#constructor_4)(string, bool) | Belirtilen şifre ile LoadOptions sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [FileType](../../groupdocs.redaction.options/loadoptions/filetype) { get; set; } | Açılacak dosyanın türünü alır veya ayarlar. |
| [Password](../../groupdocs.redaction.options/loadoptions/password) { get; set; } | Şifre korumalı belgeler için bir şifre alır veya ayarlar. |
| [PreRasterize](../../groupdocs.redaction.options/loadoptions/prerasterize) { get; set; } | Dosyanın ön rasterleştirileceğini gösteren bir değeri alır veya ayarlar. |

### Açıklamalar

**Learn more**

* [Loading documents](https://docs.groupdocs.com/redaction/net/loading-documents/)
* [Load from local disk](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
* [Load from stream](https://docs.groupdocs.com/redaction/net/load-from-stream/)
* [Load password-protected document](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

### Örnekler

Aşağıdaki örnek, şifre korumalı belgeyi nasıl açacağınızı gösterir.

```csharp
LoadOptions loadOptions = new LoadOptions("mysecretpassword");
using (var redactor = new Redactor("PasswordProtected.pdf", loadOptions))
{
    // Belgeyle çalış
}
```

### Ayrıca Bakınız

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
