---
title: "ExactPhraseRedaction"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Belge metnindeki kesin ifadeyi varsayılan olarak büyük/küçük harfe duyarsız bir şekilde değiştiren bir metin gizleme temsil eder."
type: docs
weight: 600
url: /tr/net/groupdocs.redaction.redactions/exactphraseredaction/
---
## ExactPhraseRedaction class

Belgenin metnindeki tam ifadeyi, varsayılan olarak büyük/küçük harfe duyarsız bir şekilde değiştiren bir metin redaksiyonunu temsil eder.

```csharp
public class ExactPhraseRedaction : TextRedaction
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ExactPhraseRedaction](exactphraseredaction#constructor_1)(string, ReplacementOptions) | Büyük/küçük harfe duyarsız modda ExactPhraseRedaction sınıfının yeni bir örneğini başlatır. |
| [ExactPhraseRedaction](exactphraseredaction#constructor)(string, bool, ReplacementOptions) | ExactPhraseRedaction sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Metin değiştirme türünü belirten [`ReplacementOptions`](../replacementoptions) örneğini alır. |
| override [Description](../../groupdocs.redaction.redactions/exactphraseredaction/description) { get; } | Redaction ve parametrelerini tanımlayan bir dize döndürür. |
| [IsCaseSensitive](../../groupdocs.redaction.redactions/exactphraseredaction/iscasesensitive) { get; } | Aramanın büyük/küçük harfe duyarlı olup olmadığını gösteren bir değeri alır. |
| [IsRightToLeft](../../groupdocs.redaction.redactions/exactphraseredaction/isrighttoleft) { get; set; } | Bu metnin sağdan sola olup olmadığını gösteren bir değeri alır veya ayarlar, varsayılan olarak false. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Grafik içerikten metin çıkarmak için gerekli olan [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector) uygulamasını alır veya ayarlar. |
| [SearchPhrase](../../groupdocs.redaction.redactions/exactphraseredaction/searchphrase) { get; } | Aranacak ve değiştirilecek dizeyi alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/exactphraseredaction/applyto)(DocumentFormatInstance) | Redaction'ı verilen format örneğine uygular. |

### Açıklamalar

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

### Örnekler

Aşağıdaki örnek, büyük/küçük harfe duyarlı ifade arama ve değiştirme işlemini gösterir.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
  // Varsayılan olarak, isCaseSensitive = false;
  doc.Apply(new ExactPhraseRedaction("John Doe", true /*isCaseSensitive*/, new ReplacementOptions("[personal]")));
  doc.Save();
}
```

Aşağıdaki örnek, ifadeyi (büyük/küçük harfe duyarsız) katı kırmızı bir dikdörtgenle değiştirmeyi gösterir.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
  // Varsayılan olarak, isCaseSensitive = false;
  doc.Apply(new ExactPhraseRedaction("John Doe", new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Red)));
  doc.Save();
}
```

### Ayrıca Bakınız

* class [TextRedaction](../textredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
