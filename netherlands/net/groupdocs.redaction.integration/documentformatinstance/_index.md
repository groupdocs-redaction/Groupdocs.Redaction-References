---
title: "DocumentFormatInstance"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Stelt een specifiek documentformaat voor. Implementeer deze klasse om uw eigen documenttypen toe te voegen."
type: docs
weight: 110
url: /nl/net/groupdocs.redaction.integration/documentformatinstance/
---
## DocumentFormatInstance class

Stelt een specifiek documentformaat voor. Implementeer deze klasse om uw eigen documenttypen toe te voegen.

```csharp
public abstract class DocumentFormatInstance
```

## Properties

| Naam | Beschrijving |
| --- | --- |
| [Password](../../groupdocs.redaction.integration/documentformatinstance/password) { get; set; } | Haalt een wachtwoord op of stelt een wachtwoord in voor wachtwoordbeveiligde documenten. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| virtual [Initialize](../../groupdocs.redaction.integration/documentformatinstance/initialize)(DocumentFormatConfiguration, RedactorSettings) | Voert initialisatie uit van de instantie van de documentformaat‑handler. |
| [IsRedactionAccepted](../../groupdocs.redaction.integration/documentformatinstance/isredactionaccepted)(RedactionDescription) | Controleert op implementatie van [`IRedactionCallback`](../../groupdocs.redaction.redactions/iredactioncallback) en roept deze aan, indien gespecificeerd. |
| virtual [Load](../../groupdocs.redaction.integration/documentformatinstance/load)(Stream) | Laadt het document vanuit een stream. |
| virtual [PerformBinaryCheck](../../groupdocs.redaction.integration/documentformatinstance/performbinarycheck)(Stream) | Controleert of de gegeven stream een document bevat dat door deze formaat‑instantie wordt ondersteund. |
| abstract [Save](../../groupdocs.redaction.integration/documentformatinstance/save)(Stream) | Slaat het document op in een stream. |

### Opmerkingen

**Learn more**

* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Voorbeelden

Het volgende voorbeeld laat zien hoe je een lege stub maakt voor een aangepaste formaat‑handler.

```csharp
public class DummyDocument : DocumentFormatInstance
{     
    public override void Load(Stream output)
    {
        // laad bestandsinhoud
    }

    public override void Save(Stream output)
    {
        // sla wijzigingen op in bestand;
    }
}
```

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

* namespace [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
