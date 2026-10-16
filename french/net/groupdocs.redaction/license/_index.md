---
title: "License"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Fournit des méthodes pour appliquer une licence."
type: docs
weight: 270
url: /fr/net/groupdocs.redaction/license/
---
## License class

Fournit des méthodes pour appliquer une licence.

```csharp
public class License
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [License](license)() | Initialise une instance de la classe License. |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetLicense](../../groupdocs.redaction/license/setlicense#setlicense)(Stream) | Définit la licence GroupDocs.Redaction à partir d’un flux. |
| [SetLicense](../../groupdocs.redaction/license/setlicense#setlicense_1)(string) | Définit la licence GroupDocs.Redaction à partir d’un chemin de fichier. |

### Remarques

**Learn more**

* More about licensing: [GroupDocs Licensing FAQ](https://purchase.groupdocs.com/faqs/licensing)
* More about **GroupDocs.Redaction** licensing: [Evaluation Limitations and Licensing](https://docs.groupdocs.com/redaction/net/evaluation-limitations-and-licensing/)

### Exemples

L’exemple suivant montre comment définir la licence pour GroupDocs.Redaction.

```csharp
GroupDocs.Redaction.License license = new GroupDocs.Redaction.License();
// En alternative, vous pouvez utiliser un flux:
license.SetLicense(licensePath);
```

### Voir aussi

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
