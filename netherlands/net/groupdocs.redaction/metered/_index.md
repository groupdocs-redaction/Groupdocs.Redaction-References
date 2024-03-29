---
title: Metered
second_title: GroupDocs.Redaction voor .NET API-referentie
description: Biedt methoden die het mogelijk maken om het product te activeren met Gemeten licentie en het aantal verwerkte MBs op te halen. Meer informatie over Gemeten licentieshierhttps//purchase.groupdocs.com/faqs/licensing/metered .
type: docs
weight: 270
url: /nl/net/groupdocs.redaction/metered/
---
## Metered class

Biedt methoden die het mogelijk maken om het product te activeren met Gemeten licentie en het aantal verwerkte MB's op te halen. Meer informatie over Gemeten licenties[hier](https://purchase.groupdocs.com/faqs/licensing/metered) .

```csharp
public class Metered
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [Metered](metered)() | Initialiseert een nieuw exemplaar van de klasse Metered. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| [SetMeteredKey](../../groupdocs.redaction/metered/setmeteredkey)(string, string) | Activeert het product met gemeten toetsen. |
| static [GetConsumptionCredit](../../groupdocs.redaction/metered/getconsumptioncredit)() | Krijgt het verbruikstegoed. |
| static [GetConsumptionQuantity](../../groupdocs.redaction/metered/getconsumptionquantity)() | Haalt het aantal verwerkte MB's op. |

### Opmerkingen

**Kom meer te weten**

* Meer over licenties: [Veelgestelde vragen over GroupDocs-licenties](https://purchase.groupdocs.com/faqs/licensing)
* Meer over**GroupDocs. Redactie** licentie: [Evaluatiebeperkingen en licenties](https://docs.groupdocs.com/redaction/net/evaluation-limitations-and-licensing/)

### Voorbeelden

In het volgende voorbeeld ziet u hoe u het product kunt activeren met gedoseerde sleutels.

```csharp
[C#]

Metered matered = new Metered();
matered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim matered As Metered = New Metered
matered.SetMeteredKey("PublicKey", "PrivateKey")
```

het component jar-bestand:

```csharp
Metered matered = new Metered();
matered.setMeteredKey("PublicKey", "PrivateKey");
```

### Zie ook

* naamruimte [GroupDocs.Redaction](../../groupdocs.redaction)
* montage [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
