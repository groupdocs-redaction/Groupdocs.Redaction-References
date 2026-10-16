---
title: "A consumo"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Fornisce metodi che consentono di attivare il prodotto con licenza a consumo e recuperare la quantità di MB elaborati. Scopri di più sulle licenze a consumo qui https//purchase.groupdocs.com/faqs/licensing/metered."
type: docs
weight: 280
url: /it/net/groupdocs.redaction/metered/
---
## Metered class

Fornisce metodi che consentono di attivare il prodotto con licenza a consumo e recuperare la quantità di MB elaborati. Scopri di più sulle licenze a consumo [qui](https://purchase.groupdocs.com/faqs/licensing/metered).

```csharp
public class Metered
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Metered](metered)() | Inizializza una nuova istanza della classe Metered. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetMeteredKey](../../groupdocs.redaction/metered/setmeteredkey)(string, string) | Attiva il prodotto con chiavi a consumo. |
| static [GetConsumptionCredit](../../groupdocs.redaction/metered/getconsumptioncredit)() | Ottiene il credito di consumo. |
| static [GetConsumptionQuantity](../../groupdocs.redaction/metered/getconsumptionquantity)() | Recupera la quantità di MB elaborati. |

### Osservazioni

**Learn more**

* More about licensing: [GroupDocs Licensing FAQ](https://purchase.groupdocs.com/faqs/licensing)
* More about **GroupDocs.Redaction** licensing: [Evaluation Limitations and Licensing](https://docs.groupdocs.com/redaction/net/evaluation-limitations-and-licensing/)

### Esempi

Il seguente esempio dimostra come attivare il prodotto con chiavi a consumo.

```csharp
[C#]

Metered matered = new Metered();
matered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim matered As Metered = New Metered
matered.SetMeteredKey("PublicKey", "PrivateKey")
```

il file JAR del componente:

```csharp
Metered matered = new Metered();
matered.setMeteredKey("PublicKey", "PrivateKey");
```

### Vedi anche

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
