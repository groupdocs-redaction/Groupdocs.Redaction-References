---
title: Initialize
second_title: Référence de l'API GroupDocs.Redaction pour .NET
description: Effectue linitialisation de linstance du gestionnaire de format de document.
type: docs
weight: 20
url: /fr/net/groupdocs.redaction.integration/documentformatinstance/initialize/
---
## DocumentFormatInstance.Initialize method

Effectue l'initialisation de l'instance du gestionnaire de format de document.

```csharp
public virtual void Initialize(DocumentFormatConfiguration config, RedactorSettings settings)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| config | DocumentFormatConfiguration | Paramétrage des formats |
| settings | RedactorSettings | Paramètres par défaut pour le processus de rédaction. |

### Exemples

L'exemple suivant montre comment utiliser les données d'initialisation.

```csharp
public class MyCustomHandler : DocumentFormatInstance
{
    private string MyProperty { get; set; }
    
    // Autre code personnalisé 
    ...

    public override void Initialize(DocumentFormatConfiguration config)
    {
        base.Initialize(config);
        if (config.InitializationData.ContainsKey("MyProperty"))
        {
            MyProperty = config.InitializationData["MyProperty"];
        }
    }
}

// Insertion d'un format personnalisé dans GroupDocs.Redaction
var mySettings = new DocumentFormatConfiguration();
mySettings.ExtensionFilter = ".foo";
mySettings.DocumentType = typeof(MyCustomHandler);
mySettings.InitializationData.Add("MyProperty", "bar");
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(mySettings);
```

### Voir également

* class [DocumentFormatConfiguration](../../../groupdocs.redaction.configuration/documentformatconfiguration)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [DocumentFormatInstance](../../documentformatinstance)
* espace de noms [GroupDocs.Redaction.Integration](../../documentformatinstance)
* Assemblée [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
