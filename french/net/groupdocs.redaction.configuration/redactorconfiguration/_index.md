---
title: "RedactorConfiguration"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Fournit l'accès à une liste de formats pris en charge intégrés et de formats utilisateur personnalisés."
type: docs
weight: 20
url: /fr/net/groupdocs.redaction.configuration/redactorconfiguration/
---
## RedactorConfiguration class

Fournit l'accès à une liste de formats pris en charge, intégrés et personnalisés par l'utilisateur.

```csharp
public class RedactorConfiguration
```

## Propriétés

| Nom | Description |
| --- | --- |
| [AvailableFormats](../../groupdocs.redaction.configuration/redactorconfiguration/availableformats) { get; } | Obtient une liste des formats reconnus, voir [`DocumentFormatConfiguration`](../documentformatconfiguration). |

## Méthodes

| Nom | Description |
| --- | --- |
| static [GetInstance](../../groupdocs.redaction.configuration/redactorconfiguration/getinstance)() | Fournit une instance singleton avec la configuration par défaut des formats intégrés. |
| [FindFormat](../../groupdocs.redaction.configuration/redactorconfiguration/findformat)(string) | Trouve les configurations de format pour une extension de fichier donnée. |

### Remarques

**Learn more**

* More details about **GroupDocs.Redaction** configuration: [Extend supported extensions list](https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/)
* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Exemples

L'exemple suivant montre comment ajouter un gestionnaire de format utilisateur personnalisé.

```csharp
var adobePhotoshopSettings = new DocumentFormatConfiguration();
adobePhotoshopSettings.ExtensionFilter = ".psd";
adobePhotoshopSettings.DocumentType = typeof(MyAdobePhotoshopFormatInstance);
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(adobePhotoshopSettings);
```

L'exemple suivant montre comment obtenir des gestionnaires de format intégrés ou personnalisés.

```csharp
var configuration = RedactorConfiguration.GetInstance();
var formatSettings = configuration.FindFormat(".psd");
```

### Voir aussi

* namespace [GroupDocs.Redaction.Configuration](../../groupdocs.redaction.configuration)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
