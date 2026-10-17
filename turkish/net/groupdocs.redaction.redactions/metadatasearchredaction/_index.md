---
title: "MetadataSearchRedaction"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Anahtarları ve/veya değerleri eşleştiren düzenli ifadeler kullanarak meta verileri arayan ve gizleyen bir meta veri gizleme temsil eder."
type: docs
weight: 660
url: /tr/net/groupdocs.redaction.redactions/metadatasearchredaction/
---
## MetadataSearchRedaction class

Anahtarları ve/veya değerleri eşleştirerek düzenli ifadelerle meta verileri arayan ve redakte eden bir meta veri redaksiyonunu temsil eder.

```csharp
public class MetadataSearchRedaction : MetadataRedaction
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [MetadataSearchRedaction](metadatasearchredaction#constructor_2)(Regex, string) | Değeri, gizlenen öğeleri eşleştirmek için kullanarak MetadataSearchRedaction sınıfının yeni bir örneğini başlatır. |
| [MetadataSearchRedaction](metadatasearchredaction#constructor)(string, string) | Değeri, gizlenen öğeleri eşleştirmek için kullanarak MetadataSearchRedaction sınıfının yeni bir örneğini başlatır. |
| [MetadataSearchRedaction](metadatasearchredaction#constructor_3)(Regex, string, Regex) | Öğe adını ve değeri, gizlenen öğeleri eşleştirmek için kullanarak MetadataSearchRedaction sınıfının yeni bir örneğini başlatır. |
| [MetadataSearchRedaction](metadatasearchredaction#constructor_1)(string, string, string) | Öğe adını ve değeri, gizlenen öğeleri eşleştirmek için kullanarak MetadataSearchRedaction sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/metadatasearchredaction/description) { get; } | Redaction ve parametrelerini tanımlayan bir dize döndürür. |
| [Filter](../../groupdocs.redaction.redactions/metadataredaction/filter) { get; set; } | Tüm ya da belirli meta verileri (örneğin Yazar veya Şirket) seçmek için kullanılan filtreyi alır veya ayarlar. |
| [KeyExpression](../../groupdocs.redaction.redactions/metadatasearchredaction/keyexpression) { get; } | Meta veri öğesinin adını (anahtarını) eşleştirmek için düzenli ifadeyi alır. |
| [Replacement](../../groupdocs.redaction.redactions/metadatasearchredaction/replacement) { get; } | Metinsel değiştirme değerini alır. |
| [ValueExpression](../../groupdocs.redaction.redactions/metadatasearchredaction/valueexpression) { get; } | Meta veri öğesinin değer metnini eşleştirmek için düzenli ifadeyi alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/metadataredaction/applyto)(DocumentFormatInstance) | Redaction'ı verilen format örneğine uygular. |

### Açıklamalar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document metadata redactions: [Metadata redactions](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Örnekler

Aşağıdaki örnek, belirli meta verilerde belirli bir metni nasıl arayıp gizleyeceğinizi gösterir.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.docx"))
{
   MetadataSearchRedaction redaction = new MetadataSearchRedaction("Company Ltd.", "--company--");
   // Ayarlanmamışsa, tüm meta veri öğelerine uygulanır.
   redaction.Filter = MetadataFilters.Company;
   redactor.Apply(redaction);
   redactor.Save();
}
```

### Ayrıca Bakınız

* class [MetadataRedaction](../metadataredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
