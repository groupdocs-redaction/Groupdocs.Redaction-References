---
title: DeleteAnnotationRedaction
second_title: .NET API Başvurusu için GroupDocs.Redaction
description: Metin verilen normal ifadeyle eşleşiyorsa ek açıklamaları silen bir metin redaksiyonunu temsil eder isteğe bağlı olarak tüm ek açıklamaları siler.
type: docs
weight: 470
url: /tr/net/groupdocs.redaction.redactions/deleteannotationredaction/
---
## DeleteAnnotationRedaction class

Metin verilen normal ifadeyle eşleşiyorsa ek açıklamaları silen bir metin redaksiyonunu temsil eder (isteğe bağlı olarak tüm ek açıklamaları siler).

```csharp
public class DeleteAnnotationRedaction : Redaction
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [DeleteAnnotationRedaction](deleteannotationredaction#constructor)() | Tüm ek açıklamaları silme ayarlarıyla (her şeyle eşleşen) DeleteAnnotationRedaction sınıfının yeni bir örneğini başlatır. |
| [DeleteAnnotationRedaction](deleteannotationredaction#constructor_2)(Regex) | Verilen ifadeyle eşleşen açıklamaları silerek, DeleteAnnotationRedaction sınıfının yeni bir örneğini başlatır. |
| [DeleteAnnotationRedaction](deleteannotationredaction#constructor_1)(string) | Verilen ifadeyle eşleşen açıklamaları silerek, DeleteAnnotationRedaction sınıfının yeni bir örneğini başlatır. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/deleteannotationredaction/description) { get; } | Düzeltmeyi ve parametrelerini açıklayan bir dize döndürür. |
| [Expression](../../groupdocs.redaction.redactions/deleteannotationredaction/expression) { get; } | Eşleşecek normal ifadeyi alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/deleteannotationredaction/applyto)(DocumentFormatInstance) | Redaksiyonu belirli bir biçim örneğine uygular. |

### Notlar

**Daha fazla bilgi edin**

* Redaksiyonları uygulama hakkında daha fazla ayrıntı: [Redaksiyonun temelleri](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Belge açıklama düzeltmeleri hakkında daha fazla ayrıntı: [Ek açıklama düzenlemeleri](https://docs.groupdocs.com/redaction/net/annotation-redactions/)

### Örnekler

Aşağıdaki örnek, "kullan", "göster" veya "açıkla" sözcüklerini içeren tüm ek açıklamaların belgeden nasıl kaldırılacağını (ve diğerlerini nasıl bırakılacağını) gösterir.

```csharp
using (Redactor redactor = new Redactor(@"D:\test.docx"))
{
   redactor.Apply(new DeleteAnnotationRedaction("(?im:(use|show|describe))"));
   redactor.Save()
}
```

### Ayrıca bakınız

* class [Redaction](../../groupdocs.redaction/redaction)
* ad alanı [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* toplantı [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
