---
title: "AnnotationRedaction"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Belirli bir düzenli ifadeye uyan açıklama metni, yorumlar vb. yerine geçen bir redaksiyonu temsil eder."
type: docs
weight: 530
url: /tr/net/groupdocs.redaction.redactions/annotationredaction/
---
## AnnotationRedaction class

Verilen bir düzenli ifadeye uyan açıklama metnini (yorumlar vb.) değiştiren bir redaksiyonu temsil eder.

```csharp
public class AnnotationRedaction : Redaction
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [AnnotationRedaction](annotationredaction#constructor_1)(Regex, string) | AnnotationRedaction sınıfının yeni bir örneğini başlatır. |
| [AnnotationRedaction](annotationredaction#constructor)(string, string) | AnnotationRedaction sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/annotationredaction/description) { get; } | Redaction ve parametrelerini tanımlayan bir dize döndürür. |
| [Expression](../../groupdocs.redaction.redactions/annotationredaction/expression) { get; } | Eşleşecek düzenli ifadeyi alır. |
| [Replacement](../../groupdocs.redaction.redactions/annotationredaction/replacement) { get; } | Eşleşen metin için metinsel bir değiştirme alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/annotationredaction/applyto)(DocumentFormatInstance) | Redaction'ı verilen format örneğine uygular. |

### Açıklamalar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document annotation redactions: [Annotation redactions](https://docs.groupdocs.com/redaction/net/annotation-redactions/)

### Örnekler

Aşağıdaki örnek, tüm açıklamalarda "John" adını "[redacted]" ile nasıl değiştireceğini gösterir.

```csharp
using (Redactor redactor = new Redactor(@"C:\test.pdf"))
{
   redactor.Apply(new AnnotationRedaction("(?im:john)", "[redacted]"));
   redactor.Save()
}
```

### Ayrıca Bakınız

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
