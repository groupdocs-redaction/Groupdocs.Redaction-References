---
title: "RedactorConfiguration"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Fornisce l'accesso a un elenco di formati supportati, integrati e formati personalizzati dell'utente."
type: docs
weight: 20
url: /it/net/groupdocs.redaction.configuration/redactorconfiguration/
---
## RedactorConfiguration class

Fornisce l'accesso a un elenco di formati supportati, integrati e formati personalizzati dell'utente.

```csharp
public class RedactorConfiguration
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AvailableFormats](../../groupdocs.redaction.configuration/redactorconfiguration/availableformats) { get; } | Ottiene un elenco di formati riconosciuti, vedi [`DocumentFormatConfiguration`](../documentformatconfiguration). |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [GetInstance](../../groupdocs.redaction.configuration/redactorconfiguration/getinstance)() | Fornisce un'istanza singleton con la configurazione predefinita dei formati integrati. |
| [FindFormat](../../groupdocs.redaction.configuration/redactorconfiguration/findformat)(string) | Trova le configurazioni di formato per una determinata estensione di file. |

### Osservazioni

**Learn more**

* More details about **GroupDocs.Redaction** configuration: [Extend supported extensions list](https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/)
* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Esempi

Il seguente esempio dimostra come aggiungere un gestore di formato personalizzato dell'utente.

```csharp
var adobePhotoshopSettings = new DocumentFormatConfiguration();
adobePhotoshopSettings.ExtensionFilter = ".psd";
adobePhotoshopSettings.DocumentType = typeof(MyAdobePhotoshopFormatInstance);
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(adobePhotoshopSettings);
```

Il seguente esempio dimostra come ottenere gestori di formato integrati o personalizzati dell'utente.

```csharp
var configuration = RedactorConfiguration.GetInstance();
var formatSettings = configuration.FindFormat(".psd");
```

### Vedi anche

* namespace [GroupDocs.Redaction.Configuration](../../groupdocs.redaction.configuration)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
