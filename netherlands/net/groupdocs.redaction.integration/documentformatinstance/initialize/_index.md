---
title: "Initialiseren"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Voert initialisatie uit van de instantie van de documentformaat‑handler."
type: docs
weight: 20
url: /nl/net/groupdocs.redaction.integration/documentformatinstance/initialize/
---
## DocumentFormatInstance.Initialize method

Voert initialisatie uit van de instantie van de documentformaat‑handler.

```csharp
public virtual void Initialize(DocumentFormatConfiguration config, RedactorSettings settings)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| config | DocumentFormatConfiguration | Formaatconfiguratie |
| instellingen | RedactorSettings | Standaardinstellingen voor het redactieproces. |

### Voorbeelden

Het volgende voorbeeld laat zien hoe je de initialisatiegegevens gebruikt.

```csharp
public class MyCustomHandler : DocumentFormatInstance
{
    private string MyProperty { get; set; }
    
    // Andere aangepaste code 
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

// Aansluiten van aangepast formaat in GroupDocs.Redaction
var mySettings = new DocumentFormatConfiguration();
mySettings.ExtensionFilter = ".foo";
mySettings.DocumentType = typeof(MyCustomHandler);
mySettings.InitializationData.Add("MyProperty", "bar");
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(mySettings);
```

### Zie ook

* class [DocumentFormatConfiguration](../../../groupdocs.redaction.configuration/documentformatconfiguration)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [DocumentFormatInstance](../../documentformatinstance)
* namespace [GroupDocs.Redaction.Integration](../../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
