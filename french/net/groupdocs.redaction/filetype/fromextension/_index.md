---
title: "FromExtension"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Mappe l'extension de fichier au type de fichier."
type: docs
weight: 500
url: /fr/net/groupdocs.redaction/filetype/fromextension/
---
## FileType.FromExtension method

Mappe l'extension de fichier au type de fichier.

```csharp
public static FileType FromExtension(string extension)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| extension | String | Extension de fichier (y compris le point "."). |

### Valeur de retour

Lorsque le type de fichier est pris en charge, le renvoie ; sinon, renvoie le type de fichier [`Unknown`](../unknown) par défaut.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Lancée lorsque *extension* est nulle ou une chaîne vide. |

### Voir aussi

* class [FileType](../../filetype)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
