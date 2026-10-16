---
title: "SetMeteredKey"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Activeert het product met Metered-sleutels."
type: docs
weight: 20
url: /nl/net/groupdocs.redaction/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Activeert het product met Metered-sleutels.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| publicKey | String | De public key. |
| privateKey | String | De private key. |

### Voorbeelden

Het volgende voorbeeld toont hoe het product te activeren met Metered-sleutels.

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);
```

### Zie ook

* class [Metered](../../metered)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
