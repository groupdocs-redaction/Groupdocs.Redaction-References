---
title: "Måttbaserad"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Tillhandahåller metoder som möjliggör att aktivera produkten med en Metered‑licens och hämta mängden MB som bearbetats. Läs mer om Metered‑licenser här https//purchase.groupdocs.com/faqs/licensing/metered."
type: docs
weight: 280
url: /sv/net/groupdocs.redaction/metered/
---
## Metered class

Tillhandahåller metoder som möjliggör att aktivera produkten med en Metered-licens och hämta mängden MB som bearbetats. Läs mer om Metered-licenser [här](https://purchase.groupdocs.com/faqs/licensing/metered).

```csharp
public class Metered
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [Metered](metered)() | Initierar en ny instans av Metered‑klassen. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [SetMeteredKey](../../groupdocs.redaction/metered/setmeteredkey)(string, string) | Aktiverar produkten med Metered‑nycklar. |
| static [GetConsumptionCredit](../../groupdocs.redaction/metered/getconsumptioncredit)() | Hämtar konsumtionskrediten. |
| static [GetConsumptionQuantity](../../groupdocs.redaction/metered/getconsumptionquantity)() | Hämtar mängden bearbetade MB. |

### Anmärkningar

**Learn more**

* More about licensing: [GroupDocs Licensing FAQ](https://purchase.groupdocs.com/faqs/licensing)
* More about **GroupDocs.Redaction** licensing: [Evaluation Limitations and Licensing](https://docs.groupdocs.com/redaction/net/evaluation-limitations-and-licensing/)

### Exempel

Följande exempel visar hur man aktiverar produkten med Metered‑nycklar.

```csharp
[C#]

Metered matered = new Metered();
matered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim matered As Metered = New Metered
matered.SetMeteredKey("PublicKey", "PrivateKey")
```

komponent‑jar‑filen:

```csharp
Metered matered = new Metered();
matered.setMeteredKey("PublicKey", "PrivateKey");
```

### Se även

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
