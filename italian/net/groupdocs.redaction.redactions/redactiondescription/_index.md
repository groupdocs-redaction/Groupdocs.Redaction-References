---
title: "RedactionDescription"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta le informazioni di una singola azione di modifica eseguita durante il processo di redazione."
type: docs
weight: 720
url: /it/net/groupdocs.redaction.redactions/redactiondescription/
---
## RedactionDescription class

Rappresenta le informazioni di una singola azione di modifica eseguita durante il processo di redazione.

```csharp
public class RedactionDescription
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [RedactionDescription](redactiondescription#constructor_1)(RedactionType, RedactionActionType, string) | Inizializza una nuova istanza della classe RedactionDescription senza informazioni di sostituzione. |
| [RedactionDescription](redactiondescription#constructor)(RedactionType, RedactionActionType, RegionReplacementOptions, string) | Inizializza una nuova istanza della classe RedactionDescription con informazioni di sostituzione dell'area immagine. |
| [RedactionDescription](redactiondescription#constructor_2)(RedactionType, RedactionActionType, string, TextReplacement) | Inizializza una nuova istanza della classe RedactionDescription con informazioni di sostituzione. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ActionType](../../groupdocs.redaction.redactions/redactiondescription/actiontype) { get; } | Ottiene l'operazione di redazione: sostituzione, pulizia o eliminazione. |
| [Details](../../groupdocs.redaction.redactions/redactiondescription/details) { get; set; } | Ottiene o imposta informazioni opzionali sui dettagli per l'elemento redatto. |
| [ImageAreaReplacement](../../groupdocs.redaction.redactions/redactiondescription/imageareareplacement) { get; } | Ottiene le informazioni di sostituzione per le redazioni dell'area immagine, restituisce null per le redazioni testuali. |
| [OriginalText](../../groupdocs.redaction.redactions/redactiondescription/originaltext) { get; } | Ottiene il testo corrispondente, se è fornita un'espressione. |
| [RedactionType](../../groupdocs.redaction.redactions/redactiondescription/redactiontype) { get; } | Ottiene il tipo di dati del documento - testo, metadati o annotazioni. |
| [Replacement](../../groupdocs.redaction.redactions/redactiondescription/replacement) { get; } | Ottiene le informazioni di sostituzione, può essere null. |

### Osservazioni

**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

### Vedi anche

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
