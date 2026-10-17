---
title: "Ölçümlü"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Metered lisans ile ürünü etkinleştirmeyi ve işlenen MB miktarını almaya izin veren yöntemler sağlar. Metered lisanslar hakkında daha fazla bilgi için buraya https//purchase.groupdocs.com/faqs/licensing/metered."
type: docs
weight: 280
url: /tr/net/groupdocs.redaction/metered/
---
## Metered class

Ürünü Ölçülen lisans ile etkinleştirmeyi ve işlenen MB miktarını almayı sağlayan yöntemler sunar. Ölçülen lisanslar hakkında daha fazla bilgi için [buraya](https://purchase.groupdocs.com/faqs/licensing/metered) bakın.

```csharp
public class Metered
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [Metered](metered)() | Metered sınıfının yeni bir örneğini başlatır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [SetMeteredKey](../../groupdocs.redaction/metered/setmeteredkey)(string, string) | Ürünü Metered anahtarlarıyla etkinleştirir. |
| static [GetConsumptionCredit](../../groupdocs.redaction/metered/getconsumptioncredit)() | Tüketim kredisini alır. |
| static [GetConsumptionQuantity](../../groupdocs.redaction/metered/getconsumptionquantity)() | İşlenen MB miktarını alır. |

### Açıklamalar

**Learn more**

* More about licensing: [GroupDocs Licensing FAQ](https://purchase.groupdocs.com/faqs/licensing)
* More about **GroupDocs.Redaction** licensing: [Evaluation Limitations and Licensing](https://docs.groupdocs.com/redaction/net/evaluation-limitations-and-licensing/)

### Örnekler

Aşağıdaki örnek, ürünü Metered anahtarlarıyla nasıl etkinleştireceğini gösterir.

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

### Ayrıca Bakınız

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
