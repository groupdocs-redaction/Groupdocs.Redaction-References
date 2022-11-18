---
title: ExactPhraseRedaction
second_title: .NET API Başvurusu için GroupDocs.Redaction
description: Belge metnindeki tam tümceyi değiştiren bir metin redaksiyonunu temsil eder varsayılan olarak büyük/küçük harf duyarlı değildir.
type: docs
weight: 480
url: /tr/net/groupdocs.redaction.redactions/exactphraseredaction/
---
## ExactPhraseRedaction class

Belge metnindeki tam tümceyi değiştiren bir metin redaksiyonunu temsil eder, varsayılan olarak büyük/küçük harf duyarlı değildir.

```csharp
public class ExactPhraseRedaction : TextRedaction
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [ExactPhraseRedaction](exactphraseredaction#constructor_1)(string, ReplacementOptions) | Büyük/küçük harfe duyarlı olmayan modda ExactPhraseRedaction sınıfının yeni bir örneğini başlatır. |
| [ExactPhraseRedaction](exactphraseredaction#constructor)(string, bool, ReplacementOptions) | ExactPhraseRedaction sınıfının yeni bir örneğini başlatır. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Şunu alır:[`ReplacementOptions`](../replacementoptions) örnek, metin değiştirme türünü belirterek. |
| override [Description](../../groupdocs.redaction.redactions/exactphraseredaction/description) { get; } | Düzeltmeyi ve parametrelerini açıklayan bir dize döndürür. |
| [IsCaseSensitive](../../groupdocs.redaction.redactions/exactphraseredaction/iscasesensitive) { get; } | Aramanın büyük/küçük harfe duyarlı olup olmadığını gösteren bir değer alır. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Şunu alır veya ayarlar:[`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector) uygulama, grafik içerikten metin çıkarmak için gereklidir. |
| [SearchPhrase](../../groupdocs.redaction.redactions/exactphraseredaction/searchphrase) { get; } | Aranacak ve değiştirilecek dizeyi alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/exactphraseredaction/applyto)(DocumentFormatInstance) | Redaksiyonu belirli bir biçim örneğine uygular. |

### Notlar

**Daha fazla bilgi edin**

* Redaksiyonları uygulama hakkında daha fazla ayrıntı: [Redaksiyonun temelleri](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Belge metni düzeltmeleri hakkında daha fazla ayrıntı: [Metin redaksiyonları](https://docs.groupdocs.com/redaction/net/text-redactions/)

### Örnekler

Aşağıdaki örnek, büyük/küçük harfe duyarlı tümcecik arama ve değiştirme işlemini gösterir. Aşağıdaki örnek, ifadenin (büyük/küçük harfe duyarsız) sabit kırmızı dikdörtgenle değiştirilmesini göstermektedir.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
  // Varsayılan olarak, isCaseSensitive = false;
  doc.Apply(new ExactPhraseRedaction("John Doe", true /*isCaseSensitive*/, new ReplacementOptions("[personal]")));
  doc.Save();
}
```

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
  // Varsayılan olarak, isCaseSensitive = false;
  doc.Apply(new ExactPhraseRedaction("John Doe", new ReplacementOptions(System.Drawing.Color.Red)));
  doc.Save();
}
```

### Ayrıca bakınız

* class [TextRedaction](../textredaction)
* ad alanı [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* toplantı [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->