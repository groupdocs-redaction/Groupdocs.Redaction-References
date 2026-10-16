---
title: "RedactionResult"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta il risultato dell'operazione di redazione."
type: docs
weight: 510
url: /it/net/groupdocs.redaction/redactionresult/
---
## RedactionResult class

Rappresenta il risultato dell'operazione di redazione.

```csharp
public class RedactionResult
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ErrorMessage](../../groupdocs.redaction/redactionresult/errormessage) { get; } | Ottiene il messaggio di errore per la diagnostica. |
| [Status](../../groupdocs.redaction/redactionresult/status) { get; } | Ottiene lo stato di esecuzione. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [Failed](../../groupdocs.redaction/redactionresult/failed)(string) | Inizializza una nuova istanza della classe RedactionResult con stato Failed. |
| static [Partial](../../groupdocs.redaction/redactionresult/partial)(string) | Inizializza una nuova istanza della classe RedactionResult con stato PartiallyApplied. |
| static [Skipped](../../groupdocs.redaction/redactionresult/skipped)(string) | Inizializza una nuova istanza della classe RedactionResult con stato Skipped. |
| static [Successful](../../groupdocs.redaction/redactionresult/successful)() | Inizializza una nuova istanza della classe RedactionResult con stato Applied (successful). |

### Osservazioni

**Learn more**

* More details about redaction results: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)

### Vedi anche

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
