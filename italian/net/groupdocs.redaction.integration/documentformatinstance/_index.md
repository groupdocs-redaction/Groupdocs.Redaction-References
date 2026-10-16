---
title: "DocumentFormatInstance"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta un formato specifico di un documento. Implementa questa classe per aggiungere i tuoi tipi di documento."
type: docs
weight: 110
url: /it/net/groupdocs.redaction.integration/documentformatinstance/
---
## DocumentFormatInstance class

Rappresenta un formato specifico di un documento. Implementa questa classe per aggiungere i tuoi tipi di documento.

```csharp
public abstract class DocumentFormatInstance
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Password](../../groupdocs.redaction.integration/documentformatinstance/password) { get; set; } | Ottiene o imposta una password per i documenti protetti da password. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [Initialize](../../groupdocs.redaction.integration/documentformatinstance/initialize)(DocumentFormatConfiguration, RedactorSettings) | Esegue l'inizializzazione dell'istanza del gestore del formato documento. |
| [IsRedactionAccepted](../../groupdocs.redaction.integration/documentformatinstance/isredactionaccepted)(RedactionDescription) | Verifica l'implementazione di [`IRedactionCallback`](../../groupdocs.redaction.redactions/iredactioncallback) e la invoca, se specificata. |
| virtual [Load](../../groupdocs.redaction.integration/documentformatinstance/load)(Stream) | Carica il documento da uno stream. |
| virtual [PerformBinaryCheck](../../groupdocs.redaction.integration/documentformatinstance/performbinarycheck)(Stream) | Verifica se lo stream fornito contiene un documento supportato da questa istanza di formato. |
| abstract [Save](../../groupdocs.redaction.integration/documentformatinstance/save)(Stream) | Salva il documento su uno stream. |

### Osservazioni

**Learn more**

* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Esempi

Il seguente esempio dimostra come creare un stub vuoto per un gestore di formato personalizzato.

```csharp
public class DummyDocument : DocumentFormatInstance
{     
    public override void Load(Stream output)
    {
        // carica contenuto del file
    }

    public override void Save(Stream output)
    {
        // salva le modifiche al file;
    }
}
```

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

* namespace [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
