---
title: "RegexRedaction"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta una redazione del testo che ricerca e sostituisce il testo nel documento corrispondendo all'espressione regolare fornita."
type: docs
weight: 750
url: /it/net/groupdocs.redaction.redactions/regexredaction/
---
## RegexRedaction class

Rappresenta una redazione del testo che ricerca e sostituisce il testo nel documento corrispondendo all'espressione regolare fornita.

```csharp
public class RegexRedaction : TextRedaction
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [RegexRedaction](regexredaction#constructor_1)(Regex, ReplacementOptions) | Inizializza una nuova istanza della classe RegexRedaction. |
| [RegexRedaction](regexredaction#constructor)(string, ReplacementOptions) | Inizializza una nuova istanza della classe RegexRedaction. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | Restituisce l'istanza di [`ReplacementOptions`](../replacementoptions), specificando il tipo di sostituzione del testo. |
| override [Description](../../groupdocs.redaction.redactions/regexredaction/description) { get; } | Restituisce una stringa che descrive la redazione e i suoi parametri. |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | Ottiene o imposta l'implementazione di [`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector), necessaria per estrarre il testo dal contenuto grafico. |
| [RegularExpression](../../groupdocs.redaction.redactions/regexredaction/regularexpression) { get; } | Ottiene l'espressione regolare da corrispondere. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/regexredaction/applyto)(DocumentFormatInstance) | Applica la redazione a una determinata istanza di formato. |

### Osservazioni

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

### Esempi

Il seguente esempio dimostra la sostituzione del testo utilizzando l'espressione regolare.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
      // sostituisci con testo
      redactor.Apply(new RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", new ReplacementOptions("[removed]")));
      // sostituisci con rettangolo solido blu
      redactor.Apply(new RegexRedaction(@"^\d+[,\.]{1}\d+$", new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Blue)));
      redactor.Save();
    }
```

### Vedi anche

* class [TextRedaction](../textredaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
