---
title: "DocumentFormatInstance"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar ett specifikt format för ett dokument. Implementera denna klass för att lägga till egna dokumenttyper."
type: docs
weight: 110
url: /sv/net/groupdocs.redaction.integration/documentformatinstance/
---
## DocumentFormatInstance class

Representerar ett specifikt format för ett dokument. Implementera denna klass för att lägga till egna dokumenttyper.

```csharp
public abstract class DocumentFormatInstance
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Password](../../groupdocs.redaction.integration/documentformatinstance/password) { get; set; } | Hämtar eller anger ett lösenord för lösenordsskyddade dokument. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| virtual [Initialize](../../groupdocs.redaction.integration/documentformatinstance/initialize)(DocumentFormatConfiguration, RedactorSettings) | Utför initiering av instansen av dokumentformatshanteraren. |
| [IsRedactionAccepted](../../groupdocs.redaction.integration/documentformatinstance/isredactionaccepted)(RedactionDescription) | Kontrollerar om en implementation av [`IRedactionCallback`](../../groupdocs.redaction.redactions/iredactioncallback) finns och anropar den, om den är specificerad. |
| virtual [Load](../../groupdocs.redaction.integration/documentformatinstance/load)(Stream) | Läser in dokumentet från en ström. |
| virtual [PerformBinaryCheck](../../groupdocs.redaction.integration/documentformatinstance/performbinarycheck)(Stream) | Kontrollerar om den angivna strömmen innehåller ett dokument som stöds av denna formatinstans. |
| abstract [Save](../../groupdocs.redaction.integration/documentformatinstance/save)(Stream) | Sparar dokumentet till en ström. |

### Anmärkningar

**Learn more**

* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Exempel

Följande exempel visar hur man skapar en tom stub för en anpassad formatshanterare.

```csharp
public class DummyDocument : DocumentFormatInstance
{     
    public override void Load(Stream output)
    {
        // läs in filinnehåll
    }

    public override void Save(Stream output)
    {
        // spara ändringar till fil;
    }
}
```

Följande exempel visar hur man använder initieringsdata.

```csharp
public class MyCustomHandler : DocumentFormatInstance
{
    private string MyProperty { get; set; }
    
    // Annan anpassad kod 
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

// Integrera anpassat format i GroupDocs.Redaction
var mySettings = new DocumentFormatConfiguration();
mySettings.ExtensionFilter = ".foo";
mySettings.DocumentType = typeof(MyCustomHandler);
mySettings.InitializationData.Add("MyProperty", "bar");
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(mySettings);
```

### Se även

* namespace [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
