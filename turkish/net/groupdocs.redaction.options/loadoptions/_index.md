---
title: LoadOptions
second_title: .NET API Başvurusu için GroupDocs.Redaction
description: Bir dosyayı açmak için kullanılacak seçenekleri sağlar.
type: docs
weight: 300
url: /tr/net/groupdocs.redaction.options/loadoptions/
---
## LoadOptions class

Bir dosyayı açmak için kullanılacak seçenekleri sağlar.

```csharp
public class LoadOptions
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [LoadOptions](loadoptions#constructor)() | LoadOptions sınıfının yeni bir örneğini başlatır. |
| [LoadOptions](loadoptions#constructor_1)(string) | Belirtilen parola ile LoadOptions sınıfının yeni bir örneğini başlatır. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Password](../../groupdocs.redaction.options/loadoptions/password) { get; set; } | Parola korumalı belgeler için bir parola alır veya ayarlar. |

### Notlar

**Daha fazla bilgi edin**

* [Belgeleri yükleme](https://docs.groupdocs.com/redaction/net/loading-documents/)
* [Yerel diskten yükle](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
* [Akıştan yükle](https://docs.groupdocs.com/redaction/net/load-from-stream/)
* [Parola korumalı belge yükleyin](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

### Örnekler

Aşağıdaki örnek, parola korumalı belgenin nasıl açılacağını gösterir.

```csharp
LoadOptions loadOptions = new LoadOptions("mysecretpassword");
using (var redactor = new Redactor("PasswordProtected.pdf", loadOptions))
{
    // belge ile çalış
}
```

### Ayrıca bakınız

* ad alanı [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* toplantı [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->