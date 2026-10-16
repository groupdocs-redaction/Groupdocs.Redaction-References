---
title: "DocumentFormatInstance"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente un format spécifique d’un document. Implémentez cette classe pour ajouter vos propres types de documents."
type: docs
weight: 110
url: /fr/net/groupdocs.redaction.integration/documentformatinstance/
---
## DocumentFormatInstance class

Représente un format spécifique d’un document. Implémentez cette classe pour ajouter vos propres types de documents.

```csharp
public abstract class DocumentFormatInstance
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Password](../../groupdocs.redaction.integration/documentformatinstance/password) { get; set; } | Obtient ou définit un mot de passe pour les documents protégés par mot de passe. |

## Méthodes

| Nom | Description |
| --- | --- |
| virtual [Initialize](../../groupdocs.redaction.integration/documentformatinstance/initialize)(DocumentFormatConfiguration, RedactorSettings) | Effectue l'initialisation de l'instance du gestionnaire de format de document. |
| [IsRedactionAccepted](../../groupdocs.redaction.integration/documentformatinstance/isredactionaccepted)(RedactionDescription) | Vérifie la présence d'une implémentation de [`IRedactionCallback`](../../groupdocs.redaction.redactions/iredactioncallback) et l'appelle, si spécifiée. |
| virtual [Load](../../groupdocs.redaction.integration/documentformatinstance/load)(Stream) | Charge le document depuis un flux. |
| virtual [PerformBinaryCheck](../../groupdocs.redaction.integration/documentformatinstance/performbinarycheck)(Stream) | Vérifie si le flux fourni contient un document pris en charge par cette instance de format. |
| abstract [Save](../../groupdocs.redaction.integration/documentformatinstance/save)(Stream) | Enregistre le document dans un flux. |

### Remarques

**Learn more**

* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Exemples

L'exemple suivant montre comment créer un stub vide pour un gestionnaire de format personnalisé.

```csharp
public class DummyDocument : DocumentFormatInstance
{     
    public override void Load(Stream output)
    {
        // charger le contenu du fichier
    }

    public override void Save(Stream output)
    {
        // enregistrer les modifications dans le fichier;
    }
}
```

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

// Intégration d'un format personnalisé dans GroupDocs.Redaction
var mySettings = new DocumentFormatConfiguration();
mySettings.ExtensionFilter = ".foo";
mySettings.DocumentType = typeof(MyCustomHandler);
mySettings.InitializationData.Add("MyProperty", "bar");
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(mySettings);
```

### Voir aussi

* namespace [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
