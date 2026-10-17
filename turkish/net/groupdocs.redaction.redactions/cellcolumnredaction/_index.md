---
title: "CellColumnRedaction"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Bir elektronik tablo, CSV, Excel vb. belgelerdeki metni değiştiren bir metin redaksiyonunu temsil eder."
type: docs
weight: 540
url: /tr/net/groupdocs.redaction.redactions/cellcolumnredaction/
---
## CellColumnRedaction class

Bir elektronik tablo belgesindeki (CSV, Excel vb.) metni değiştiren bir metin redaksiyonunu temsil eder.

```csharp
public class CellColumnRedaction : TextRedaction
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [CellColumnRedaction](cellcolumnredaction)(CellFilter, Regex, ReplacementOptions) | CellColumnRedaction sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Metin değiştirme türünü belirten [`ReplacementOptions`](../replacementoptions) örneğini alır. |
| override [Description](../../groupdocs.redaction.redactions/cellcolumnredaction/description) { get; } | Redaction ve parametrelerini tanımlayan bir dize döndürür. |
| [Filter](../../groupdocs.redaction.redactions/cellcolumnredaction/filter) { get; } | Sütun ve çalışma sayfası filtresini alır. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Grafik içerikten metin çıkarmak için gerekli olan [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector) uygulamasını alır veya ayarlar. |
| [Pattern](../../groupdocs.redaction.redactions/cellcolumnredaction/pattern) { get; } | Eşleşecek düzenli ifadeyi alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/cellcolumnredaction/applyto)(DocumentFormatInstance) | Redaction'ı verilen format örneğine uygular. |

### Açıklamalar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about spreadsheet redactions: [Spreadsheet redactions](https://docs.groupdocs.com/redaction/net/spreadsheet-redactions/)

### Örnekler

Aşağıdaki örnek, bir elektronik tablo belgesindeki "Customers" çalışma sayfasının ikinci sütunundan kullanıcı e-postalarını kaldırmayı gösterir.

```csharp
using (Redactor redactor = new Redactor("D:\\Sales in September.xslx"))
{
   var filter = new CellFilter()
   {
       ColumnIndex = 1, // zero-based 2nd column
       WorkSheetName = "Customers"
   };
   var expression = new Regex("^\\w+([-+.']\\w+)*@\\w+([-.]\\w+)*\\.\\w+([-.]\\w+)*$");
   RedactorChangeLog changeLog = redactor.Apply(new CellColumnRedaction(filter, expression, new ReplacementOptions("[customer email]")));
   if (result.Status != RedactionStatus.Failed)
   {
      doc.Save(new SaveOptions() { AddSuffix = true });
   };
}
```

### Ayrıca Bakınız

* class [TextRedaction](../textredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
