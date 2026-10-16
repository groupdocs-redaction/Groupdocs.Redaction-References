---
title: "GetInstance"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Fournit une instance singleton avec la configuration par défaut des formats intégrés."
type: docs
weight: 10
url: /fr/net/groupdocs.redaction.configuration/redactorconfiguration/getinstance/
---
## RedactorConfiguration.GetInstance method

Fournit une instance singleton avec la configuration par défaut des formats intégrés.

```csharp
public static RedactorConfiguration GetInstance()
```

### Valeur de retour

Instance de configuration

### Exemples

L'exemple suivant montre comment ajouter un gestionnaire de format personnalisé.

```csharp
var adobePhotoshopSettings = new DocumentFormatConfiguration();
adobePhotoshopSettings.ExtensionFilter = ".psd";
adobePhotoshopSettings.DocumentType = typeof(MyAdobePhotoshopFormatInstance);
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(adobePhotoshopSettings);
```

### Voir aussi

* class [RedactorConfiguration](../../redactorconfiguration)
* namespace [GroupDocs.Redaction.Configuration](../../../groupdocs.redaction.configuration)
* assembly [GroupDocs.Redaction](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
