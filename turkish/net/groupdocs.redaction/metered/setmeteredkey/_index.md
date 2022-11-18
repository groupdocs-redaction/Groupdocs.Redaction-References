---
title: SetMeteredKey
second_title: .NET API Başvurusu için GroupDocs.Redaction
description: Ürünü Ölçümlü tuşlarla etkinleştirir.
type: docs
weight: 20
url: /tr/net/groupdocs.redaction/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Ürünü Ölçümlü tuşlarla etkinleştirir.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| publicKey | String | Genel anahtar. |
| privateKey | String | Özel anahtar. |

### Örnekler

Aşağıdaki örnek, ürünün Ölçülü tuşlarla nasıl etkinleştirileceğini gösterir.

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);
```

### Ayrıca bakınız

* class [Metered](../../metered)
* ad alanı [GroupDocs.Redaction](../../metered)
* toplantı [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->