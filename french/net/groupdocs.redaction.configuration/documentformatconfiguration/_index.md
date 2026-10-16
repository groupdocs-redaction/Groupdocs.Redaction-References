---
title: "DocumentFormatConfiguration"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente une référence de type pour la classe DocumentFormatInstance../groupdocs.redaction.integration/documentformatinstancederived et la liste des extensions de fichiers prises en charge pour une détection de format plus rapide."
type: docs
weight: 10
url: /fr/net/groupdocs.redaction.configuration/documentformatconfiguration/
---
## DocumentFormatConfiguration class

Représente une référence de type pour la classe dérivée de [`DocumentFormatInstance`](../../groupdocs.redaction.integration/documentformatinstance) et la liste des extensions de fichiers prises en charge pour une détection de format plus rapide.

```csharp
public class DocumentFormatConfiguration
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [DocumentFormatConfiguration](documentformatconfiguration)() | Initialise une nouvelle instance de la classe DocumentFormatConfiguration. |

## Propriétés

| Nom | Description |
| --- | --- |
| [DocumentType](../../groupdocs.redaction.configuration/documentformatconfiguration/documenttype) { get; set; } | Obtient ou définit le type d'une classe, héritant de [`DocumentFormatInstance`](../../groupdocs.redaction.integration/documentformatinstance). |
| [ExtensionFilter](../../groupdocs.redaction.configuration/documentformatconfiguration/extensionfilter) { get; set; } | Obtient ou définit une liste d'extensions de fichiers séparées par des virgules (",") (par exemple ".pdf"), insensible à la casse. |
| [InitializationData](../../groupdocs.redaction.configuration/documentformatconfiguration/initializationdata) { get; set; } | Obtient ou définit les données requises pour l'initialisation de [`DocumentFormatInstance`](../../groupdocs.redaction.integration/documentformatinstance). |

## Méthodes

| Nom | Description |
| --- | --- |
| [SupportsExtension](../../groupdocs.redaction.configuration/documentformatconfiguration/supportsextension)(string) | Vérifie si une extension de fichier donnée peut être traitée comme DocumentType. |

### Remarques

**Learn more**

* More details about **GroupDocs.Redaction** configuration: [Extend supported extensions list](https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/)
* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Exemples

L'exemple suivant montre comment définir les propriétés d'une configuration de format personnalisée.

```csharp
var adobePhotoshopSettings = new DocumentFormatConfiguration();
adobePhotoshopSettings.ExtensionFilter = ".psd";
adobePhotoshopSettings.DocumentType = typeof(MyAdobePhotoshopFormatInstance);
```

### Voir aussi

* namespace [GroupDocs.Redaction.Configuration](../../groupdocs.redaction.configuration)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
