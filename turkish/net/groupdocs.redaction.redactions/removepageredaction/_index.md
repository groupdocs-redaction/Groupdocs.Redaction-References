---
title: "RemovePageRedaction"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Bir belgeden sayfa, slayt, çalışma sayfası vb. kaldıran bir gizleme temsil eder."
type: docs
weight: 770
url: /tr/net/groupdocs.redaction.redactions/removepageredaction/
---
## RemovePageRedaction class

Bir belgeden sayfa (slayt, çalışma sayfası vb.) kaldıran bir redaksiyonu temsil eder.

```csharp
public class RemovePageRedaction : Redaction
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [RemovePageRedaction](removepageredaction)(PageSeekOrigin, int, int) | RemovePageRedaction sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../groupdocs.redaction.redactions/removepageredaction/count) { get; } | Kaldırılacak sayfa sayısını alır. |
| virtual [Description](../../groupdocs.redaction/redaction/description) { get; } | Redaction ve parametrelerini tanımlayan bir dize döndürür. |
| [Index](../../groupdocs.redaction.redactions/removepageredaction/index) { get; } | Başlangıç konumu indeksini (0 tabanlı) alır. |
| [Origin](../../groupdocs.redaction.redactions/removepageredaction/origin) { get; } | Belgenin başlangıcı ya da sonu olan arama referans konumunu alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/removepageredaction/applyto)(DocumentFormatInstance) | Redaction'ı verilen format örneğine uygular. |

### Açıklamalar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about removing pages: [Remove page redaction](https://docs.groupdocs.com/redaction/net/remove-page-redaction/)

### Örnekler

Aşağıdaki örnek, belgenin son sayfasını nasıl kaldıracağınızı gösterir.

```csharp
using (Redactor redactor = new Redactor(@"C:\test.pdf"))
{
   redactor.Apply(new RemovePageRedaction(PageSeekOrigin.End, 0, 1));
   redactor.Save()
}
```

### Ayrıca Bakınız

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
