---
title: "GetConsumptionQuantity"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Recupera la quantità di MB elaborati."
type: docs
weight: 40
url: /it/net/groupdocs.redaction/metered/getconsumptionquantity/
---
## Metered.GetConsumptionQuantity method

Recupera la quantità di MB elaborati.

```csharp
public static decimal GetConsumptionQuantity()
```

### Valore di ritorno

quantità di consumo

### Esempi

Il seguente esempio dimostra come recuperare la quantità di MB elaborati.

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);

decimal mbProcessed = Metered.GetConsumptionQuantity();
```

### Vedi anche

* class [Metered](../../metered)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
