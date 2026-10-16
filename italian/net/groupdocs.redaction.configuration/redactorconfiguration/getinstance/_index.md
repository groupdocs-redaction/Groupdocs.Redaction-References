---
title: "GetInstance"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Fornisce un'istanza singleton con la configurazione predefinita dei formati incorporati."
type: docs
weight: 10
url: /it/net/groupdocs.redaction.configuration/redactorconfiguration/getinstance/
---
## RedactorConfiguration.GetInstance method

Fornisce un'istanza singleton con la configurazione predefinita dei formati integrati.

```csharp
public static RedactorConfiguration GetInstance()
```

### Valore di ritorno

Istanza di configurazione

### Esempi

Il seguente esempio dimostra come aggiungere un gestore di formato personalizzato.

```csharp
var adobePhotoshopSettings = new DocumentFormatConfiguration();
adobePhotoshopSettings.ExtensionFilter = ".psd";
adobePhotoshopSettings.DocumentType = typeof(MyAdobePhotoshopFormatInstance);
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(adobePhotoshopSettings);
```

### Vedi anche

* class [RedactorConfiguration](../../redactorconfiguration)
* namespace [GroupDocs.Redaction.Configuration](../../../groupdocs.redaction.configuration)
* assembly [GroupDocs.Redaction](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
