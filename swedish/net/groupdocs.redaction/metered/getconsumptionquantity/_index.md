---
title: "GetConsumptionQuantity"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Hämtar mängden bearbetade MB."
type: docs
weight: 40
url: /sv/net/groupdocs.redaction/metered/getconsumptionquantity/
---
## Metered.GetConsumptionQuantity method

Hämtar mängden bearbetade MB.

```csharp
public static decimal GetConsumptionQuantity()
```

### Returvärde

förbrukningsmängd

### Exempel

Följande exempel visar hur man hämtar mängden MB som har bearbetats.

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);

decimal mbProcessed = Metered.GetConsumptionQuantity();
```

### Se även

* class [Metered](../../metered)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
