---
title: "SetMeteredKey"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Ürünü Metered anahtarlarıyla etkinleştirir."
type: docs
weight: 20
url: /tr/net/groupdocs.redaction/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Ürünü Metered anahtarlarıyla etkinleştirir.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| publicKey | String | Açık anahtar. |
| privateKey | String | Özel anahtar. |

### Örnekler

Aşağıdaki örnek, ürünü Metered anahtarlarıyla nasıl etkinleştireceğini gösterir.

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);
```

### Ayrıca Bakınız

* class [Metered](../../metered)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->
