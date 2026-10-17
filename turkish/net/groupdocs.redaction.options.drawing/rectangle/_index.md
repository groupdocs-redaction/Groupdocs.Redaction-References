---
title: "Dikdörtgen"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Bir sayfa veya görüntü üzerindeki dikdörtgen alanı, örneğin bir OCR metin sınırı veya bir redaksiyon kutusu olarak tanımlar."
type: docs
weight: 350
url: /tr/net/groupdocs.redaction.options.drawing/rectangle/
---
## Rectangle structure

Bir sayfa veya görüntü üzerindeki dikdörtgen alanı tanımlar, örneğin bir OCR metin sınırı veya kırpma kutusu.

```csharp
public struct Rectangle : IEquatable<Rectangle>
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [Rectangle](rectangle#constructor)(Point, Size) | Üst sol nokta ve bölge boyutundan bir dikdörtgen oluşturur. |
| [Rectangle](rectangle#constructor_1)(int, int, int, int) | Köşe koordinatları ve boyutlardan bir dikdörtgen oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| static [Empty](../../groupdocs.redaction.options.drawing/rectangle/empty) { get; } | Orijinde sıfır genişlik ve yükseklikte bir dikdörtgen. |
| [Height](../../groupdocs.redaction.options.drawing/rectangle/height) { get; set; } | Alan yüksekliği, piksel cinsinden. |
| [IsEmpty](../../groupdocs.redaction.options.drawing/rectangle/isempty) { get; } | Dikdörtgenin boş olup olmadığını gösteren bir değer alır. |
| [Location](../../groupdocs.redaction.options.drawing/rectangle/location) { get; } | Dikdörtgenin üst sol köşesi. |
| [Size](../../groupdocs.redaction.options.drawing/rectangle/size) { get; } | Dikdörtgenin genişliği ve yüksekliği. |
| [Width](../../groupdocs.redaction.options.drawing/rectangle/width) { get; set; } | Alan genişliği, piksel cinsinden. |
| [X](../../groupdocs.redaction.options.drawing/rectangle/x) { get; set; } | Üst sol köşenin yatay konumu, piksel cinsinden. |
| [Y](../../groupdocs.redaction.options.drawing/rectangle/y) { get; set; } | Üst sol köşenin dikey konumu, piksel cinsinden. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [Equals](../../groupdocs.redaction.options.drawing/rectangle/equals#equals_1)(object) | Bu dikdörtgeni başka bir nesneyle karşılaştırır. |
| [Equals](../../groupdocs.redaction.options.drawing/rectangle/equals#equals)(Rectangle) | Sınırları başka bir dikdörtgenle karşılaştırır. |
| override [GetHashCode](../../groupdocs.redaction.options.drawing/rectangle/gethashcode)() | Konum ve boyuttan türetilen bir karma kodu döndürür. |
| override [ToString](../../groupdocs.redaction.options.drawing/rectangle/tostring)() | Sınırları okunabilir bir biçimde döndürür. |

### Ayrıca Bakınız

* namespace [GroupDocs.Redaction.Options.Drawing](../../groupdocs.redaction.options.drawing)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
