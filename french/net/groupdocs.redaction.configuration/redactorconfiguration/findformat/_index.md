---
title: "FindFormat"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Trouve les configurations de format pour une extension de fichier donnée."
type: docs
weight: 30
url: /fr/net/groupdocs.redaction.configuration/redactorconfiguration/findformat/
---
## RedactorConfiguration.FindFormat method

Trouve les configurations de format pour une extension de fichier donnée.

```csharp
public DocumentFormatConfiguration FindFormat(string fileExtension)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileExtension | String | Extension de fichier, le format est ".ext" |

### Valeur de retour

Si trouvé, instance de [`DocumentFormatConfiguration`](../../documentformatconfiguration), sinon null

### Exemples

L'exemple suivant montre comment obtenir des gestionnaires de format intégrés ou personnalisés.

```csharp
var configuration = RedactorConfiguration.GetInstance();
var formatSettings = configuration.FindFormat(".psd");
```

### Voir aussi

* class [DocumentFormatConfiguration](../../documentformatconfiguration)
* class [RedactorConfiguration](../../redactorconfiguration)
* namespace [GroupDocs.Redaction.Configuration](../../../groupdocs.redaction.configuration)
* assembly [GroupDocs.Redaction](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
