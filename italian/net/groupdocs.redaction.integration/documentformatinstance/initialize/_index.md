---
title: "Inizializza"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Esegue l'inizializzazione dell'istanza del gestore del formato documento."
type: docs
weight: 20
url: /it/net/groupdocs.redaction.integration/documentformatinstance/initialize/
---
## DocumentFormatInstance.Initialize method

Esegue l'inizializzazione dell'istanza del gestore del formato documento.

```csharp
public virtual void Initialize(DocumentFormatConfiguration config, RedactorSettings settings)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| config | DocumentFormatConfiguration | Configurazione del formato |
| impostazioni | RedactorSettings | Impostazioni predefinite per il processo di redazione. |

### Esempi

Il seguente esempio dimostra come utilizzare i dati di inizializzazione.

```csharp
public class MyCustomHandler : DocumentFormatInstance
{
    private string MyProperty { get; set; }
    
    // Altro codice personalizzato 
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

// Integrazione del formato personalizzato in GroupDocs.Redaction
var mySettings = new DocumentFormatConfiguration();
mySettings.ExtensionFilter = ".foo";
mySettings.DocumentType = typeof(MyCustomHandler);
mySettings.InitializationData.Add("MyProperty", "bar");
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(mySettings);
```

### Vedi anche

* class [DocumentFormatConfiguration](../../../groupdocs.redaction.configuration/documentformatconfiguration)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [DocumentFormatInstance](../../documentformatinstance)
* namespace [GroupDocs.Redaction.Integration](../../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
