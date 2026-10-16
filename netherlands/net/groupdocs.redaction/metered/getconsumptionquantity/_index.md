---
title: "GetConsumptionQuantity"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Haalt de hoeveelheid verwerkte MB's op."
type: docs
weight: 40
url: /nl/net/groupdocs.redaction/metered/getconsumptionquantity/
---
## Metered.GetConsumptionQuantity method

Haalt de hoeveelheid verwerkte MB's op.

```csharp
public static decimal GetConsumptionQuantity()
```

### Retourwaarde

verbruikshoeveelheid

### Voorbeelden

Het volgende voorbeeld toont hoe de hoeveelheid verwerkte MB's op te halen.

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);

decimal mbProcessed = Metered.GetConsumptionQuantity();
```

### Zie ook

* class [Metered](../../metered)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
