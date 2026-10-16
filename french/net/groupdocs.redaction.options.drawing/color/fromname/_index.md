---
title: "FromName"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Crée une couleur à partir du nom spécifié d’une couleur connue. Si le nom n’est pas un nom de couleur connu, une exception est levée."
type: docs
weight: 1440
url: /fr/net/groupdocs.redaction.options.drawing/color/fromname/
---
## Color.FromName method

Crée une couleur à partir du nom spécifié d’une couleur connue. Si *name* n’est pas un nom de couleur connu, une exception est levée.

```csharp
public static Color FromName(string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom d’une couleur connue, comme `Red` ou `Black`. |

### Valeur de retour

La couleur nommée.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *name* est `null`. |
| ArgumentException | *name* n'est pas un nom de couleur connu. |

### Voir aussi

* struct [Color](../../color)
* namespace [GroupDocs.Redaction.Options.Drawing](../../../groupdocs.redaction.options.drawing)
* assembly [GroupDocs.Redaction](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
