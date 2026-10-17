---
title: "GetConsumptionQuantity"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "İşlenen MB miktarını alır."
type: docs
weight: 40
url: /tr/net/groupdocs.redaction/metered/getconsumptionquantity/
---
## Metered.GetConsumptionQuantity method

İşlenen MB miktarını alır.

```csharp
public static decimal GetConsumptionQuantity()
```

### Dönüş Değeri

tüketim miktarı

### Örnekler

Aşağıdaki örnek, işlenen MB miktarını nasıl alacağınızı gösterir.

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);

decimal mbProcessed = Metered.GetConsumptionQuantity();
```

### Ayrıca Bakınız

* class [Metered](../../metered)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
