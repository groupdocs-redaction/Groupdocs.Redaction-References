---
title: "DeleteAnnotationRedaction"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Verilen düzenli ifadeye uyan metin için ek açıklamaları silen bir metin redaksiyonunu temsil eder, isteğe bağlı olarak tüm ek açıklamaları da siler."
type: docs
weight: 580
url: /tr/net/groupdocs.redaction.redactions/deleteannotationredaction/
---
## DeleteAnnotationRedaction class

Metin verilen bir düzenli ifadeye uyuyorsa açıklamaları (isteğe bağlı olarak tüm açıklamaları) silen bir metin redaksiyonunu temsil eder.

```csharp
public class DeleteAnnotationRedaction : Redaction
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [DeleteAnnotationRedaction](deleteannotationredaction#constructor)() | DeleteAnnotationRedaction sınıfının yeni bir örneğini, tüm ek açıklamaları (her şeyi eşleştirerek) silmek için ayarlarla başlatır. |
| [DeleteAnnotationRedaction](deleteannotationredaction#constructor_2)(Regex) | DeleteAnnotationRedaction sınıfının yeni bir örneğini, verilen ifadeye uyan ek açıklamaları silerek başlatır. |
| [DeleteAnnotationRedaction](deleteannotationredaction#constructor_1)(string) | DeleteAnnotationRedaction sınıfının yeni bir örneğini, verilen ifadeye uyan ek açıklamaları silerek başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/deleteannotationredaction/description) { get; } | Redaction ve parametrelerini tanımlayan bir dize döndürür. |
| [Expression](../../groupdocs.redaction.redactions/deleteannotationredaction/expression) { get; } | Eşleşecek düzenli ifadeyi alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/deleteannotationredaction/applyto)(DocumentFormatInstance) | Redaction'ı verilen format örneğine uygular. |

### Açıklamalar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document annotation redactions: [Annotation redactions](https://docs.groupdocs.com/redaction/net/annotation-redactions/)

### Örnekler

Aşağıdaki örnek, belgede "use", "show" veya "describe" sözcüklerini içeren tüm ek açıklamaları nasıl kaldırıp diğerlerini bırakacağını gösterir.

```csharp
using (Redactor redactor = new Redactor(@"D:\test.docx"))
{
   redactor.Apply(new DeleteAnnotationRedaction("(?im:(use|show|describe))"));
   redactor.Save()
}
```

### Ayrıca Bakınız

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
