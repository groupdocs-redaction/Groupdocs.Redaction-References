---
title: "CellColumnRedaction"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta una redazione di testo che sostituisce il testo in documenti di fogli di calcolo, CSV, Excel, ecc."
type: docs
weight: 540
url: /it/net/groupdocs.redaction.redactions/cellcolumnredaction/
---
## CellColumnRedaction class

Rappresenta una redazione di testo che sostituisce il testo nei documenti di foglio di calcolo (CSV, Excel, ecc.).

```csharp
public class CellColumnRedaction : TextRedaction
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [CellColumnRedaction](cellcolumnredaction)(CellFilter, Regex, ReplacementOptions) | Inizializza una nuova istanza della classe CellColumnRedaction. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Restituisce l'istanza di [`ReplacementOptions`](../replacementoptions), specificando il tipo di sostituzione del testo. |
| override [Description](../../groupdocs.redaction.redactions/cellcolumnredaction/description) { get; } | Restituisce una stringa che descrive la redazione e i suoi parametri. |
| [Filter](../../groupdocs.redaction.redactions/cellcolumnredaction/filter) { get; } | Ottiene il filtro di colonna e foglio di lavoro. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Ottiene o imposta l'implementazione di [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector), necessaria per estrarre il testo dal contenuto grafico. |
| [Pattern](../../groupdocs.redaction.redactions/cellcolumnredaction/pattern) { get; } | Ottiene l'espressione regolare da corrispondere. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/cellcolumnredaction/applyto)(DocumentFormatInstance) | Applica la redazione a una determinata istanza di formato. |

### Osservazioni

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about spreadsheet redactions: [Spreadsheet redactions](https://docs.groupdocs.com/redaction/net/spreadsheet-redactions/)

### Esempi

Il seguente esempio dimostra la rimozione delle email degli utenti da una seconda colonna nel foglio di lavoro "Customers" di un documento di foglio di calcolo.

```csharp
using (Redactor redactor = new Redactor("D:\\Sales in September.xslx"))
{
   var filter = new CellFilter()
   {
       ColumnIndex = 1, // zero-based 2nd column
       WorkSheetName = "Customers"
   };
   var expression = new Regex("^\\w+([-+.']\\w+)*@\\w+([-.]\\w+)*\\.\\w+([-.]\\w+)*$");
   RedactorChangeLog changeLog = redactor.Apply(new CellColumnRedaction(filter, expression, new ReplacementOptions("[customer email]")));
   if (result.Status != RedactionStatus.Failed)
   {
      doc.Save(new SaveOptions() { AddSuffix = true });
   };
}
```

### Vedi anche

* class [TextRedaction](../textredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
