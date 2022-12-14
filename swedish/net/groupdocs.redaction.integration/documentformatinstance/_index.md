---
title: DocumentFormatInstance
second_title: GroupDocs.Redaction för .NET API-referens
description: Representerar ett specifikt format för ett dokument. Implementera den här klassen för att lägga till dina egna dokumenttyper.
type: docs
weight: 110
url: /sv/net/groupdocs.redaction.integration/documentformatinstance/
---
## DocumentFormatInstance class

Representerar ett specifikt format för ett dokument. Implementera den här klassen för att lägga till dina egna dokumenttyper.

```csharp
public abstract class DocumentFormatInstance
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Password](../../groupdocs.redaction.integration/documentformatinstance/password) { get; set; } | Hämtar eller ställer in ett lösenord för lösenordsskyddade dokument. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| virtual [Initialize](../../groupdocs.redaction.integration/documentformatinstance/initialize)(DocumentFormatConfiguration, RedactorSettings) | Utför initiering av instansen av dokumentformathanterare. |
| [IsRedactionAccepted](../../groupdocs.redaction.integration/documentformatinstance/isredactionaccepted)(RedactionDescription) | Söker efter[`IRedactionCallback`](../../groupdocs.redaction.redactions/iredactioncallback) implementering och anropar den, om specificerad. |
| virtual [Load](../../groupdocs.redaction.integration/documentformatinstance/load)(Stream) | Laddar dokumentet från en ström. |
| virtual [PerformBinaryCheck](../../groupdocs.redaction.integration/documentformatinstance/performbinarycheck)(Stream) | Kontrollerar om den givna strömmen innehåller ett dokument som stöds av denna formatinstans. |
| abstract [Save](../../groupdocs.redaction.integration/documentformatinstance/save)(Stream) | Sparar dokumentet i en ström. |

### Anmärkningar

**Läs mer**

* Mer information om att implementera anpassade format: [Skapa anpassad formathanterare](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Exempel

Följande exempel visar hur man skapar en tom stubb för en anpassad formathanterare.

Följande exempel visar hur man använder initialiseringsdata.

```csharp
public class DummyDocument : DocumentFormatInstance
{     
    public override void Load(Stream output)
    {
        // ladda filinnehåll
    }

    public override void Save(Stream output)
    {
        // spara ändringar i filen;
    }
}
```

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

// Ansluter anpassat format till GroupDocs.Redaction
var mySettings = new DocumentFormatConfiguration();
mySettings.ExtensionFilter = ".foo";
mySettings.DocumentType = typeof(MyCustomHandler);
mySettings.InitializationData.Add("MyProperty", "bar");
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(mySettings);
```

### Se även

* namnutrymme [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* hopsättning [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
