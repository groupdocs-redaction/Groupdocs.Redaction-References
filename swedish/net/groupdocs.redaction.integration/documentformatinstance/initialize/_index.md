---
title: "Initialize"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Utför initiering av instansen av dokumentformatshanteraren."
type: docs
weight: 20
url: /sv/net/groupdocs.redaction.integration/documentformatinstance/initialize/
---
## DocumentFormatInstance.Initialize method

Utför initiering av instansen av dokumentformatshanteraren.

```csharp
public virtual void Initialize(DocumentFormatConfiguration config, RedactorSettings settings)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| config | DocumentFormatConfiguration | Formatkonfiguration |
| settings | RedactorSettings | Standardinställningar för raderingsprocessen. |

### Exempel

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

* class [DocumentFormatConfiguration](../../../groupdocs.redaction.configuration/documentformatconfiguration)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [DocumentFormatInstance](../../documentformatinstance)
* namespace [GroupDocs.Redaction.Integration](../../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
