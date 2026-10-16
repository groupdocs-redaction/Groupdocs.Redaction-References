---
title: "Metered"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Biedt methoden die het mogelijk maken het product te activeren met een Metered-licentie en de hoeveelheid verwerkte MB's op te halen. Meer informatie over Metered-licenties vindt u hierhttps//purchase.groupdocs.com/faqs/licensing/metered."
type: docs
weight: 280
url: /nl/net/groupdocs.redaction/metered/
---
## Metered class

Biedt methoden waarmee het product kan worden geactiveerd met een Metered-licentie en het aantal verwerkte MB's kan worden opgehaald. Meer informatie over Metered-licenties [hier](https://purchase.groupdocs.com/faqs/licensing/metered).

```csharp
public class Metered
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [Metered](metered)() | Initialiseert een nieuwe instantie van de Metered-klasse. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [SetMeteredKey](../../groupdocs.redaction/metered/setmeteredkey)(string, string) | Activeert het product met Metered-sleutels. |
| static [GetConsumptionCredit](../../groupdocs.redaction/metered/getconsumptioncredit)() | Haalt het consumptiekrediet op. |
| static [GetConsumptionQuantity](../../groupdocs.redaction/metered/getconsumptionquantity)() | Haalt de hoeveelheid verwerkte MB's op. |

### Opmerkingen

**Learn more**

* More about licensing: [GroupDocs Licensing FAQ](https://purchase.groupdocs.com/faqs/licensing)
* More about **GroupDocs.Redaction** licensing: [Evaluation Limitations and Licensing](https://docs.groupdocs.com/redaction/net/evaluation-limitations-and-licensing/)

### Voorbeelden

Het volgende voorbeeld toont hoe het product te activeren met Metered-sleutels.

```csharp
[C#]

Metered matered = new Metered();
matered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim matered As Metered = New Metered
matered.SetMeteredKey("PublicKey", "PrivateKey")
```

het component‑jar‑bestand:

```csharp
Metered matered = new Metered();
matered.setMeteredKey("PublicKey", "PrivateKey");
```

### Zie ook

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
