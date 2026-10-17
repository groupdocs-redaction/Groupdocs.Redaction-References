---
title: "Nokta"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Genellikle bir redaksiyon alanının sol üst köşesi olan sayfa veya görüntüdeki piksel kaydırmasını tanımlar."
type: docs
weight: 340
url: /tr/net/groupdocs.redaction.options.drawing/point/
---
## Point structure

Bir sayfa veya görüntü üzerindeki piksel kaydırmasını tanımlar, genellikle kırpma alanının sol üst köşesidir.

```csharp
public struct Point : IEquatable<Point>
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [Point](point)(int, int) | Redaksiyon bölgesi kökeni için bir nokta oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| static [Empty](../../groupdocs.redaction.options.drawing/point/empty) { get; } | Köken (0, 0) noktasında bir nokta. |
| [X](../../groupdocs.redaction.options.drawing/point/x) { get; } | Sol kenardan, piksel cinsinden yatay kaydırma. |
| [Y](../../groupdocs.redaction.options.drawing/point/y) { get; } | Üst kenardan, piksel cinsinden dikey kaydırma. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [Equals](../../groupdocs.redaction.options.drawing/point/equals#equals_1)(object) | Bu noktayı başka bir nesneyle karşılaştırır. |
| [Equals](../../groupdocs.redaction.options.drawing/point/equals#equals)(Point) | Koordinatları başka bir nokta ile karşılaştırır. |
| override [GetHashCode](../../groupdocs.redaction.options.drawing/point/gethashcode)() | Koordinatlardan türetilen bir hash kodu döndürür. |
| override [ToString](../../groupdocs.redaction.options.drawing/point/tostring)() | Koordinatları okunabilir bir biçimde döndürür. |

### Ayrıca Bakınız

* namespace [GroupDocs.Redaction.Options.Drawing](../../groupdocs.redaction.options.drawing)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
