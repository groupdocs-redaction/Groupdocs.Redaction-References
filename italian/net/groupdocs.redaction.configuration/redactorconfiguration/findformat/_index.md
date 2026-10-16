---
title: "FindFormat"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Trova le configurazioni di formato per una determinata estensione di file."
type: docs
weight: 30
url: /it/net/groupdocs.redaction.configuration/redactorconfiguration/findformat/
---
## RedactorConfiguration.FindFormat method

Trova le configurazioni di formato per una determinata estensione di file.

```csharp
public DocumentFormatConfiguration FindFormat(string fileExtension)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileExtension | String | Estensione file, il formato è ".ext" |

### Valore di ritorno

Se trovato, istanza di [`DocumentFormatConfiguration`](../../documentformatconfiguration), altrimenti null

### Esempi

Il seguente esempio dimostra come ottenere gestori di formato integrati o personalizzati dell'utente.

```csharp
var configuration = RedactorConfiguration.GetInstance();
var formatSettings = configuration.FindFormat(".psd");
```

### Vedi anche

* class [DocumentFormatConfiguration](../../documentformatconfiguration)
* class [RedactorConfiguration](../../redactorconfiguration)
* namespace [GroupDocs.Redaction.Configuration](../../../groupdocs.redaction.configuration)
* assembly [GroupDocs.Redaction](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
