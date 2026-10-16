---
title: "LoadOptions"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Fournit des options qui seront utilisées pour ouvrir un fichier."
type: docs
weight: 380
url: /fr/net/groupdocs.redaction.options/loadoptions/
---
## LoadOptions class

Fournit des options qui seront utilisées pour ouvrir un fichier.

```csharp
public class LoadOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [LoadOptions](loadoptions#constructor)() | Initialise une nouvelle instance de la classe LoadOptions. |
| [LoadOptions](loadoptions#constructor_1)(bool) | Initialise une nouvelle instance de la classe LoadOptions avec le drapeau de pré-rasterisation spécifié. |
| [LoadOptions](loadoptions#constructor_2)(FileType) | Initialise une nouvelle instance de la classe LoadOptions avec le type de fichier spécifié. |
| [LoadOptions](loadoptions#constructor_3)(string) | Initialise une nouvelle instance de la classe LoadOptions avec le mot de passe spécifié. |
| [LoadOptions](loadoptions#constructor_4)(string, bool) | Initialise une nouvelle instance de la classe LoadOptions avec le mot de passe spécifié. |

## Propriétés

| Nom | Description |
| --- | --- |
| [FileType](../../groupdocs.redaction.options/loadoptions/filetype) { get; set; } | Obtient ou définit le type de fichier à ouvrir. |
| [Password](../../groupdocs.redaction.options/loadoptions/password) { get; set; } | Obtient ou définit un mot de passe pour les documents protégés par mot de passe. |
| [PreRasterize](../../groupdocs.redaction.options/loadoptions/prerasterize) { get; set; } | Obtient ou définit une valeur indiquant si le fichier doit être pré-rasterisé. |

### Remarques

**Learn more**

* [Loading documents](https://docs.groupdocs.com/redaction/net/loading-documents/)
* [Load from local disk](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
* [Load from stream](https://docs.groupdocs.com/redaction/net/load-from-stream/)
* [Load password-protected document](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

### Exemples

L'exemple suivant montre comment ouvrir un document protégé par mot de passe.

```csharp
LoadOptions loadOptions = new LoadOptions("mysecretpassword");
using (var redactor = new Redactor("PasswordProtected.pdf", loadOptions))
{
    // travailler avec le document
}
```

### Voir aussi

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
