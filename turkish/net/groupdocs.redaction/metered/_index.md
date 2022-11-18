---
title: Metered
second_title: .NET API Başvurusu için GroupDocs.Redaction
description: Ürünün Metered lisansıyla etkinleştirilmesine ve işlenen MB miktarının alınmasına izin veren yöntemler sağlar. Metered lisansları hakkında daha fazla bilgi edininburadahttps//purchase.groupdocs.com/faqs/licensing/metered .
type: docs
weight: 270
url: /tr/net/groupdocs.redaction/metered/
---
## Metered class

Ürünün Metered lisansıyla etkinleştirilmesine ve işlenen MB miktarının alınmasına izin veren yöntemler sağlar. Metered lisansları hakkında daha fazla bilgi edinin[burada](https://purchase.groupdocs.com/faqs/licensing/metered) .

```csharp
public class Metered
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [Metered](metered)() | Ölçülen sınıfın yeni bir örneğini başlatır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [SetMeteredKey](../../groupdocs.redaction/metered/setmeteredkey)(string, string) | Ürünü Ölçümlü tuşlarla etkinleştirir. |
| static [GetConsumptionCredit](../../groupdocs.redaction/metered/getconsumptioncredit)() | Tüketim kredisini alır. |
| static [GetConsumptionQuantity](../../groupdocs.redaction/metered/getconsumptionquantity)() | İşlenen MB miktarını alır. |

### Notlar

**Daha fazla bilgi edin**

* Lisanslama hakkında daha fazlası: [GroupDocs Lisanslama SSS](https://purchase.groupdocs.com/faqs/licensing)
* hakkında daha fazla bilgi**GroupDocs.Redaksiyon** lisanslama: [Değerlendirme Sınırlamaları ve Lisanslama](https://docs.groupdocs.com/redaction/net/evaluation-limitations-and-licensing/)

### Örnekler

Aşağıdaki örnek, ürünün Ölçülen tuşlarla nasıl etkinleştirileceğini gösterir.

```csharp
[C#]

Metered matered = new Metered();
matered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim matered As Metered = New Metered
matered.SetMeteredKey("PublicKey", "PrivateKey")
```

bileşen jar dosyası:

```csharp
Metered matered = new Metered();
matered.setMeteredKey("PublicKey", "PrivateKey");
```

### Ayrıca bakınız

* ad alanı [GroupDocs.Redaction](../../groupdocs.redaction)
* toplantı [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->