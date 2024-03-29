---
title: Metered
second_title: Riferimento API GroupDocs.Redaction per .NET
description: Fornisce metodi che consentono di attivare il prodotto con licenza a consumo e recuperare la quantità di MB elaborati. Ulteriori informazioni sulle licenze a consumoQuihttps//purchase.groupdocs.com/faqs/licensing/metered .
type: docs
weight: 270
url: /it/net/groupdocs.redaction/metered/
---
## Metered class

Fornisce metodi che consentono di attivare il prodotto con licenza a consumo e recuperare la quantità di MB elaborati. Ulteriori informazioni sulle licenze a consumo[Qui](https://purchase.groupdocs.com/faqs/licensing/metered) .

```csharp
public class Metered
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Metered](metered)() | Inizializza una nuova istanza della classe misurata. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetMeteredKey](../../groupdocs.redaction/metered/setmeteredkey)(string, string) | Attiva il prodotto con chiavi a consumo. |
| static [GetConsumptionCredit](../../groupdocs.redaction/metered/getconsumptioncredit)() | Ottiene il credito di consumo. |
| static [GetConsumptionQuantity](../../groupdocs.redaction/metered/getconsumptionquantity)() | Recupera la quantità di MB elaborati. |

### Osservazioni

**Saperne di più**

* Ulteriori informazioni sulla licenza: [Domande frequenti sulle licenze di GroupDocs](https://purchase.groupdocs.com/faqs/licensing)
* Ulteriori informazioni**GroupDocs.Redazione** licenza: [Limiti di valutazione e licenza](https://docs.groupdocs.com/redaction/net/evaluation-limitations-and-licensing/)

### Esempi

L'esempio seguente mostra come attivare il prodotto con le chiavi a consumo.

```csharp
[C#]

Metered matered = new Metered();
matered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim matered As Metered = New Metered
matered.SetMeteredKey("PublicKey", "PrivateKey")
```

il file jar del componente:

```csharp
Metered matered = new Metered();
matered.setMeteredKey("PublicKey", "PrivateKey");
```

### Guarda anche

* spazio dei nomi [GroupDocs.Redaction](../../groupdocs.redaction)
* assemblea [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
