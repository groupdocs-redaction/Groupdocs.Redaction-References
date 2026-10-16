---
title: "DocumentFormatConfiguration"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta un riferimento di tipo per la classe DocumentFormatInstance../groupdocs.redaction.integration/documentformatinstancederived e l'elenco delle estensioni di file supportate per una rilevazione del formato più rapida."
type: docs
weight: 10
url: /it/net/groupdocs.redaction.configuration/documentformatconfiguration/
---
## DocumentFormatConfiguration class

Rappresenta un riferimento di tipo per la classe derivata da [`DocumentFormatInstance`](../../groupdocs.redaction.integration/documentformatinstance) e l'elenco delle estensioni di file supportate per una rilevazione del formato più rapida.

```csharp
public class DocumentFormatConfiguration
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [DocumentFormatConfiguration](documentformatconfiguration)() | Inizializza una nuova istanza della classe DocumentFormatConfiguration. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DocumentType](../../groupdocs.redaction.configuration/documentformatconfiguration/documenttype) { get; set; } | Ottiene o imposta il tipo di una classe, ereditando da [`DocumentFormatInstance`](../../groupdocs.redaction.integration/documentformatinstance). |
| [ExtensionFilter](../../groupdocs.redaction.configuration/documentformatconfiguration/extensionfilter) { get; set; } | Ottiene o imposta un elenco delimitato da virgole (\",\") di estensioni di file (ad esempio \".pdf\"), senza distinzione tra maiuscole e minuscole. |
| [InitializationData](../../groupdocs.redaction.configuration/documentformatconfiguration/initializationdata) { get; set; } | Ottiene o imposta i dati, richiesti per l'inizializzazione di [`DocumentFormatInstance`](../../groupdocs.redaction.integration/documentformatinstance). |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SupportsExtension](../../groupdocs.redaction.configuration/documentformatconfiguration/supportsextension)(string) | Verifica se una determinata estensione di file può essere gestita come DocumentType. |

### Osservazioni

**Learn more**

* More details about **GroupDocs.Redaction** configuration: [Extend supported extensions list](https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/)
* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Esempi

Il seguente esempio dimostra come impostare le proprietà per una configurazione di formato personalizzata.

```csharp
var adobePhotoshopSettings = new DocumentFormatConfiguration();
adobePhotoshopSettings.ExtensionFilter = ".psd";
adobePhotoshopSettings.DocumentType = typeof(MyAdobePhotoshopFormatInstance);
```

### Vedi anche

* namespace [GroupDocs.Redaction.Configuration](../../groupdocs.redaction.configuration)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
