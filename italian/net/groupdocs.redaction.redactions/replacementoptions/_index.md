---
title: "ReplacementOptions"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta le opzioni per la sostituzione del testo corrispondente."
type: docs
weight: 780
url: /it/net/groupdocs.redaction.redactions/replacementoptions/
---
## ReplacementOptions class

Rappresenta le opzioni per la sostituzione del testo corrispondente.

```csharp
public class ReplacementOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ReplacementOptions](replacementoptions#constructor)(Color) | Inizializza una nuova istanza della classe ReplacementOptions con rettangolo colorato come opzione. |
| [ReplacementOptions](replacementoptions#constructor_1)(string) | Inizializza una nuova istanza della classe ReplacementOptions con testo di sostituzione come opzione. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ActionType](../../groupdocs.redaction.redactions/replacementoptions/actiontype) { get; } | Ottiene l'azione di sostituzione: disegnare un riquadro o sostituire il testo. |
| [BoxColor](../../groupdocs.redaction.redactions/replacementoptions/boxcolor) { get; set; } | Ottiene o imposta il colore per l'opzione DrawBox (altrimenti ignorato). |
| [CustomRedaction](../../groupdocs.redaction.redactions/replacementoptions/customredaction) { get; set; } | Ottiene o imposta un gestore di redazione personalizzato [`ICustomRedactionHandler`](../icustomredactionhandler) che consente agli utenti di definire la propria logica di redazione. |
| [Filters](../../groupdocs.redaction.redactions/replacementoptions/filters) { get; set; } | Ottiene o imposta un array di filtri da applicare con questa redazione. |
| [Replacement](../../groupdocs.redaction.redactions/replacementoptions/replacement) { get; set; } | Ottiene o imposta il valore di sostituzione testuale. |

### Osservazioni

**Learn more**

* More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)
* More details about redaction filters: [Use PDF redaction filters](https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/)

### Vedi anche

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
