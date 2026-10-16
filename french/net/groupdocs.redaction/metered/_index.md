---
title: "Mesuré"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Fournit des méthodes qui permettent d'activer le produit avec une licence Mesurée et de récupérer la quantité de Mo traités. En savoir plus sur les licences Mesurées icihttps//purchase.groupdocs.com/faqs/licensing/metered."
type: docs
weight: 280
url: /fr/net/groupdocs.redaction/metered/
---
## Metered class

Fournit des méthodes qui permettent d'activer le produit avec une licence à la consommation et de récupérer la quantité de Mo traités. En savoir plus sur les licences à la consommation [ici](https://purchase.groupdocs.com/faqs/licensing/metered).

```csharp
public class Metered
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Metered](metered)() | Initialise une nouvelle instance de la classe Metered. |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetMeteredKey](../../groupdocs.redaction/metered/setmeteredkey)(string, string) | Active le produit avec des clés Mesurées. |
| static [GetConsumptionCredit](../../groupdocs.redaction/metered/getconsumptioncredit)() | Obtient le crédit de consommation. |
| static [GetConsumptionQuantity](../../groupdocs.redaction/metered/getconsumptionquantity)() | Récupère la quantité de Mo traités. |

### Remarques

**Learn more**

* More about licensing: [GroupDocs Licensing FAQ](https://purchase.groupdocs.com/faqs/licensing)
* More about **GroupDocs.Redaction** licensing: [Evaluation Limitations and Licensing](https://docs.groupdocs.com/redaction/net/evaluation-limitations-and-licensing/)

### Exemples

L'exemple suivant montre comment activer le produit avec des clés Mesurées.

```csharp
[C#]

Metered matered = new Metered();
matered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim matered As Metered = New Metered
matered.SetMeteredKey("PublicKey", "PrivateKey")
```

le fichier jar du composant :

```csharp
Metered matered = new Metered();
matered.setMeteredKey("PublicKey", "PrivateKey");
```

### Voir aussi

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
