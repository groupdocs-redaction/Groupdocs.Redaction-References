---
title: "RedactorSettings"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta le impostazioni di redazione che consentono di personalizzare il processo di redazione."
type: docs
weight: 430
url: /it/net/groupdocs.redaction.options/redactorsettings/
---
## RedactorSettings class

Rappresenta le impostazioni di redazione, consentendo di personalizzare il processo di redazione.

```csharp
public class RedactorSettings
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [RedactorSettings](redactorsettings#constructor)() | Inizializza una nuova istanza della classe RedactorSettings. |
| [RedactorSettings](redactorsettings#constructor_2)(ILogger) | Inizializza una nuova istanza della classe RedactorSettings con una determinata istanza di ILogger. |
| [RedactorSettings](redactorsettings#constructor_1)(IOcrConnector) | Inizializza una nuova istanza della classe RedactorSettings con una determinata istanza di IOcrConnector. |
| [RedactorSettings](redactorsettings#constructor_5)(IRedactionCallback) | Inizializza una nuova istanza della classe RedactorSettings con una determinata istanza di IRedactionCallback. |
| [RedactorSettings](redactorsettings#constructor_3)(ILogger, IRedactionCallback) | Inizializza una nuova istanza della classe RedactorSettings con le istanze fornite di ILogger e IRedactionCallback. |
| [RedactorSettings](redactorsettings#constructor_4)(ILogger, IRedactionCallback, IOcrConnector) | Inizializza una nuova istanza della classe RedactorSettings con le istanze fornite di ILogger, IRedactionCallback e IOcrConnector. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Logger](../../groupdocs.redaction.options/redactorsettings/logger) { get; set; } | Ottiene o imposta un'istanza di una classe, che implementa [`ILogger`](../ilogger), utilizzata per registrare eventi ed errori. |
| [OcrConnector](../../groupdocs.redaction.options/redactorsettings/ocrconnector) { get; set; } | Ottiene o imposta un'istanza di una classe, che implementa l'interfaccia [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector). |
| [RedactionCallback](../../groupdocs.redaction.options/redactorsettings/redactioncallback) { get; set; } | Ottiene o imposta un'istanza di una classe, che implementa [`IRedactionCallback`](../../groupdocs.redaction.redactions/iredactioncallback). |

### Osservazioni

**Learn more**

* More details about implementing ILogger interface: [Use advanced logging](https://docs.groupdocs.com/redaction/net/use-advanced-logging/)
* More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

### Vedi anche

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
