---
title: "TextRedaction"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta una classe astratta di base per le redazioni del testo del documento."
type: docs
weight: 800
url: /it/net/groupdocs.redaction.redactions/textredaction/
---
## TextRedaction class

Rappresenta una classe astratta di base per le redazioni del testo del documento.

```csharp
public abstract class TextRedaction : Redaction
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Restituisce l'istanza di [`ReplacementOptions`](../replacementoptions), specificando il tipo di sostituzione del testo. |
| virtual [Description](../../groupdocs.redaction/redaction/description) { get; } | Restituisce una stringa che descrive la redazione e i suoi parametri. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Ottiene o imposta l'implementazione di [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector), necessaria per estrarre il testo dal contenuto grafico. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| abstract [ApplyTo](../../groupdocs.redaction/redaction/applyto)(DocumentFormatInstance) | Applica la redazione a una determinata istanza di formato. |

### Osservazioni

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

### Vedi anche

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
